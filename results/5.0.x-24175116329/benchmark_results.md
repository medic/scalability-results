# CouchDb Performance benchmark 

## Database Info

CouchDb version: 3.5.0

Database doc count: 903030

## _changes benchmark 
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 30 |
| 1000 |  |  |  |  | 98 |
| 10000 |  |  |  |  | 791 |
| 100 |  | true |  |  | 37 |
| 1000 |  | true |  |  | 527 |
| 10000 |  | true |  |  | 1200 |
| 100 |  |  | 100 |  | 243 |
| 1000 |  |  | 1000 |  | 561 |
| 10000 |  |  | 10000 |  | 525 |
| 100 | Mid Sequence |  |  |  | 33 |
| 1000 | Mid Sequence |  |  |  | 148 |
| 10000 | Mid Sequence |  |  |  | 1345 |
| 100 | Mid Sequence | true |  |  | 37 |
| 1000 | Mid Sequence | true |  |  | 134 |
| 10000 | Mid Sequence | true |  |  | 1028 |
| 100 | Mid Sequence |  | 100 |  | 144 |
| 1000 | Mid Sequence |  | 1000 |  | 49 |
| 10000 | Mid Sequence |  | 10000 |  | 131 |
| 10000 |  |  |  | true | 1461 |
| 10000 |  | true |  | true | 1884 |
| 10000 |  |  | 10000 | true | 998 |


## _all_docs benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 27 |
| 1000 |  |  | 37 |
| 10000 |  |  | 193 |
| 100 | true |  | 30 |
| 1000 | true |  | 83 |
| 10000 | true |  | 610 |
| 10000 |  | true | 1280 |
| 10000 | true | true | 1592 |


## _bulk_get benchmark 
| count| Duration (ms) |
|--|--|
| 100 | 29 |
| 1000 | 78 |
| 10000 | 726 |


