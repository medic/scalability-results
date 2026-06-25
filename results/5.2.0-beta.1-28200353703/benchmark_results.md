# CouchDb Performance benchmark 

## Database Info

CouchDb version: 3.5.2

Database doc count: 903030

## _changes benchmark 
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 31 |
| 1000 |  |  |  |  | 99 |
| 10000 |  |  |  |  | 2766 |
| 100 |  | true |  |  | 33 |
| 1000 |  | true |  |  | 132 |
| 10000 |  | true |  |  | 2263 |
| 100 |  |  | 100 |  | 101 |
| 1000 |  |  | 1000 |  | 42 |
| 10000 |  |  | 10000 |  | 156 |
| 100 | Mid Sequence |  |  |  | 31 |
| 1000 | Mid Sequence |  |  |  | 130 |
| 10000 | Mid Sequence |  |  |  | 660 |
| 100 | Mid Sequence | true |  |  | 32 |
| 1000 | Mid Sequence | true |  |  | 2485 |
| 10000 | Mid Sequence | true |  |  | 995 |
| 100 | Mid Sequence |  | 100 |  | 33 |
| 1000 | Mid Sequence |  | 1000 |  | 30 |
| 10000 | Mid Sequence |  | 10000 |  | 126 |
| 10000 |  |  |  | true | 1473 |
| 10000 |  | true |  | true | 1912 |
| 10000 |  |  | 10000 | true | 959 |


## _all_docs benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 20 |
| 1000 |  |  | 35 |
| 10000 |  |  | 206 |
| 100 | true |  | 25 |
| 1000 | true |  | 90 |
| 10000 | true |  | 618 |
| 10000 |  | true | 990 |
| 10000 | true | true | 1301 |


## _bulk_get benchmark 
| count| Duration (ms) |
|--|--|
| 100 | 30 |
| 1000 | 67 |
| 10000 | 722 |


## view benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 102235 |
| 100 |  |  | 27 |
| 1000 |  |  | 45 |
| 10000 |  |  | 275 |
| 100 | true |  | 34 |
| 1000 | true |  | 140 |
| 10000 | true |  | 981 |
| 100 |  | true | 81 |
| 1000 |  | true | 585 |
| 10000 |  | true | 5591 |
| 10000 | true | true | 5999 |


## nouveau_index benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 69001 |
| 100 |  |  | 121 |
| 1000 |  |  | 239 |
| 10000 |  |  | 1547 |
| 100 | true |  | 67 |
| 1000 | true |  | 348 |
| 10000 | true |  | 2523 |
| 100 |  | true | 163 |
| 1000 |  | true | 289 |
| 10000 |  | true | 1910 |
| 10000 | true | true | 2518 |


