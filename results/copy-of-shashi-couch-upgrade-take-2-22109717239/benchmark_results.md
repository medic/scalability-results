# CouchDb Performance benchmark 

## Database Info

CouchDb version: 3.5.1

Database doc count: 903030

## _changes benchmark 
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 38 |
| 1000 |  |  |  |  | 109 |
| 10000 |  |  |  |  | 734 |
| 100 |  | true |  |  | 44 |
| 1000 |  | true |  |  | 150 |
| 10000 |  | true |  |  | 1069 |
| 100 |  |  | 100 |  | 35 |
| 1000 |  |  | 1000 |  | 36 |
| 10000 |  |  | 10000 |  | 150 |
| 100 | Mid Sequence |  |  |  | 34 |
| 1000 | Mid Sequence |  |  |  | 100 |
| 10000 | Mid Sequence |  |  |  | 688 |
| 100 | Mid Sequence | true |  |  | 40 |
| 1000 | Mid Sequence | true |  |  | 138 |
| 10000 | Mid Sequence | true |  |  | 1100 |
| 100 | Mid Sequence |  | 100 |  | 679 |
| 1000 | Mid Sequence |  | 1000 |  | 967 |
| 10000 | Mid Sequence |  | 10000 |  | 150 |
| 10000 |  |  |  | true | 1640 |
| 10000 |  | true |  | true | 1962 |
| 10000 |  |  | 10000 | true | 973 |


## _all_docs benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 24 |
| 1000 |  |  | 44 |
| 10000 |  |  | 201 |
| 100 | true |  | 268 |
| 1000 | true |  | 84 |
| 10000 | true |  | 2310 |
| 10000 |  | true | 1385 |
| 10000 | true | true | 1679 |


## _bulk_get benchmark 
| count| Duration (ms) |
|--|--|
| 100 | 25 |
| 1000 | 77 |
| 10000 | 1002 |


## view benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 122716 |
| 100 |  |  | 33 |
| 1000 |  |  | 773 |
| 10000 |  |  | 374 |
| 100 | true |  | 40 |
| 1000 | true |  | 132 |
| 10000 | true |  | 1169 |
| 100 |  | true | 89 |
| 1000 |  | true | 577 |
| 10000 |  | true | 5645 |
| 10000 | true | true | 6646 |


## nouveau_index benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 2683576 |
| 100 |  |  | 123 |
| 1000 |  |  | 201 |
| 10000 |  |  | 1251 |
| 100 | true |  | 63 |
| 1000 | true |  | 254 |
| 10000 | true |  | 2360 |
| 100 |  | true | 39 |
| 1000 |  | true | 202 |
| 10000 |  | true | 1615 |
| 10000 | true | true | 2418 |


