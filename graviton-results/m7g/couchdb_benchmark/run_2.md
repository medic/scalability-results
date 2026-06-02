# CouchDb Performance benchmark

## Database Info

CouchDb version: 3.5.0

Database doc count: 903030

## _changes benchmark
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 35 |
| 1000 |  |  |  |  | 93 |
| 10000 |  |  |  |  | 715 |
| 100 |  | true |  |  | 48 |
| 1000 |  | true |  |  | 125 |
| 10000 |  | true |  |  | 986 |
| 100 |  |  | 100 |  | 31 |
| 1000 |  |  | 1000 |  | 37 |
| 10000 |  |  | 10000 |  | 131 |
| 100 | Mid Sequence |  |  |  | 34 |
| 1000 | Mid Sequence |  |  |  | 92 |
| 10000 | Mid Sequence |  |  |  | 637 |
| 100 | Mid Sequence | true |  |  | 45 |
| 1000 | Mid Sequence | true |  |  | 126 |
| 10000 | Mid Sequence | true |  |  | 933 |
| 100 | Mid Sequence |  | 100 |  | 33 |
| 1000 | Mid Sequence |  | 1000 |  | 36 |
| 10000 | Mid Sequence |  | 10000 |  | 129 |
| 10000 |  |  |  | true | 1128 |
| 10000 |  | true |  | true | 1385 |
| 10000 |  |  | 10000 | true | 652 |


## _all_docs benchmark
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 25 |
| 1000 |  |  | 40 |
| 10000 |  |  | 189 |
| 100 | true |  | 30 |
| 1000 | true |  | 73 |
| 10000 | true |  | 455 |
| 10000 |  | true | 810 |
| 10000 | true | true | 1079 |


## _bulk_get benchmark
| count| Duration (ms) |
|--|--|
| 100 | 28 |
| 1000 | 73 |
| 10000 | 664 |


## view benchmark
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 58151 |
| 100 |  |  | 27 |
| 1000 |  |  | 48 |
| 10000 |  |  | 247 |
| 100 | true |  | 36 |
| 1000 | true |  | 101 |
| 10000 | true |  | 759 |
| 100 |  | true | 65 |
| 1000 |  | true | 395 |
| 10000 |  | true | 3553 |
| 10000 | true | true | 3909 |


## nouveau_index benchmark
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 130397 |
| 100 |  |  | 69 |
| 1000 |  |  | 125 |
| 10000 |  |  | 967 |
| 100 | true |  | 59 |
| 1000 | true |  | 230 |
| 10000 | true |  | 2199 |
| 100 |  | true | 53 |
| 1000 |  | true | 159 |
| 10000 |  | true | 1518 |
| 10000 | true | true | 2514 |

