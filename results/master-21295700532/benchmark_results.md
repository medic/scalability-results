# CouchDb Performance benchmark 

## Database Info

CouchDb version: 3.5.0

Database doc count: 903030

## _changes benchmark 
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 31 |
| 1000 |  |  |  |  | 101 |
| 10000 |  |  |  |  | 624 |
| 100 |  | true |  |  | 38 |
| 1000 |  | true |  |  | 128 |
| 10000 |  | true |  |  | 1024 |
| 100 |  |  | 100 |  | 32 |
| 1000 |  |  | 1000 |  | 33 |
| 10000 |  |  | 10000 |  | 129 |
| 100 | Mid Sequence |  |  |  | 33 |
| 1000 | Mid Sequence |  |  |  | 94 |
| 10000 | Mid Sequence |  |  |  | 1255 |
| 100 | Mid Sequence | true |  |  | 35 |
| 1000 | Mid Sequence | true |  |  | 119 |
| 10000 | Mid Sequence | true |  |  | 1002 |
| 100 | Mid Sequence |  | 100 |  | 27 |
| 1000 | Mid Sequence |  | 1000 |  | 33 |
| 10000 | Mid Sequence |  | 10000 |  | 129 |
| 10000 |  |  |  | true | 1936 |
| 10000 |  | true |  | true | 2575 |
| 10000 |  |  | 10000 | true | 1002 |


## _all_docs benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 23 |
| 1000 |  |  | 36 |
| 10000 |  |  | 194 |
| 100 | true |  | 30 |
| 1000 | true |  | 78 |
| 10000 | true |  | 578 |
| 10000 |  | true | 1200 |
| 10000 | true | true | 1564 |


## _bulk_get benchmark 
| count| Duration (ms) |
|--|--|
| 100 | 30 |
| 1000 | 86 |
| 10000 | 771 |


## view benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 29 |
| 1000 |  |  | 50 |
| 10000 |  |  | 257 |
| 100 | true |  | 41 |
| 1000 | true |  | 297 |
| 10000 | true |  | 1155 |
| 100 |  | true | 89 |
| 1000 |  | true | 594 |
| 10000 |  | true | 5703 |
| 10000 | true | true | 6303 |


## nouveau_index benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 127 |
| 1000 |  |  | 298 |
| 10000 |  |  | 2065 |
| 100 | true |  | 99 |
| 1000 | true |  | 354 |
| 10000 | true |  | 3230 |
| 100 |  | true | 45 |
| 1000 |  | true | 258 |
| 10000 |  | true | 1887 |
| 10000 | true | true | 3547 |


