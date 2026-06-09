# CouchDb Performance benchmark 

## Database Info

CouchDb version: 3.5.2

Database doc count: 903030

## _changes benchmark 
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 33 |
| 1000 |  |  |  |  | 75 |
| 10000 |  |  |  |  | 620 |
| 100 |  | true |  |  | 37 |
| 1000 |  | true |  |  | 149 |
| 10000 |  | true |  |  | 2718 |
| 100 |  |  | 100 |  | 27 |
| 1000 |  |  | 1000 |  | 32 |
| 10000 |  |  | 10000 |  | 150 |
| 100 | Mid Sequence |  |  |  | 41 |
| 1000 | Mid Sequence |  |  |  | 499 |
| 10000 | Mid Sequence |  |  |  | 632 |
| 100 | Mid Sequence | true |  |  | 34 |
| 1000 | Mid Sequence | true |  |  | 126 |
| 10000 | Mid Sequence | true |  |  | 1060 |
| 100 | Mid Sequence |  | 100 |  | 37 |
| 1000 | Mid Sequence |  | 1000 |  | 32 |
| 10000 | Mid Sequence |  | 10000 |  | 128 |
| 10000 |  |  |  | true | 1564 |
| 10000 |  | true |  | true | 1881 |
| 10000 |  |  | 10000 | true | 1011 |


## _all_docs benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 36 |
| 1000 |  |  | 37 |
| 10000 |  |  | 224 |
| 100 | true |  | 38 |
| 1000 | true |  | 108 |
| 10000 | true |  | 654 |
| 10000 |  | true | 1015 |
| 10000 | true | true | 1342 |


## _bulk_get benchmark 
| count| Duration (ms) |
|--|--|
| 100 | 26 |
| 1000 | 70 |
| 10000 | 706 |


## view benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 97347 |
| 100 |  |  | 26 |
| 1000 |  |  | 44 |
| 10000 |  |  | 285 |
| 100 | true |  | 35 |
| 1000 | true |  | 146 |
| 10000 | true |  | 986 |
| 100 |  | true | 87 |
| 1000 |  | true | 596 |
| 10000 |  | true | 5748 |
| 10000 | true | true | 6099 |


## nouveau_index benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 72414 |
| 100 |  |  | 123 |
| 1000 |  |  | 239 |
| 10000 |  |  | 1800 |
| 100 | true |  | 91 |
| 1000 | true |  | 303 |
| 10000 | true |  | 2624 |
| 100 |  | true | 152 |
| 1000 |  | true | 350 |
| 10000 |  | true | 1700 |
| 10000 | true | true | 2799 |


