---
name: Independent researcher
about: Report Sybil Activity on LayerZero
title: "[Sybil Report]"
labels: under review
assignees: LayerZero-GH

---

# Reported Addresses

I have provided full list of addresses in report.txt file

# Description

My solution I can separate on 2 parts:
1. Filtering input data
2. Clustering addresses into batches based on their chain activity.

# Detailed Methodology & Walkthrough

## Filtering input data

I downloaded snapshot file `2024-05-15-snapshot1_transactions.tar`. 

After that I filtered this file in different files following next pattern `"/projects/<project>/<source_chain>-<destination_chain>.csv"`

So I got a directories of projects and `.csv` file with transfers between chains.

Implementation of this algorithm you can find here

## Clustering addresses into batches based on their chain activity.

After filtering I faced with problem how to cluster addresses. So I decided to check their activity in Stargate between Arbitrum and Optimism. And I have found that some of addresses regularly send transactions together at the same time. So I decided to write small script to find batch of addresses and count how often they make transactions in one block.

After that I made an assumption how many addresses should be in the batch and how often should they make transactions together to call them sybil activity.

# Algorithm Methodology:
### 1. First of all I go through all transactions between 2 chains on one project and store data in HastTable. We also insure that there will be not address dublication further

    ```HashTable: sender_wallet -> Set(source_timestamp_utc, ...)```
   
### 2. After that I change key and value of HastTable, but set is unhashable, so I change it to Tuple

    ```HashTable: Tuple(source_timestamp_utc) -> [sender_wallet, ...]```

### 3. And last step is to reduce extra transactions from Tuple to group up wallets

Before:
```
{
    (source_timestamp_utc1, source_timestamp_utc2) -> [sender_wallet1, sender_wallet2],
    (source_timestamp_utc1, source_timestamp_utc2, source_timestamp_utc3) -> [sender_wallet3]
}
```

After:
```
{
    (source_timestamp_utc1, source_timestamp_utc2) -> [sender_wallet1, sender_wallet2, sender_wallet3]
}
```

I also deside that if 5 or more addresses are found in one block 4 or more times it looks like activity based on automatic transactions sending, because of low probability for this in case of organic activity (I should remind that I made this algorithm based on data filtered by project and source_chain/destination_chain only).
It's also possible to change this parameters, so please write comment and I will resubmit report.txt

Implementation of this algorithm you can find here

# Reward Address (If Eligible)
0x9aA85330c79D390Df46dD3e2fAE5dC33E175f18f
