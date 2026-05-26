# CouchDb Performance benchmark 

## Database Info

CouchDb version: 3.5.0

Database doc count: 903030

## _changes benchmark 
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 53 |
| 1000 |  |  |  |  | 132 |
| 10000 |  |  |  |  | 1008 |
| 100 |  | true |  |  | 45 |
| 1000 |  | true |  |  | 166 |
| 10000 |  | true |  |  | 1638 |
| 100 |  |  | 100 |  | 33 |
| 1000 |  |  | 1000 |  | 38 |
| 10000 |  |  | 10000 |  | 195 |
| 100 | Mid Sequence |  |  |  | 34 |
| 1000 | Mid Sequence |  |  |  | 124 |
| 10000 | Mid Sequence |  |  |  | 911 |
| 100 | Mid Sequence | true |  |  | 46 |
| 1000 | Mid Sequence | true |  |  | 191 |
| 10000 | Mid Sequence | true |  |  | 1647 |
| 100 | Mid Sequence |  | 100 |  | 41 |
| 1000 | Mid Sequence |  | 1000 |  | 39 |
| 10000 | Mid Sequence |  | 10000 |  | 171 |
| 10000 |  |  |  | true | 1973 |
| 10000 |  | true |  | true | 2484 |
| 10000 |  |  | 10000 | true | 1202 |


## _all_docs benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 47 |
| 1000 |  |  | 55 |
| 10000 |  |  | 321 |
| 100 | true |  | 34 |
| 1000 | true |  | 100 |
| 10000 | true |  | 887 |
| 10000 |  | true | 1705 |
| 10000 | true | true | 2257 |


## _bulk_get benchmark 
| count| Duration (ms) |
|--|--|
| 100 | 40 |
| 1000 | 122 |
| 10000 | 1181 |


## view benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 132618 |
| 100 |  |  | 35 |
| 1000 |  |  | 64 |
| 10000 |  |  | 527 |
| 100 | true |  | 43 |
| 1000 | true |  | 137 |
| 10000 | true |  | 1338 |
| 100 |  | true | 92 |
| 1000 |  | true | 676 |
| 10000 |  | true | 6358 |
| 10000 | true | true | 7036 |


## nouveau_index benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 246934 |
| 100 |  |  | 192 |
| 1000 |  |  | 447 |
| 10000 |  |  | 2936 |
| 100 | true |  | 81 |
| 1000 | true |  | 525 |
| 10000 | true |  | 4453 |
| 100 |  | true | 164 |
| 1000 |  | true | 972 |
| 10000 |  | true | 2902 |
| 10000 | true | true | 4422 |


