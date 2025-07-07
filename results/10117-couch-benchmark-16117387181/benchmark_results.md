# CouchDb Performance benchmark 

## Database Info

CouchDb version: 3.5.0

Database doc count: 903030

## _changes benchmark 
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 20 |
| 1000 |  |  |  |  | 75 |
| 10000 |  |  |  |  | 552 |
| 100 |  | true |  |  | 22 |
| 1000 |  | true |  |  | 109 |
| 10000 |  | true |  |  | 1000 |
| 100 |  |  | 100 |  | 15 |
| 1000 |  |  | 1000 |  | 21 |
| 10000 |  |  | 10000 |  | 110 |
| 100 | Mid Sequence |  |  |  | 19 |
| 1000 | Mid Sequence |  |  |  | 76 |
| 10000 | Mid Sequence |  |  |  | 615 |
| 100 | Mid Sequence | true |  |  | 21 |
| 1000 | Mid Sequence | true |  |  | 112 |
| 10000 | Mid Sequence | true |  |  | 986 |
| 100 | Mid Sequence |  | 100 |  | 16 |
| 1000 | Mid Sequence |  | 1000 |  | 21 |
| 10000 | Mid Sequence |  | 1000 |  | 112 |
| 10000 |  |  |  | true | 1455 |
| 10000 |  | true |  | true | 1900 |
| 10000 |  |  | 10000 | true | 1023 |


## _all_docs benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 11 |
| 1000 |  |  | 23 |
| 10000 |  |  | 169 |
| 100 | true |  | 16 |
| 1000 | true |  | 72 |
| 10000 | true |  | 567 |
| 10000 |  | true | 1252 |
| 10000 | true | true | 1512 |


