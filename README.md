# LayerZero Sybil Reporting

The [deadline to self-report](https://sybil.layerzero.network/) as a sybil is May 18th, 02:00 UTC, following the publication of the up-to-date list of self-reported and identified sybil addresses found by LayerZero Foundation, Chaos Labs, and Nansen. This will mark the end of Phase 1 of [addressing sybil activity](https://medium.com/layerzero-official/addressing-sybil-activity-a2f92218ddd3). 

Phase 2 begins on May 18th at 02:00 UTC, during which anyone can submit a Sybil activity report. Successful reports will result in the sybil addresses receiving nothing and the bounty hunter receiving 10% of the sybil’s intended allocation. 

Bounty hunters can use the following information to start producing reports; however, submissions will not be open until May 18th at 02:00 UTC. Submissions received before the start time, and after the deadline, will not be considered.

**All transaction data prior to Snapshot #1 can be downloaded [here (Dropbox)](https://www.dropbox.com/scl/fo/m0ji3zbmbockvqkyl9353/ALYUg0-rLU2fuDMSd9nuB34?rlkey=kdu7zf877k919c34t754nxerc&st=qz5cfa1n&dl=0) or [here (S3 Bucket)](https://layerzerodataset.s3.us-east-2.amazonaws.com/snapshot1_transactions.csv.gz). The data is provided in two formats, one single csv file and a tar file that is split into smaller chunks.**

## Guidelines

- **Report Timeline:** Sybil activity must predate [Snapshot #1](https://twitter.com/LayerZero_Labs/status/1785821562475839843).
- **Excluded Addresses:** Bounty addresses must not overlap with the identified sybil list published by LayerZero, Nansen, and Chaos (which will include self-reported addresses). 
- **Minimum Address:** Reports must contain at least 20 addresses with clear methodology.
- **Disqualifications:** Reports including addresses already published, addresses with no LayerZero transactions, or reports lacking sufficient reasoning and/or methodology will be disqualified. 
- **Submission Deadline:** The deadline to submit reports is May 31st 23:59 UTC
- **Submission Review:** Bounty awarded to the first **eligible** report for a given sybil address.
- **Final Authority:** Eligibility of a submission is at the sole discretion of LayerZero Foundation and its best efforts to review all submissions.


# How to Report

Use the Issue Template within this Repository to provide the following:

### Sybil Addresses
Provide a list of LayerZero sybil addresses that would currently receive a token allocation and are not on the lists published by LayerZero, Nansen, and Chaos (which includes self-reported addresses).
### Reasoning 
Describe in detail the relationship between LayerZero addresses suspected of sybil. The goal is to determine how these addresses are linked to each other and/or linked to sybil activity. 
### Methodology 
Explain the method used to identify the addresses and provide proof that they are all controlled by a single individual or entity. The methodology should be easily verifiable, and have a low risk of misclassifying real users, otherwise the report will be deemed ineligible. Include links to any additional materials, such as a GitHub repo with the script used to uncover the reported addresses.
### Reward Address
Please provide an Ethereum address that will receive any potential rewards earned from this submission. Note: this cannot be claimed until TGE. All allocation eligibility will be subject to any legal or geographic requirements.


*This framework is inspired by previous work done by [Safe](https://github.com/safe-global/safe-user-allocation-reports/) and [Hop](https://github.com/hop-protocol/hop-airdrop).* 

