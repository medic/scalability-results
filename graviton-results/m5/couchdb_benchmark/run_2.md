# CouchDb Performance benchmark

## Database Info

CouchDb version: 3.5.0

Database doc count: 903030

## _changes benchmark
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 36 |
| 1000 |  |  |  |  | 107 |
| 10000 |  |  |  |  | 845 |
| 100 |  | true |  |  | 64 |
| 1000 |  | true |  |  | 167 |
| 10000 |  | true |  |  | 1231 |
| 100 |  |  | 100 |  | 31 |
| 1000 |  |  | 1000 |  | 41 |
| 10000 |  |  | 10000 |  | 166 |
| 100 | Mid Sequence |  |  |  | 34 |
| 1000 | Mid Sequence |  |  |  | 129 |
| 10000 | Mid Sequence |  |  |  | 811 |
| 100 | Mid Sequence | true |  |  | 41 |
| 1000 | Mid Sequence | true |  |  | 160 |
| 10000 | Mid Sequence | true |  |  | 1235 |
| 100 | Mid Sequence |  | 100 |  | 33 |
| 1000 | Mid Sequence |  | 1000 |  | 39 |
| 10000 | Mid Sequence |  | 10000 |  | 167 |
| 10000 |  |  |  | true | 1545 |
| 10000 |  | true |  | true | 2217 |
| 10000 |  |  | 10000 | true | 1059 |


## _all_docs benchmark
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 24 |
| 1000 |  |  | 42 |
| 10000 |  |  | 235 |
| 100 | true |  | 31 |
| 1000 | true |  | 93 |
| 10000 | true |  | 684 |
| 10000 |  | true | 1267 |
| 10000 | true | true | 1611 |


## _bulk_get benchmark
| count| Duration (ms) |
|--|--|
| 100 | 30 |
| 1000 | 81 |
| 10000 | 818 |


## view benchmark
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 100871 |
| 100 |  |  | 33 |
| 1000 |  |  | 57 |
| 10000 |  |  | 318 |
| 100 | true |  | 44 |
| 1000 | true |  | 147 |
| 10000 | true |  | 1129 |
| 100 |  | true | 94 |
| 1000 |  | true | 584 |
| 10000 |  | true | 5542 |
| 10000 | true | true | 5980 |


## nouveau_index benchmark
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 192011 |
| 100 |  |  | 101 |
| 1000 |  |  | 301 |
| 10000 |  |  | 2176 |
| 100 | true |  | 83 |
| 1000 | true |  | 423 |
| 10000 | true |  | 3741 |
| 100 |  | true | 55 |
| 1000 |  | true | 243 |
| 10000 |  | true | 1922 |
| 10000 | true | true | 3495 |

