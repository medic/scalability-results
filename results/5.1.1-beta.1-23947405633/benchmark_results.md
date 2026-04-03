# CouchDb Performance benchmark 

## Database Info

CouchDb version: 3.5.0

Database doc count: 903030

## _changes benchmark 
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 30 |
| 1000 |  |  |  |  | 96 |
| 10000 |  |  |  |  | 631 |
| 100 |  | true |  |  | 37 |
| 1000 |  | true |  |  | 134 |
| 10000 |  | true |  |  | 1022 |
| 100 |  |  | 100 |  | 30 |
| 1000 |  |  | 1000 |  | 32 |
| 10000 |  |  | 10000 |  | 149 |
| 100 | Mid Sequence |  |  |  | 33 |
| 1000 | Mid Sequence |  |  |  | 91 |
| 10000 | Mid Sequence |  |  |  | 598 |
| 100 | Mid Sequence | true |  |  | 39 |
| 1000 | Mid Sequence | true |  |  | 124 |
| 10000 | Mid Sequence | true |  |  | 1028 |
| 100 | Mid Sequence |  | 100 |  | 35 |
| 1000 | Mid Sequence |  | 1000 |  | 39 |
| 10000 | Mid Sequence |  | 10000 |  | 146 |
| 10000 |  |  |  | true | 1495 |
| 10000 |  | true |  | true | 1950 |
| 10000 |  |  | 10000 | true | 1060 |


## _all_docs benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 28 |
| 1000 |  |  | 37 |
| 10000 |  |  | 205 |
| 100 | true |  | 41 |
| 1000 | true |  | 78 |
| 10000 | true |  | 637 |
| 10000 |  | true | 1226 |
| 10000 | true | true | 1572 |


## _bulk_get benchmark 
| count| Duration (ms) |
|--|--|
| 100 | 29 |
| 1000 | 86 |
| 10000 | 787 |


## view benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 112075 |
| 100 |  |  | 28 |
| 1000 |  |  | 46 |
| 10000 |  |  | 258 |
| 100 | true |  | 49 |
| 1000 | true |  | 165 |
| 10000 | true |  | 1190 |
| 100 |  | true | 88 |
| 1000 |  | true | 604 |
| 10000 |  | true | 5617 |
| 10000 | true | true | 6267 |


## nouveau_index benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 173207 |
| 100 |  |  | 126 |
| 1000 |  |  | 466 |
| 10000 |  |  | 2167 |
| 100 | true |  | 79 |
| 1000 | true |  | 338 |
| 10000 | true |  | 3130 |
| 100 |  | true | 59 |
| 1000 |  | true | 214 |
| 10000 |  | true | 1663 |
| 10000 | true | true | 2911 |


