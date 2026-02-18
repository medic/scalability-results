# CouchDb Performance benchmark 

## Database Info

CouchDb version: 3.5.1

Database doc count: 903030

## _changes benchmark 
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 37 |
| 1000 |  |  |  |  | 28712 |
| 10000 |  |  |  |  | 71938 |
| 100 |  | true |  |  | 44 |
| 1000 |  | true |  |  | 148 |
| 10000 |  | true |  |  | 1089 |
| 100 |  |  | 100 |  | 31 |
| 1000 |  |  | 1000 |  | 45 |
| 10000 |  |  | 10000 |  | 154 |
| 100 | Mid Sequence |  |  |  | 43 |
| 1000 | Mid Sequence |  |  |  | 104 |
| 10000 | Mid Sequence |  |  |  | 682 |
| 100 | Mid Sequence | true |  |  | 63 |
| 1000 | Mid Sequence | true |  |  | 173 |
| 10000 | Mid Sequence | true |  |  | 1074 |
| 100 | Mid Sequence |  | 100 |  | 28 |
| 1000 | Mid Sequence |  | 1000 |  | 35 |
| 10000 | Mid Sequence |  | 10000 |  | 147 |
| 10000 |  |  |  | true | 1516 |
| 10000 |  | true |  | true | 2568 |
| 10000 |  |  | 10000 | true | 1024 |


## _all_docs benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 25 |
| 1000 |  |  | 40 |
| 10000 |  |  | 214 |
| 100 | true |  | 30 |
| 1000 | true |  | 83 |
| 10000 | true |  | 667 |
| 10000 |  | true | 1076 |
| 10000 | true | true | 1333 |


## _bulk_get benchmark 
| count| Duration (ms) |
|--|--|
| 100 | 28 |
| 1000 | 74 |
| 10000 | 730 |


## view benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 122447 |
| 100 |  |  | 30 |
| 1000 |  |  | 64 |
| 10000 |  |  | 7758 |
| 100 | true |  | 46 |
| 1000 | true |  | 179 |
| 10000 | true |  | 1082 |
| 100 |  | true | 97 |
| 1000 |  | true | 621 |
| 10000 |  | true | 5812 |
| 10000 | true | true | 6156 |


## nouveau_index benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 3190949 |
| 100 |  |  | 90 |
| 1000 |  |  | 215 |
| 10000 |  |  | 1263 |
| 100 | true |  | 103 |
| 1000 | true |  | 325 |
| 10000 | true |  | 2450 |
| 100 |  | true | 53 |
| 1000 |  | true | 238 |
| 10000 |  | true | 1749 |
| 10000 | true | true | 2759 |


