# CouchDb Performance benchmark

## Database Info

CouchDb version: 3.5.0

Database doc count: 903030

## _changes benchmark
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 36 |
| 1000 |  |  |  |  | 198 |
| 10000 |  |  |  |  | 1167 |
| 100 |  | true |  |  | 59 |
| 1000 |  | true |  |  | 169 |
| 10000 |  | true |  |  | 1265 |
| 100 |  |  | 100 |  | 33 |
| 1000 |  |  | 1000 |  | 41 |
| 10000 |  |  | 10000 |  | 180 |
| 100 | Mid Sequence |  |  |  | 38 |
| 1000 | Mid Sequence |  |  |  | 112 |
| 10000 | Mid Sequence |  |  |  | 767 |
| 100 | Mid Sequence | true |  |  | 39 |
| 1000 | Mid Sequence | true |  |  | 163 |
| 10000 | Mid Sequence | true |  |  | 1268 |
| 100 | Mid Sequence |  | 100 |  | 33 |
| 1000 | Mid Sequence |  | 1000 |  | 39 |
| 10000 | Mid Sequence |  | 10000 |  | 172 |
| 10000 |  |  |  | true | 1556 |
| 10000 |  | true |  | true | 2231 |
| 10000 |  |  | 10000 | true | 1058 |


## _all_docs benchmark
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 26 |
| 1000 |  |  | 43 |
| 10000 |  |  | 219 |
| 100 | true |  | 32 |
| 1000 | true |  | 96 |
| 10000 | true |  | 702 |
| 10000 |  | true | 1287 |
| 10000 | true | true | 1654 |


## _bulk_get benchmark
| count| Duration (ms) |
|--|--|
| 100 | 34 |
| 1000 | 85 |
| 10000 | 789 |


## view benchmark
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 102297 |
| 100 |  |  | 28 |
| 1000 |  |  | 47 |
| 10000 |  |  | 300 |
| 100 | true |  | 40 |
| 1000 | true |  | 154 |
| 10000 | true |  | 1133 |
| 100 |  | true | 87 |
| 1000 |  | true | 583 |
| 10000 |  | true | 5475 |
| 10000 | true | true | 6043 |


## nouveau_index benchmark
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 198295 |
| 100 |  |  | 266 |
| 1000 |  |  | 655 |
| 10000 |  |  | 2664 |
| 100 | true |  | 99 |
| 1000 | true |  | 466 |
| 10000 | true |  | 3671 |
| 100 |  | true | 182 |
| 1000 |  | true | 765 |
| 10000 |  | true | 2847 |
| 10000 | true | true | 3494 |


