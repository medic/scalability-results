# CouchDb Performance benchmark

## Database Info

CouchDb version: 3.5.0

Database doc count: 903030

## _changes benchmark
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 35 |
| 1000 |  |  |  |  | 101 |
| 10000 |  |  |  |  | 683 |
| 100 |  | true |  |  | 39 |
| 1000 |  | true |  |  | 129 |
| 10000 |  | true |  |  | 998 |
| 100 |  |  | 100 |  | 30 |
| 1000 |  |  | 1000 |  | 36 |
| 10000 |  |  | 10000 |  | 129 |
| 100 | Mid Sequence |  |  |  | 33 |
| 1000 | Mid Sequence |  |  |  | 89 |
| 10000 | Mid Sequence |  |  |  | 663 |
| 100 | Mid Sequence | true |  |  | 36 |
| 1000 | Mid Sequence | true |  |  | 127 |
| 10000 | Mid Sequence | true |  |  | 937 |
| 100 | Mid Sequence |  | 100 |  | 31 |
| 1000 | Mid Sequence |  | 1000 |  | 35 |
| 10000 | Mid Sequence |  | 10000 |  | 128 |
| 10000 |  |  |  | true | 1106 |
| 10000 |  | true |  | true | 1392 |
| 10000 |  |  | 10000 | true | 668 |


## _all_docs benchmark
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 28 |
| 1000 |  |  | 38 |
| 10000 |  |  | 180 |
| 100 | true |  | 30 |
| 1000 | true |  | 71 |
| 10000 | true |  | 467 |
| 10000 |  | true | 794 |
| 10000 | true | true | 1051 |


## _bulk_get benchmark
| count| Duration (ms) |
|--|--|
| 100 | 30 |
| 1000 | 75 |
| 10000 | 668 |


## view benchmark
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 57681 |
| 100 |  |  | 26 |
| 1000 |  |  | 46 |
| 10000 |  |  | 249 |
| 100 | true |  | 34 |
| 1000 | true |  | 109 |
| 10000 | true |  | 762 |
| 100 |  | true | 67 |
| 1000 |  | true | 399 |
| 10000 |  | true | 3556 |
| 10000 | true | true | 3858 |


## nouveau_index benchmark
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 133628 |
| 100 |  |  | 132 |
| 1000 |  |  | 227 |
| 10000 |  |  | 1087 |
| 100 | true |  | 63 |
| 1000 | true |  | 228 |
| 10000 | true |  | 1977 |
| 100 |  | true | 130 |
| 1000 |  | true | 367 |
| 10000 |  | true | 1821 |
| 10000 | true | true | 2529 |
