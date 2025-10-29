# CouchDb Performance benchmark 

## Database Info

CouchDb version: 3.5.0

Database doc count: 903030

## _changes benchmark 
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 38 |
| 1000 |  |  |  |  | 105 |
| 10000 |  |  |  |  | 714 |
| 100 |  | true |  |  | 42 |
| 1000 |  | true |  |  | 146 |
| 10000 |  | true |  |  | 1063 |
| 100 |  |  | 100 |  | 37 |
| 1000 |  |  | 1000 |  | 35 |
| 10000 |  |  | 10000 |  | 147 |
| 100 | Mid Sequence |  |  |  | 32 |
| 1000 | Mid Sequence |  |  |  | 107 |
| 10000 | Mid Sequence |  |  |  | 719 |
| 100 | Mid Sequence | true |  |  | 37 |
| 1000 | Mid Sequence | true |  |  | 132 |
| 10000 | Mid Sequence | true |  |  | 2940 |
| 100 | Mid Sequence |  | 100 |  | 179 |
| 1000 | Mid Sequence |  | 1000 |  | 35 |
| 10000 | Mid Sequence |  | 10000 |  | 145 |
| 10000 |  |  |  | true | 1576 |
| 10000 |  | true |  | true | 2000 |
| 10000 |  |  | 10000 | true | 1038 |


## _all_docs benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 25 |
| 1000 |  |  | 46 |
| 10000 |  |  | 199 |
| 100 | true |  | 33 |
| 1000 | true |  | 110 |
| 10000 | true |  | 611 |
| 10000 |  | true | 1345 |
| 10000 | true | true | 1688 |


## _bulk_get benchmark 
| count| Duration (ms) |
|--|--|
| 100 | 30 |
| 1000 | 72 |
| 10000 | 827 |


