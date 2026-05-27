# CouchDb Performance benchmark 

## Database Info

CouchDb version: 3.5.0

Database doc count: 903030

## _changes benchmark 
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 44 |
| 1000 |  |  |  |  | 141 |
| 10000 |  |  |  |  | 1029 |
| 100 |  | true |  |  | 54 |
| 1000 |  | true |  |  | 169 |
| 10000 |  | true |  |  | 1417 |
| 100 |  |  | 100 |  | 35 |
| 1000 |  |  | 1000 |  | 46 |
| 10000 |  |  | 10000 |  | 196 |
| 100 | Mid Sequence |  |  |  | 33 |
| 1000 | Mid Sequence |  |  |  | 114 |
| 10000 | Mid Sequence |  |  |  | 974 |
| 100 | Mid Sequence | true |  |  | 83 |
| 1000 | Mid Sequence | true |  |  | 166 |
| 10000 | Mid Sequence | true |  |  | 1557 |
| 100 | Mid Sequence |  | 100 |  | 39 |
| 1000 | Mid Sequence |  | 1000 |  | 40 |
| 10000 | Mid Sequence |  | 10000 |  | 176 |
| 10000 |  |  |  | true | 1867 |
| 10000 |  | true |  | true | 2419 |
| 10000 |  |  | 10000 | true | 1132 |


## _all_docs benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 25 |
| 1000 |  |  | 41 |
| 10000 |  |  | 279 |
| 100 | true |  | 34 |
| 1000 | true |  | 98 |
| 10000 | true |  | 852 |
| 10000 |  | true | 1616 |
| 10000 | true | true | 2070 |


## _bulk_get benchmark 
| count| Duration (ms) |
|--|--|
| 100 | 34 |
| 1000 | 89 |
| 10000 | 1037 |


## view benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 128289 |
| 100 |  |  | 29 |
| 1000 |  |  | 53 |
| 10000 |  |  | 334 |
| 100 | true |  | 55 |
| 1000 | true |  | 122 |
| 10000 | true |  | 1067 |
| 100 |  | true | 105 |
| 1000 |  | true | 702 |
| 10000 |  | true | 6341 |
| 10000 | true | true | 7171 |


## nouveau_index benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 234527 |
| 100 |  |  | 112 |
| 1000 |  |  | 430 |
| 10000 |  |  | 2781 |
| 100 | true |  | 89 |
| 1000 | true |  | 452 |
| 10000 | true |  | 4353 |
| 100 |  | true | 55 |
| 1000 |  | true | 390 |
| 10000 |  | true | 2581 |
| 10000 | true | true | 4182 |


