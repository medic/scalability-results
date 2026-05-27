# CouchDb Performance benchmark 

## Database Info

CouchDb version: 3.5.0

Database doc count: 903030

## _changes benchmark 
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 37 |
| 1000 |  |  |  |  | 125 |
| 10000 |  |  |  |  | 939 |
| 100 |  | true |  |  | 43 |
| 1000 |  | true |  |  | 173 |
| 10000 |  | true |  |  | 1577 |
| 100 |  |  | 100 |  | 33 |
| 1000 |  |  | 1000 |  | 41 |
| 10000 |  |  | 10000 |  | 170 |
| 100 | Mid Sequence |  |  |  | 37 |
| 1000 | Mid Sequence |  |  |  | 123 |
| 10000 | Mid Sequence |  |  |  | 1116 |
| 100 | Mid Sequence | true |  |  | 43 |
| 1000 | Mid Sequence | true |  |  | 163 |
| 10000 | Mid Sequence | true |  |  | 1600 |
| 100 | Mid Sequence |  | 100 |  | 36 |
| 1000 | Mid Sequence |  | 1000 |  | 45 |
| 10000 | Mid Sequence |  | 10000 |  | 196 |
| 10000 |  |  |  | true | 2096 |
| 10000 |  | true |  | true | 2462 |
| 10000 |  |  | 10000 | true | 1224 |


## _all_docs benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 47 |
| 1000 |  |  | 59 |
| 10000 |  |  | 265 |
| 100 | true |  | 51 |
| 1000 | true |  | 104 |
| 10000 | true |  | 828 |
| 10000 |  | true | 1599 |
| 10000 | true | true | 2216 |


## _bulk_get benchmark 
| count| Duration (ms) |
|--|--|
| 100 | 32 |
| 1000 | 110 |
| 10000 | 1038 |


## view benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 130200 |
| 100 |  |  | 34 |
| 1000 |  |  | 70 |
| 10000 |  |  | 434 |
| 100 | true |  | 42 |
| 1000 | true |  | 154 |
| 10000 | true |  | 1431 |
| 100 |  | true | 93 |
| 1000 |  | true | 641 |
| 10000 |  | true | 5879 |
| 10000 | true | true | 7052 |


## nouveau_index benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 238163 |
| 100 |  |  | 97 |
| 1000 |  |  | 428 |
| 10000 |  |  | 3665 |
| 100 | true |  | 102 |
| 1000 | true |  | 599 |
| 10000 | true |  | 4762 |
| 100 |  | true | 90 |
| 1000 |  | true | 381 |
| 10000 |  | true | 2656 |
| 10000 | true | true | 4227 |


