# CouchDb Performance benchmark 

## Database Info

CouchDb version: 3.5.0

Database doc count: 903030

## _changes benchmark 
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 20 |
| 1000 |  |  |  |  | 80 |
| 10000 |  |  |  |  | 662 |
| 100 |  | true |  |  | 25 |
| 1000 |  | true |  |  | 112 |
| 10000 |  | true |  |  | 1008 |
| 100 |  |  | 100 |  | 15 |
| 1000 |  |  | 1000 |  | 21 |
| 10000 |  |  | 10000 |  | 124 |
| 100 | Mid Sequence |  |  |  | 20 |
| 1000 | Mid Sequence |  |  |  | 78 |
| 10000 | Mid Sequence |  |  |  | 628 |
| 100 | Mid Sequence | true |  |  | 24 |
| 1000 | Mid Sequence | true |  |  | 112 |
| 10000 | Mid Sequence | true |  |  | 966 |
| 100 | Mid Sequence |  | 100 |  | 17 |
| 1000 | Mid Sequence |  | 1000 |  | 34 |
| 10000 | Mid Sequence |  | 10000 |  | 120 |
| 10000 |  |  |  | true | 1438 |
| 10000 |  | true |  | true | 1825 |
| 10000 |  |  | 10000 | true | 976 |


## _all_docs benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 12 |
| 1000 |  |  | 27 |
| 10000 |  |  | 193 |
| 100 | true |  | 22 |
| 1000 | true |  | 74 |
| 10000 | true |  | 608 |
| 10000 |  | true | 1246 |
| 10000 | true | true | 1539 |


## _bulk_get benchmark 
| count| Duration (ms) |
|--|--|
| 100 | 16 |
| 1000 | 59 |
| 10000 | 707 |


