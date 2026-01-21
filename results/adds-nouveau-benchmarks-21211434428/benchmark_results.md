# CouchDb Performance benchmark 

## Database Info

CouchDb version: 3.5.0

Database doc count: 903030

## _changes benchmark 
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 33 |
| 1000 |  |  |  |  | 103 |
| 10000 |  |  |  |  | 615 |
| 100 |  | true |  |  | 37 |
| 1000 |  | true |  |  | 139 |
| 10000 |  | true |  |  | 1022 |
| 100 |  |  | 100 |  | 32 |
| 1000 |  |  | 1000 |  | 35 |
| 10000 |  |  | 10000 |  | 141 |
| 100 | Mid Sequence |  |  |  | 40 |
| 1000 | Mid Sequence |  |  |  | 100 |
| 10000 | Mid Sequence |  |  |  | 617 |
| 100 | Mid Sequence | true |  |  | 40 |
| 1000 | Mid Sequence | true |  |  | 128 |
| 10000 | Mid Sequence | true |  |  | 1076 |
| 100 | Mid Sequence |  | 100 |  | 26 |
| 1000 | Mid Sequence |  | 1000 |  | 36 |
| 10000 | Mid Sequence |  | 10000 |  | 136 |
| 10000 |  |  |  | true | 1558 |
| 10000 |  | true |  | true | 1985 |
| 10000 |  |  | 10000 | true | 1033 |


## _all_docs benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 25 |
| 1000 |  |  | 37 |
| 10000 |  |  | 214 |
| 100 | true |  | 33 |
| 1000 | true |  | 94 |
| 10000 | true |  | 645 |
| 10000 |  | true | 1260 |
| 10000 | true | true | 1613 |


## _bulk_get benchmark 
| count| Duration (ms) |
|--|--|
| 100 | 30 |
| 1000 | 78 |
| 10000 | 763 |


## view benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 28 |
| 1000 |  |  | 48 |
| 10000 |  |  | 277 |
| 100 | true |  | 39 |
| 1000 | true |  | 132 |
| 10000 | true |  | 1148 |
| 100 |  | true | 90 |
| 1000 |  | true | 601 |
| 10000 |  | true | 7227 |
| 10000 | true | true | 6587 |


## nouveau_index benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 146 |
| 1000 |  |  | 1044 |
| 10000 |  |  | 2437 |
| 100 | true |  | 79 |
| 1000 | true |  | 387 |
| 10000 | true |  | 3513 |
| 100 |  | true | 52 |
| 1000 |  | true | 261 |
| 10000 |  | true | 2142 |
| 10000 | true | true | 3610 |


