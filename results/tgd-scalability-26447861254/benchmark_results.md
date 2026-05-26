# CouchDb Performance benchmark 

## Database Info

CouchDb version: 3.5.0

Database doc count: 903030

## _changes benchmark 
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 32 |
| 1000 |  |  |  |  | 86 |
| 10000 |  |  |  |  | 655 |
| 100 |  | true |  |  | 43 |
| 1000 |  | true |  |  | 143 |
| 10000 |  | true |  |  | 1018 |
| 100 |  |  | 100 |  | 30 |
| 1000 |  |  | 1000 |  | 42 |
| 10000 |  |  | 10000 |  | 151 |
| 100 | Mid Sequence |  |  |  | 30 |
| 1000 | Mid Sequence |  |  |  | 79 |
| 10000 | Mid Sequence |  |  |  | 650 |
| 100 | Mid Sequence | true |  |  | 40 |
| 1000 | Mid Sequence | true |  |  | 132 |
| 10000 | Mid Sequence | true |  |  | 1069 |
| 100 | Mid Sequence |  | 100 |  | 39 |
| 1000 | Mid Sequence |  | 1000 |  | 33 |
| 10000 | Mid Sequence |  | 10000 |  | 146 |
| 10000 |  |  |  | true | 1455 |
| 10000 |  | true |  | true | 1919 |
| 10000 |  |  | 10000 | true | 1015 |


## _all_docs benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 22 |
| 1000 |  |  | 36 |
| 10000 |  |  | 200 |
| 100 | true |  | 27 |
| 1000 | true |  | 82 |
| 10000 | true |  | 679 |
| 10000 |  | true | 1293 |
| 10000 | true | true | 1597 |


## _bulk_get benchmark 
| count| Duration (ms) |
|--|--|
| 100 | 27 |
| 1000 | 81 |
| 10000 | 763 |


## view benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 120523 |
| 100 |  |  | 26 |
| 1000 |  |  | 51 |
| 10000 |  |  | 282 |
| 100 | true |  | 37 |
| 1000 | true |  | 144 |
| 10000 | true |  | 1164 |
| 100 |  | true | 90 |
| 1000 |  | true | 633 |
| 10000 |  | true | 5841 |
| 10000 | true | true | 6358 |


## nouveau_index benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 190456 |
| 100 |  |  | 267 |
| 1000 |  |  | 337 |
| 10000 |  |  | 2601 |
| 100 | true |  | 75 |
| 1000 | true |  | 976 |
| 10000 | true |  | 9231 |
| 100 |  | true | 394 |
| 1000 |  | true | 15541 |
| 10000 |  | true | 15276 |
| 10000 | true | true | 2748 |


