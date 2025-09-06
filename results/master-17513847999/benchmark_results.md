# CouchDb Performance benchmark 

## Database Info

CouchDb version: 3.5.0

Database doc count: 903030

## _changes benchmark 
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 18 |
| 1000 |  |  |  |  | 82 |
| 10000 |  |  |  |  | 593 |
| 100 |  | true |  |  | 25 |
| 1000 |  | true |  |  | 119 |
| 10000 |  | true |  |  | 937 |
| 100 |  |  | 100 |  | 20 |
| 1000 |  |  | 1000 |  | 21 |
| 10000 |  |  | 10000 |  | 132 |
| 100 | Mid Sequence |  |  |  | 22 |
| 1000 | Mid Sequence |  |  |  | 77 |
| 10000 | Mid Sequence |  |  |  | 632 |
| 100 | Mid Sequence | true |  |  | 23 |
| 1000 | Mid Sequence | true |  |  | 113 |
| 10000 | Mid Sequence | true |  |  | 960 |
| 100 | Mid Sequence |  | 100 |  | 14 |
| 1000 | Mid Sequence |  | 1000 |  | 22 |
| 10000 | Mid Sequence |  | 10000 |  | 118 |
| 10000 |  |  |  | true | 1457 |
| 10000 |  | true |  | true | 1883 |
| 10000 |  |  | 10000 | true | 993 |


## _all_docs benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 12 |
| 1000 |  |  | 25 |
| 10000 |  |  | 189 |
| 100 | true |  | 19 |
| 1000 | true |  | 70 |
| 10000 | true |  | 608 |
| 10000 |  | true | 1219 |
| 10000 | true | true | 1521 |


## _bulk_get benchmark 
| count| Duration (ms) |
|--|--|
| 100 | 15 |
| 1000 | 62 |
| 10000 | 716 |


