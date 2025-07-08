# CouchDb Performance benchmark 

## Database Info

CouchDb version: 3.4.2

Database doc count: 903030

## _changes benchmark 
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 21 |
| 1000 |  |  |  |  | 89 |
| 10000 |  |  |  |  | 866 |
| 100 |  | true |  |  | 28 |
| 1000 |  | true |  |  | 142 |
| 10000 |  | true |  |  | 1398 |
| 100 |  |  | 100 |  | 19 |
| 1000 |  |  | 1000 |  | 26 |
| 10000 |  |  | 10000 |  | 144 |
| 100 | Mid Sequence |  |  |  | 45 |
| 1000 | Mid Sequence |  |  |  | 99 |
| 10000 | Mid Sequence |  |  |  | 806 |
| 100 | Mid Sequence | true |  |  | 29 |
| 1000 | Mid Sequence | true |  |  | 151 |
| 10000 | Mid Sequence | true |  |  | 1370 |
| 100 | Mid Sequence |  | 100 |  | 29 |
| 1000 | Mid Sequence |  | 1000 |  | 34 |
| 10000 | Mid Sequence |  | 1000 |  | 152 |
| 10000 |  |  |  | true | 1937 |
| 10000 |  | true |  | true | 2513 |
| 10000 |  |  | 10000 | true | 1361 |


## _all_docs benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 15 |
| 1000 |  |  | 27 |
| 10000 |  |  | 209 |
| 100 | true |  | 24 |
| 1000 | true |  | 84 |
| 10000 | true |  | 690 |
| 10000 |  | true | 1609 |
| 10000 | true | true | 1883 |


