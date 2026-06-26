# CouchDb Performance benchmark 

## Database Info

CouchDb version: 3.5.2

Database doc count: 903030

## _changes benchmark 
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 32 |
| 1000 |  |  |  |  | 83 |
| 10000 |  |  |  |  | 633 |
| 100 |  | true |  |  | 34 |
| 1000 |  | true |  |  | 128 |
| 10000 |  | true |  |  | 1007 |
| 100 |  |  | 100 |  | 27 |
| 1000 |  |  | 1000 |  | 29 |
| 10000 |  |  | 10000 |  | 127 |
| 100 | Mid Sequence |  |  |  | 31 |
| 1000 | Mid Sequence |  |  |  | 89 |
| 10000 | Mid Sequence |  |  |  | 604 |
| 100 | Mid Sequence | true |  |  | 33 |
| 1000 | Mid Sequence | true |  |  | 118 |
| 10000 | Mid Sequence | true |  |  | 1039 |
| 100 | Mid Sequence |  | 100 |  | 35 |
| 1000 | Mid Sequence |  | 1000 |  | 29 |
| 10000 | Mid Sequence |  | 10000 |  | 127 |
| 10000 |  |  |  | true | 1473 |
| 10000 |  | true |  | true | 1837 |
| 10000 |  |  | 10000 | true | 983 |


## _all_docs benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 21 |
| 1000 |  |  | 33 |
| 10000 |  |  | 206 |
| 100 | true |  | 27 |
| 1000 | true |  | 76 |
| 10000 | true |  | 630 |
| 10000 |  | true | 988 |
| 10000 | true | true | 1337 |


## _bulk_get benchmark 
| count| Duration (ms) |
|--|--|
| 100 | 29 |
| 1000 | 67 |
| 10000 | 691 |


## view benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 100557 |
| 100 |  |  | 29 |
| 1000 |  |  | 62 |
| 10000 |  |  | 272 |
| 100 | true |  | 36 |
| 1000 | true |  | 135 |
| 10000 | true |  | 961 |
| 100 |  | true | 93 |
| 1000 |  | true | 584 |
| 10000 |  | true | 5494 |
| 10000 | true | true | 5846 |


## nouveau_index benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 69375 |
| 100 |  |  | 110 |
| 1000 |  |  | 241 |
| 10000 |  |  | 1438 |
| 100 | true |  | 69 |
| 1000 | true |  | 310 |
| 10000 | true |  | 2506 |
| 100 |  | true | 160 |
| 1000 |  | true | 398 |
| 10000 |  | true | 1568 |
| 10000 | true | true | 2484 |


