# CouchDb Performance benchmark 

## Database Info

CouchDb version: 3.5.0

Database doc count: 903030

## _changes benchmark 
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 20 |
| 1000 |  |  |  |  | 87 |
| 10000 |  |  |  |  | 627 |
| 100 |  | true |  |  | 25 |
| 1000 |  | true |  |  | 128 |
| 10000 |  | true |  |  | 1001 |
| 100 |  |  | 100 |  | 15 |
| 1000 |  |  | 1000 |  | 21 |
| 10000 |  |  | 10000 |  | 136 |
| 100 | Mid Sequence |  |  |  | 23 |
| 1000 | Mid Sequence |  |  |  | 78 |
| 10000 | Mid Sequence |  |  |  | 650 |
| 100 | Mid Sequence | true |  |  | 23 |
| 1000 | Mid Sequence | true |  |  | 104 |
| 10000 | Mid Sequence | true |  |  | 1026 |
| 100 | Mid Sequence |  | 100 |  | 17 |
| 1000 | Mid Sequence |  | 1000 |  | 21 |
| 10000 | Mid Sequence |  | 1000 |  | 123 |
| 10000 |  |  |  | true | 1532 |
| 10000 |  | true |  | true | 1917 |
| 10000 |  |  | 10000 | true | 1018 |


## _all_docs benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 12 |
| 1000 |  |  | 24 |
| 10000 |  |  | 186 |
| 100 | true |  | 19 |
| 1000 | true |  | 63 |
| 10000 | true |  | 611 |
| 10000 |  | true | 1333 |
| 10000 | true | true | 1620 |


## _bulk_get benchmark 
| count| Duration (ms) |
|--|--|
| 100 | 15 |
| 1000 | 61 |
| 10000 | 755 |


