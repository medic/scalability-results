# CouchDb Performance benchmark 

## Database Info

CouchDb version: 3.5.0

Database doc count: 903030

## _changes benchmark 
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 32 |
| 1000 |  |  |  |  | 145 |
| 10000 |  |  |  |  | 953 |
| 100 |  | true |  |  | 46 |
| 1000 |  | true |  |  | 163 |
| 10000 |  | true |  |  | 1516 |
| 100 |  |  | 100 |  | 44 |
| 1000 |  |  | 1000 |  | 38 |
| 10000 |  |  | 10000 |  | 181 |
| 100 | Mid Sequence |  |  |  | 37 |
| 1000 | Mid Sequence |  |  |  | 107 |
| 10000 | Mid Sequence |  |  |  | 1013 |
| 100 | Mid Sequence | true |  |  | 39 |
| 1000 | Mid Sequence | true |  |  | 177 |
| 10000 | Mid Sequence | true |  |  | 1376 |
| 100 | Mid Sequence |  | 100 |  | 37 |
| 1000 | Mid Sequence |  | 1000 |  | 36 |
| 10000 | Mid Sequence |  | 10000 |  | 162 |
| 10000 |  |  |  | true | 1830 |
| 10000 |  | true |  | true | 2309 |
| 10000 |  |  | 10000 | true | 1093 |


## _all_docs benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 23 |
| 1000 |  |  | 57 |
| 10000 |  |  | 299 |
| 100 | true |  | 32 |
| 1000 | true |  | 99 |
| 10000 | true |  | 863 |
| 10000 |  | true | 1572 |
| 10000 | true | true | 1953 |


## _bulk_get benchmark 
| count| Duration (ms) |
|--|--|
| 100 | 30 |
| 1000 | 82 |
| 10000 | 972 |


## view benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 126167 |
| 100 |  |  | 30 |
| 1000 |  |  | 53 |
| 10000 |  |  | 435 |
| 100 | true |  | 36 |
| 1000 | true |  | 154 |
| 10000 | true |  | 1270 |
| 100 |  | true | 74 |
| 1000 |  | true | 587 |
| 10000 |  | true | 6067 |
| 10000 | true | true | 7143 |


## nouveau_index benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 224373 |
| 100 |  |  | 221 |
| 1000 |  |  | 537 |
| 10000 |  |  | 2793 |
| 100 | true |  | 80 |
| 1000 | true |  | 466 |
| 10000 | true |  | 4205 |
| 100 |  | true | 201 |
| 1000 |  | true | 637 |
| 10000 |  | true | 2829 |
| 10000 | true | true | 4064 |


