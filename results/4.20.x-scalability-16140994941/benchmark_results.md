# CouchDb Performance benchmark 

## Database Info

CouchDb version: 3.4.2

Database doc count: 903030

## _changes benchmark 
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 23 |
| 1000 |  |  |  |  | 81 |
| 10000 |  |  |  |  | 814 |
| 100 |  | true |  |  | 25 |
| 1000 |  | true |  |  | 143 |
| 10000 |  | true |  |  | 1279 |
| 100 |  |  | 100 |  | 17 |
| 1000 |  |  | 1000 |  | 25 |
| 10000 |  |  | 10000 |  | 138 |
| 100 | Mid Sequence |  |  |  | 21 |
| 1000 | Mid Sequence |  |  |  | 87 |
| 10000 | Mid Sequence |  |  |  | 792 |
| 100 | Mid Sequence | true |  |  | 27 |
| 1000 | Mid Sequence | true |  |  | 151 |
| 10000 | Mid Sequence | true |  |  | 1324 |
| 100 | Mid Sequence |  | 100 |  | 14 |
| 1000 | Mid Sequence |  | 1000 |  | 22 |
| 10000 | Mid Sequence |  | 1000 |  | 145 |
| 10000 |  |  |  | true | 1884 |
| 10000 |  | true |  | true | 2382 |
| 10000 |  |  | 10000 | true | 1203 |


## _all_docs benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 13 |
| 1000 |  |  | 28 |
| 10000 |  |  | 200 |
| 100 | true |  | 21 |
| 1000 | true |  | 75 |
| 10000 | true |  | 643 |
| 10000 |  | true | 1662 |
| 10000 | true | true | 1936 |


