# CouchDb Performance benchmark 

## Database Info

CouchDb version: 3.5.0

Database doc count: 903030

## _changes benchmark 
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 35 |
| 1000 |  |  |  |  | 123 |
| 10000 |  |  |  |  | 948 |
| 100 |  | true |  |  | 69 |
| 1000 |  | true |  |  | 159 |
| 10000 |  | true |  |  | 1523 |
| 100 |  |  | 100 |  | 32 |
| 1000 |  |  | 1000 |  | 45 |
| 10000 |  |  | 10000 |  | 306 |
| 100 | Mid Sequence |  |  |  | 33 |
| 1000 | Mid Sequence |  |  |  | 126 |
| 10000 | Mid Sequence |  |  |  | 1170 |
| 100 | Mid Sequence | true |  |  | 59 |
| 1000 | Mid Sequence | true |  |  | 164 |
| 10000 | Mid Sequence | true |  |  | 1891 |
| 100 | Mid Sequence |  | 100 |  | 36 |
| 1000 | Mid Sequence |  | 1000 |  | 42 |
| 10000 | Mid Sequence |  | 10000 |  | 202 |
| 10000 |  |  |  | true | 2124 |
| 10000 |  | true |  | true | 2852 |
| 10000 |  |  | 10000 | true | 1311 |


## _all_docs benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 49 |
| 1000 |  |  | 52 |
| 10000 |  |  | 377 |
| 100 | true |  | 65 |
| 1000 | true |  | 91 |
| 10000 | true |  | 949 |
| 10000 |  | true | 1737 |
| 10000 | true | true | 2094 |


## _bulk_get benchmark 
| count| Duration (ms) |
|--|--|
| 100 | 38 |
| 1000 | 110 |
| 10000 | 1046 |


## view benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 126866 |
| 100 |  |  | 28 |
| 1000 |  |  | 53 |
| 10000 |  |  | 340 |
| 100 | true |  | 40 |
| 1000 | true |  | 125 |
| 10000 | true |  | 1411 |
| 100 |  | true | 92 |
| 1000 |  | true | 615 |
| 10000 |  | true | 5987 |
| 10000 | true | true | 7053 |


## nouveau_index benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 239384 |
| 100 |  |  | 224 |
| 1000 |  |  | 467 |
| 10000 |  |  | 3318 |
| 100 | true |  | 101 |
| 1000 | true |  | 532 |
| 10000 | true |  | 4641 |
| 100 |  | true | 217 |
| 1000 |  | true | 575 |
| 10000 |  | true | 3011 |
| 10000 | true | true | 4298 |


