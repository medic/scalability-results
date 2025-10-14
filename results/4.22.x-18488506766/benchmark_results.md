# CouchDb Performance benchmark 

## Database Info

CouchDb version: 3.5.0

Database doc count: 903030

## _changes benchmark 
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 21 |
| 1000 |  |  |  |  | 84 |
| 10000 |  |  |  |  | 696 |
| 100 |  | true |  |  | 24 |
| 1000 |  | true |  |  | 114 |
| 10000 |  | true |  |  | 1019 |
| 100 |  |  | 100 |  | 16 |
| 1000 |  |  | 1000 |  | 21 |
| 10000 |  |  | 10000 |  | 132 |
| 100 | Mid Sequence |  |  |  | 20 |
| 1000 | Mid Sequence |  |  |  | 84 |
| 10000 | Mid Sequence |  |  |  | 595 |
| 100 | Mid Sequence | true |  |  | 22 |
| 1000 | Mid Sequence | true |  |  | 118 |
| 10000 | Mid Sequence | true |  |  | 1001 |
| 100 | Mid Sequence |  | 100 |  | 15 |
| 1000 | Mid Sequence |  | 1000 |  | 27 |
| 10000 | Mid Sequence |  | 10000 |  | 131 |
| 10000 |  |  |  | true | 1562 |
| 10000 |  | true |  | true | 1882 |
| 10000 |  |  | 10000 | true | 1008 |


## _all_docs benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 13 |
| 1000 |  |  | 27 |
| 10000 |  |  | 196 |
| 100 | true |  | 17 |
| 1000 | true |  | 72 |
| 10000 | true |  | 651 |
| 10000 |  | true | 1267 |
| 10000 | true | true | 1546 |


## _bulk_get benchmark 
| count| Duration (ms) |
|--|--|
| 100 | 15 |
| 1000 | 58 |
| 10000 | 696 |


