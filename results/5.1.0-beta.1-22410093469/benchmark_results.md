# CouchDb Performance benchmark 

## Database Info

CouchDb version: 3.5.0

Database doc count: 903030

## _changes benchmark 
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 31 |
| 1000 |  |  |  |  | 103 |
| 10000 |  |  |  |  | 609 |
| 100 |  | true |  |  | 41 |
| 1000 |  | true |  |  | 140 |
| 10000 |  | true |  |  | 1039 |
| 100 |  |  | 100 |  | 37 |
| 1000 |  |  | 1000 |  | 39 |
| 10000 |  |  | 10000 |  | 154 |
| 100 | Mid Sequence |  |  |  | 44 |
| 1000 | Mid Sequence |  |  |  | 96 |
| 10000 | Mid Sequence |  |  |  | 685 |
| 100 | Mid Sequence | true |  |  | 36 |
| 1000 | Mid Sequence | true |  |  | 135 |
| 10000 | Mid Sequence | true |  |  | 1065 |
| 100 | Mid Sequence |  | 100 |  | 30 |
| 1000 | Mid Sequence |  | 1000 |  | 33 |
| 10000 | Mid Sequence |  | 10000 |  | 142 |
| 10000 |  |  |  | true | 1526 |
| 10000 |  | true |  | true | 1912 |
| 10000 |  |  | 10000 | true | 1058 |


## _all_docs benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 25 |
| 1000 |  |  | 42 |
| 10000 |  |  | 193 |
| 100 | true |  | 31 |
| 1000 | true |  | 82 |
| 10000 | true |  | 631 |
| 10000 |  | true | 1341 |
| 10000 | true | true | 1607 |


## _bulk_get benchmark 
| count| Duration (ms) |
|--|--|
| 100 | 28 |
| 1000 | 83 |
| 10000 | 754 |


## view benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 125819 |
| 100 |  |  | 34 |
| 1000 |  |  | 48 |
| 10000 |  |  | 274 |
| 100 | true |  | 41 |
| 1000 | true |  | 143 |
| 10000 | true |  | 1062 |
| 100 |  | true | 84 |
| 1000 |  | true | 593 |
| 10000 |  | true | 5816 |
| 10000 | true | true | 6200 |


## nouveau_index benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 194424 |
| 100 |  |  | 136 |
| 1000 |  |  | 341 |
| 10000 |  |  | 2378 |
| 100 | true |  | 84 |
| 1000 | true |  | 373 |
| 10000 | true |  | 3536 |
| 100 |  | true | 51 |
| 1000 |  | true | 390 |
| 10000 |  | true | 1757 |
| 10000 | true | true | 3095 |


