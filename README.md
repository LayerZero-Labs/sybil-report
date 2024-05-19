# LayerZero Sybil Reporting

The [deadline to self-report](https://sybil.layerzero.network/) as sybil has passed. The publication of the initial list of addresses that are not eligible for bounty hunting can be found [here](https://github.com/LayerZero-Labs/sybil-report/blob/main/initialList.txt).

Successful reports result in the sybil addresses receiving nothing and the bounty hunter receiving 10% of the sybil’s intended allocation. 

Bounty hunters can use the information below to produce a report; however, submissions after the deadline will not be considered.

**All transaction data prior to Snapshot #1 can be downloaded from Dropbox and AWS S3. The data is provided in two formats, one single csv file and a tar file that is split into smaller chunks.**
- [Dropbox Folder](https://www.dropbox.com/scl/fo/m0ji3zbmbockvqkyl9353/ALYUg0-rLU2fuDMSd9nuB34?rlkey=kdu7zf877k919c34t754nxerc&st=9t45y59t&dl=0)
- [S3 (csv)](https://layerzerodataset.s3.us-east-2.amazonaws.com/2024-05-15-snapshot1_transactions.csv.gz)
- [S3 (tar)](https://layerzerodataset.s3.us-east-2.amazonaws.com/2024-05-15-snapshot1_transactions.tar)

## Guidelines

- **Report Timeline:** Sybil activity must predate [Snapshot #1](https://twitter.com/LayerZero_Labs/status/1785821562475839843).
- **Excluded Addresses:** Bounty addresses must not overlap with the [initial list](https://github.com/LayerZero-Labs/sybil-report/blob/main/initialList.txt) published by LayerZero, Nansen, and Chaos (which will include self-reported addresses). 
- **Minimum Address:** Reports must contain at least 20 addresses with clear methodology.
- **Disqualifications:** Reports including a high number of addresses already published, addresses with no LayerZero transactions, or reports lacking sufficient reasoning and/or methodology will be disqualified. 
- **Submission Deadline:** The deadline to submit reports is May 31st 23:59 UTC
- **Submission Review:** Bounty awarded to the first **eligible** report for a given sybil address.
- **Final Authority:** Eligibility of a submission is at the sole discretion of LayerZero Foundation and its best efforts to review all submissions.


# How to Report

Use the [Issue Template](https://github.com/LayerZero-Labs/sybil-report/issues/new/choose) within this Repository to provide the following:

### Sybil Addresses
Provide a list of LayerZero sybil addresses that would currently receive a token allocation and are not on the lists published by LayerZero, Nansen, and Chaos (which includes self-reported addresses). If your report exceeds the issue character limit, you can add comments with the additional addresses directly to the issue. Avoid using external files.
### Reasoning 
Describe in detail the relationship between LayerZero addresses suspected of sybil. The goal is to determine how these addresses are linked to each other and/or linked to sybil activity. 
### Methodology 
Explain the method used to identify the addresses and provide proof that they are all controlled by a single individual or entity. The methodology should be easily verifiable, and have a low risk of misclassifying real users, otherwise the report will be deemed ineligible. You can report multiple sybil clusters in a single issue, provided that the same methodology applies to all accounts listed. Include references to any additional materials within the issue.
### Reward Address
Please provide an Ethereum address that will receive any potential rewards earned from this submission. Note: this cannot be claimed until TGE. All allocation eligibility will be subject to any legal or geographic requirements.


*This framework is inspired by previous work done by [Safe](https://github.com/safe-global/safe-user-allocation-reports/) and [Hop](https://github.com/hop-protocol/hop-airdrop).* 

