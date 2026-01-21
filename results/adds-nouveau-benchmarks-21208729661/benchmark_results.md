# CouchDb Performance benchmark 

## Database Info

CouchDb version: 3.5.0

Database doc count: 903030

## _changes benchmark 
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 40 |
| 1000 |  |  |  |  | 104 |
| 10000 |  |  |  |  | 646 |
| 100 |  | true |  |  | 41 |
| 1000 |  | true |  |  | 129 |
| 10000 |  | true |  |  | 957 |
| 100 |  |  | 100 |  | 35 |
| 1000 |  |  | 1000 |  | 38 |
| 10000 |  |  | 10000 |  | 134 |
| 100 | Mid Sequence |  |  |  | 36 |
| 1000 | Mid Sequence |  |  |  | 542 |
| 10000 | Mid Sequence |  |  |  | 629 |
| 100 | Mid Sequence | true |  |  | 41 |
| 1000 | Mid Sequence | true |  |  | 142 |
| 10000 | Mid Sequence | true |  |  | 1250 |
| 100 | Mid Sequence |  | 100 |  | 126 |
| 1000 | Mid Sequence |  | 1000 |  | 38 |
| 10000 | Mid Sequence |  | 10000 |  | 136 |
| 10000 |  |  |  | true | 1463 |
| 10000 |  | true |  | true | 1887 |
| 10000 |  |  | 10000 | true | 1033 |


## _all_docs benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 28 |
| 1000 |  |  | 42 |
| 10000 |  |  | 205 |
| 100 | true |  | 36 |
| 1000 | true |  | 96 |
| 10000 | true |  | 601 |
| 10000 |  | true | 1249 |
| 10000 | true | true | 1522 |


## _bulk_get benchmark 
| count| Duration (ms) |
|--|--|
| 100 | 31 |
| 1000 | 78 |
| 10000 | 742 |


## view benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 44 |
| 1000 |  |  | 51 |
| 10000 |  |  | 285 |
| 100 | true |  | 43 |
| 1000 | true |  | 166 |
| 10000 | true |  | 1398 |
| 100 |  | true | 5693 |
| 1000 |  | true | 7213 |
| 10000 |  | true | 5995 |
| 10000 | true | true | 6184 |


## nouveau_index benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 262 |
| 1000 |  |  | 330 |
| 10000 |  |  | 2219 |
| 100 | true |  | 86 |
| 1000 | true |  | 372 |
| 10000 | true |  | 3304 |
| 100 |  | true | 59 |
| 1000 |  | true | 271 |
| 10000 |  | true | 1774 |
| 10000 | true | true | 3300 |


