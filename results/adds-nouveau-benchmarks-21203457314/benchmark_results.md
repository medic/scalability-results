# CouchDb Performance benchmark 

## Database Info

CouchDb version: 3.5.0

Database doc count: 903030

## _changes benchmark 
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 36 |
| 1000 |  |  |  |  | 106 |
| 10000 |  |  |  |  | 626 |
| 100 |  | true |  |  | 43 |
| 1000 |  | true |  |  | 128 |
| 10000 |  | true |  |  | 969 |
| 100 |  |  | 100 |  | 49 |
| 1000 |  |  | 1000 |  | 38 |
| 10000 |  |  | 10000 |  | 140 |
| 100 | Mid Sequence |  |  |  | 40 |
| 1000 | Mid Sequence |  |  |  | 96 |
| 10000 | Mid Sequence |  |  |  | 587 |
| 100 | Mid Sequence | true |  |  | 41 |
| 1000 | Mid Sequence | true |  |  | 138 |
| 10000 | Mid Sequence | true |  |  | 987 |
| 100 | Mid Sequence |  | 100 |  | 34 |
| 1000 | Mid Sequence |  | 1000 |  | 37 |
| 10000 | Mid Sequence |  | 10000 |  | 140 |
| 10000 |  |  |  | true | 1535 |
| 10000 |  | true |  | true | 3047 |
| 10000 |  |  | 10000 | true | 996 |


## _all_docs benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 32 |
| 1000 |  |  | 40 |
| 10000 |  |  | 179 |
| 100 | true |  | 31 |
| 1000 | true |  | 80 |
| 10000 | true |  | 561 |
| 10000 |  | true | 1191 |
| 10000 | true | true | 1461 |


## _bulk_get benchmark 
| count| Duration (ms) |
|--|--|
| 100 | 31 |
| 1000 | 77 |
| 10000 | 725 |


## view benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 29 |
| 1000 |  |  | 51 |
| 10000 |  |  | 253 |
| 100 | true |  | 42 |
| 1000 | true |  | 128 |
| 10000 | true |  | 1044 |
| 100 |  | true | 88 |
| 1000 |  | true | 96 |
| 10000 |  | true | 86 |
| 10000 | true | true | 99 |


## nouveau_index benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 135 |
| 1000 |  |  | 307 |
| 10000 |  |  | 2158 |
| 100 | true |  | 86 |
| 1000 | true |  | 333 |
| 10000 | true |  | 3784 |
| 100 |  | true | 49 |
| 1000 |  | true | 277 |
| 10000 |  | true | 1886 |
| 10000 | true | true | 3081 |


