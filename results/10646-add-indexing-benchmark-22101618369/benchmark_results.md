# CouchDb Performance benchmark 

## Database Info

CouchDb version: 3.5.0

Database doc count: 903030

## _changes benchmark 
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 43 |
| 1000 |  |  |  |  | 103 |
| 10000 |  |  |  |  | 660 |
| 100 |  | true |  |  | 60 |
| 1000 |  | true |  |  | 138 |
| 10000 |  | true |  |  | 1016 |
| 100 |  |  | 100 |  | 44 |
| 1000 |  |  | 1000 |  | 32 |
| 10000 |  |  | 10000 |  | 145 |
| 100 | Mid Sequence |  |  |  | 32 |
| 1000 | Mid Sequence |  |  |  | 90 |
| 10000 | Mid Sequence |  |  |  | 665 |
| 100 | Mid Sequence | true |  |  | 36 |
| 1000 | Mid Sequence | true |  |  | 139 |
| 10000 | Mid Sequence | true |  |  | 1036 |
| 100 | Mid Sequence |  | 100 |  | 42 |
| 1000 | Mid Sequence |  | 1000 |  | 58 |
| 10000 | Mid Sequence |  | 10000 |  | 150 |
| 10000 |  |  |  | true | 1452 |
| 10000 |  | true |  | true | 1982 |
| 10000 |  |  | 10000 | true | 1002 |


## _all_docs benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 39 |
| 1000 |  |  | 41 |
| 10000 |  |  | 226 |
| 100 | true |  | 36 |
| 1000 | true |  | 84 |
| 10000 | true |  | 633 |
| 10000 |  | true | 1244 |
| 10000 | true | true | 1607 |


## _bulk_get benchmark 
| count| Duration (ms) |
|--|--|
| 100 | 27 |
| 1000 | 74 |
| 10000 | 768 |


## view benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 118731.350644 |
| 100 |  |  | 35 |
| 1000 |  |  | 47 |
| 10000 |  |  | 288 |
| 100 | true |  | 50 |
| 1000 | true |  | 156 |
| 10000 | true |  | 1194 |
| 100 |  | true | 86 |
| 1000 |  | true | 576 |
| 10000 |  | true | 5572 |
| 10000 | true | true | 6167 |


## nouveau_index benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 184828.358692 |
| 100 |  |  | 142 |
| 1000 |  |  | 301 |
| 10000 |  |  | 2138 |
| 100 | true |  | 82 |
| 1000 | true |  | 344 |
| 10000 | true |  | 3344 |
| 100 |  | true | 72 |
| 1000 |  | true | 282 |
| 10000 |  | true | 1720 |
| 10000 | true | true | 2987 |


