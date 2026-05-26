# CouchDb Performance benchmark 

## Database Info

CouchDb version: 3.5.0

Database doc count: 903030

## _changes benchmark 
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 38 |
| 1000 |  |  |  |  | 145 |
| 10000 |  |  |  |  | 995 |
| 100 |  | true |  |  | 45 |
| 1000 |  | true |  |  | 193 |
| 10000 |  | true |  |  | 1669 |
| 100 |  |  | 100 |  | 34 |
| 1000 |  |  | 1000 |  | 44 |
| 10000 |  |  | 10000 |  | 217 |
| 100 | Mid Sequence |  |  |  | 42 |
| 1000 | Mid Sequence |  |  |  | 137 |
| 10000 | Mid Sequence |  |  |  | 1153 |
| 100 | Mid Sequence | true |  |  | 38 |
| 1000 | Mid Sequence | true |  |  | 206 |
| 10000 | Mid Sequence | true |  |  | 1538 |
| 100 | Mid Sequence |  | 100 |  | 37 |
| 1000 | Mid Sequence |  | 1000 |  | 65 |
| 10000 | Mid Sequence |  | 10000 |  | 218 |
| 10000 |  |  |  | true | 1828 |
| 10000 |  | true |  | true | 2491 |
| 10000 |  |  | 10000 | true | 1149 |


## _all_docs benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 39 |
| 1000 |  |  | 54 |
| 10000 |  |  | 285 |
| 100 | true |  | 30 |
| 1000 | true |  | 108 |
| 10000 | true |  | 867 |
| 10000 |  | true | 1647 |
| 10000 | true | true | 2066 |


## _bulk_get benchmark 
| count| Duration (ms) |
|--|--|
| 100 | 30 |
| 1000 | 85 |
| 10000 | 982 |


## view benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 127294 |
| 100 |  |  | 34 |
| 1000 |  |  | 81 |
| 10000 |  |  | 419 |
| 100 | true |  | 44 |
| 1000 | true |  | 139 |
| 10000 | true |  | 5263 |
| 100 |  | true | 75 |
| 1000 |  | true | 604 |
| 10000 |  | true | 6140 |
| 10000 | true | true | 7452 |


## nouveau_index benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 233632 |
| 100 |  |  | 175 |
| 1000 |  |  | 555 |
| 10000 |  |  | 3129 |
| 100 | true |  | 94 |
| 1000 | true |  | 577 |
| 10000 | true |  | 4641 |
| 100 |  | true | 158 |
| 1000 |  | true | 724 |
| 10000 |  | true | 3082 |
| 10000 | true | true | 4198 |


