# CouchDb Performance benchmark

## Database Info

CouchDb version: 3.5.0

Database doc count: 903030

## _changes benchmark
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 44 |
| 1000 |  |  |  |  | 122 |
| 10000 |  |  |  |  | 1048 |
| 100 |  | true |  |  | 46 |
| 1000 |  | true |  |  | 177 |
| 10000 |  | true |  |  | 1274 |
| 100 |  |  | 100 |  | 37 |
| 1000 |  |  | 1000 |  | 46 |
| 10000 |  |  | 10000 |  | 168 |
| 100 | Mid Sequence |  |  |  | 40 |
| 1000 | Mid Sequence |  |  |  | 123 |
| 10000 | Mid Sequence |  |  |  | 837 |
| 100 | Mid Sequence | true |  |  | 45 |
| 1000 | Mid Sequence | true |  |  | 162 |
| 10000 | Mid Sequence | true |  |  | 1237 |
| 100 | Mid Sequence |  | 100 |  | 37 |
| 1000 | Mid Sequence |  | 1000 |  | 45 |
| 10000 | Mid Sequence |  | 10000 |  | 166 |
| 10000 |  |  |  | true | 1547 |
| 10000 |  | true |  | true | 1835 |
| 10000 |  |  | 10000 | true | 897 |


## _all_docs benchmark
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 31 |
| 1000 |  |  | 49 |
| 10000 |  |  | 238 |
| 100 | true |  | 39 |
| 1000 | true |  | 99 |
| 10000 | true |  | 674 |
| 10000 |  | true | 1006 |
| 10000 | true | true | 1266 |


## _bulk_get benchmark
| count| Duration (ms) |
|--|--|
| 100 | 35 |
| 1000 | 101 |
| 10000 | 937 |


## view benchmark
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 74833 |
| 100 |  |  | 33 |
| 1000 |  |  | 58 |
| 10000 |  |  | 319 |
| 100 | true |  | 41 |
| 1000 | true |  | 119 |
| 10000 | true |  | 969 |
| 100 |  | true | 84 |
| 1000 |  | true | 508 |
| 10000 |  | true | 4625 |
| 10000 | true | true | 5106 |


## nouveau_index benchmark
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 156448 |
| 100 |  |  | 89 |
| 1000 |  |  | 195 |
| 10000 |  |  | 1357 |
| 100 | true |  | 72 |
| 1000 | true |  | 301 |
| 10000 | true |  | 2899 |
| 100 |  | true | 49 |
| 1000 |  | true | 189 |
| 10000 |  | true | 1908 |
| 10000 | true | true | 3144 |