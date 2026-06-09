# CouchDb Performance benchmark 

## Database Info

CouchDb version: 3.5.2

Database doc count: 903030

## _changes benchmark 
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 27 |
| 1000 |  |  |  |  | 88 |
| 10000 |  |  |  |  | 682 |
| 100 |  | true |  |  | 34 |
| 1000 |  | true |  |  | 157 |
| 10000 |  | true |  |  | 1043 |
| 100 |  |  | 100 |  | 27 |
| 1000 |  |  | 1000 |  | 29 |
| 10000 |  |  | 10000 |  | 133 |
| 100 | Mid Sequence |  |  |  | 28 |
| 1000 | Mid Sequence |  |  |  | 84 |
| 10000 | Mid Sequence |  |  |  | 689 |
| 100 | Mid Sequence | true |  |  | 33 |
| 1000 | Mid Sequence | true |  |  | 134 |
| 10000 | Mid Sequence | true |  |  | 1057 |
| 100 | Mid Sequence |  | 100 |  | 29 |
| 1000 | Mid Sequence |  | 1000 |  | 31 |
| 10000 | Mid Sequence |  | 10000 |  | 159 |
| 10000 |  |  |  | true | 1533 |
| 10000 |  | true |  | true | 1939 |
| 10000 |  |  | 10000 | true | 973 |


## _all_docs benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 20 |
| 1000 |  |  | 36 |
| 10000 |  |  | 190 |
| 100 | true |  | 24 |
| 1000 | true |  | 85 |
| 10000 | true |  | 626 |
| 10000 |  | true | 1054 |
| 10000 | true | true | 1321 |


## _bulk_get benchmark 
| count| Duration (ms) |
|--|--|
| 100 | 30 |
| 1000 | 76 |
| 10000 | 753 |


## view benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 104357 |
| 100 |  |  | 25 |
| 1000 |  |  | 44 |
| 10000 |  |  | 273 |
| 100 | true |  | 32 |
| 1000 | true |  | 107 |
| 10000 | true |  | 999 |
| 100 |  | true | 84 |
| 1000 |  | true | 604 |
| 10000 |  | true | 5670 |
| 10000 | true | true | 5812 |


## nouveau_index benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 71940 |
| 100 |  |  | 160 |
| 1000 |  |  | 233 |
| 10000 |  |  | 1531 |
| 100 | true |  | 2592 |
| 1000 | true |  | 319 |
| 10000 | true |  | 2511 |
| 100 |  | true | 182 |
| 1000 |  | true | 394 |
| 10000 |  | true | 1745 |
| 10000 | true | true | 2419 |


