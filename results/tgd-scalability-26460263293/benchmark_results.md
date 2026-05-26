# CouchDb Performance benchmark 

## Database Info

CouchDb version: 3.5.0

Database doc count: 903030

## _changes benchmark 
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 38 |
| 1000 |  |  |  |  | 154 |
| 10000 |  |  |  |  | 1096 |
| 100 |  | true |  |  | 60 |
| 1000 |  | true |  |  | 169 |
| 10000 |  | true |  |  | 1709 |
| 100 |  |  | 100 |  | 37 |
| 1000 |  |  | 1000 |  | 38 |
| 10000 |  |  | 10000 |  | 204 |
| 100 | Mid Sequence |  |  |  | 33 |
| 1000 | Mid Sequence |  |  |  | 117 |
| 10000 | Mid Sequence |  |  |  | 1024 |
| 100 | Mid Sequence | true |  |  | 65 |
| 1000 | Mid Sequence | true |  |  | 170 |
| 10000 | Mid Sequence | true |  |  | 1621 |
| 100 | Mid Sequence |  | 100 |  | 41 |
| 1000 | Mid Sequence |  | 1000 |  | 42 |
| 10000 | Mid Sequence |  | 10000 |  | 242 |
| 10000 |  |  |  | true | 2158 |
| 10000 |  | true |  | true | 2468 |
| 10000 |  |  | 10000 | true | 1190 |


## _all_docs benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 49 |
| 1000 |  |  | 63 |
| 10000 |  |  | 275 |
| 100 | true |  | 37 |
| 1000 | true |  | 103 |
| 10000 | true |  | 961 |
| 10000 |  | true | 1780 |
| 10000 | true | true | 2212 |


## _bulk_get benchmark 
| count| Duration (ms) |
|--|--|
| 100 | 31 |
| 1000 | 87 |
| 10000 | 1135 |


## view benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 127167 |
| 100 |  |  | 30 |
| 1000 |  |  | 47 |
| 10000 |  |  | 346 |
| 100 | true |  | 42 |
| 1000 | true |  | 134 |
| 10000 | true |  | 1247 |
| 100 |  | true | 82 |
| 1000 |  | true | 587 |
| 10000 |  | true | 6179 |
| 10000 | true | true | 6989 |


## nouveau_index benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 235644 |
| 100 |  |  | 187 |
| 1000 |  |  | 535 |
| 10000 |  |  | 3031 |
| 100 | true |  | 81 |
| 1000 | true |  | 511 |
| 10000 | true |  | 4619 |
| 100 |  | true | 193 |
| 1000 |  | true | 1071 |
| 10000 |  | true | 3007 |
| 10000 | true | true | 4242 |


