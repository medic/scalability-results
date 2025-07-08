# CouchDb Performance benchmark 

## Database Info

CouchDb version: 3.5.0

Database doc count: 903030

## _changes benchmark 
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 19 |
| 1000 |  |  |  |  | 64 |
| 10000 |  |  |  |  | 560 |
| 100 |  | true |  |  | 22 |
| 1000 |  | true |  |  | 98 |
| 10000 |  | true |  |  | 951 |
| 100 |  |  | 100 |  | 13 |
| 1000 |  |  | 1000 |  | 18 |
| 10000 |  |  | 10000 |  | 102 |
| 100 | Mid Sequence |  |  |  | 17 |
| 1000 | Mid Sequence |  |  |  | 69 |
| 10000 | Mid Sequence |  |  |  | 573 |
| 100 | Mid Sequence | true |  |  | 19 |
| 1000 | Mid Sequence | true |  |  | 113 |
| 10000 | Mid Sequence | true |  |  | 956 |
| 100 | Mid Sequence |  | 100 |  | 13 |
| 1000 | Mid Sequence |  | 1000 |  | 19 |
| 10000 | Mid Sequence |  | 1000 |  | 105 |
| 10000 |  |  |  | true | 1431 |
| 10000 |  | true |  | true | 1816 |
| 10000 |  |  | 10000 | true | 952 |


## _all_docs benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 10 |
| 1000 |  |  | 24 |
| 10000 |  |  | 167 |
| 100 | true |  | 17 |
| 1000 | true |  | 67 |
| 10000 | true |  | 539 |
| 10000 |  | true | 1228 |
| 10000 | true | true | 1511 |


