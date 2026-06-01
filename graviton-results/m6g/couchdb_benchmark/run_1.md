# CouchDb Performance benchmark

## Database Info

CouchDb version: 3.5.0

Database doc count: 903030

## _changes benchmark
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 44 |
| 1000 |  |  |  |  | 119 |
| 10000 |  |  |  |  | 920 |
| 100 |  | true |  |  | 50 |
| 1000 |  | true |  |  | 173 |
| 10000 |  | true |  |  | 1323 |
| 100 |  |  | 100 |  | 39 |
| 1000 |  |  | 1000 |  | 47 |
| 10000 |  |  | 10000 |  | 189 |
| 100 | Mid Sequence |  |  |  | 43 |
| 1000 | Mid Sequence |  |  |  | 123 |
| 10000 | Mid Sequence |  |  |  | 846 |
| 100 | Mid Sequence | true |  |  | 52 |
| 1000 | Mid Sequence | true |  |  | 173 |
| 10000 | Mid Sequence | true |  |  | 1266 |
| 100 | Mid Sequence |  | 100 |  | 40 |
| 1000 | Mid Sequence |  | 1000 |  | 46 |
| 10000 | Mid Sequence |  | 10000 |  | 173 |
| 10000 |  |  |  | true | 1571 |
| 10000 |  | true |  | true | 1919 |
| 10000 |  |  | 10000 | true | 933 |


## _all_docs benchmark
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 33 |
| 1000 |  |  | 50 |
| 10000 |  |  | 248 |
| 100 | true |  | 39 |
| 1000 | true |  | 104 |
| 10000 | true |  | 704 |
| 10000 |  | true | 1030 |
| 10000 | true | true | 1336 |


## _bulk_get benchmark
| count| Duration (ms) |
|--|--|
| 100 | 38 |
| 1000 | 101 |
| 10000 | 963 |


## view benchmark
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 74557 |
| 100 |  |  | 61 |
| 1000 |  |  | 58 |
| 10000 |  |  | 317 |
| 100 | true |  | 41 |
| 1000 | true |  | 122 |
| 10000 | true |  | 989 |
| 100 |  | true | 84 |
| 1000 |  | true | 507 |
| 10000 |  | true | 4661 |
| 10000 | true | true | 5064 |


## nouveau_index benchmark
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 168238 |
| 100 |  |  | 69 |
| 1000 |  |  | 203 |
| 10000 |  |  | 1326 |
| 100 | true |  | 72 |
| 1000 | true |  | 290 |
| 10000 | true |  | 2845 |
| 100 |  | true | 55 |
| 1000 |  | true | 227 |
| 10000 |  | true | 1861 |