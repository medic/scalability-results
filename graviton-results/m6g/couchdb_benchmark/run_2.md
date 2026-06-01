# CouchDb Performance benchmark

## Database Info

CouchDb version: 3.5.0

Database doc count: 903030

## _changes benchmark
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 337 |
| 1000 |  |  |  |  | 637 |
| 10000 |  |  |  |  | 3269 |
| 100 |  | true |  |  | 343 |
| 1000 |  | true |  |  | 690 |
| 10000 |  | true |  |  | 3839 |
| 100 |  |  | 100 |  | 287 |
| 1000 |  |  | 1000 |  | 342 |
| 10000 |  |  | 10000 |  | 925 |
| 100 | Mid Sequence |  |  |  | 339 |
| 1000 | Mid Sequence |  |  |  | 639 |
| 10000 | Mid Sequence |  |  |  | 3766 |
| 100 | Mid Sequence | true |  |  | 343 |
| 1000 | Mid Sequence | true |  |  | 751 |
| 10000 | Mid Sequence | true |  |  | 1677 |
| 100 | Mid Sequence |  | 100 |  | 277 |
| 1000 | Mid Sequence |  | 1000 |  | 341 |
| 10000 | Mid Sequence |  | 10000 |  | 948 |
| 10000 |  |  |  | true | 4607 |
| 10000 |  | true |  | true | 5089 |
| 10000 |  |  | 10000 | true | 1995 |


## _all_docs benchmark
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 267 |
| 1000 |  |  | 373 |
| 10000 |  |  | 1173 |
| 100 | true |  | 317 |
| 1000 | true |  | 513 |
| 10000 | true |  | 1821 |
| 10000 |  | true | 2262 |
| 10000 | true | true | 2405 |


## _bulk_get benchmark
| count| Duration (ms) |
|--|--|
| 100 | 316 |
| 1000 | 629 |
| 10000 | 2218 |


## view benchmark
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 75604 |
| 100 |  |  | 269 |
| 1000 |  |  | 352 |
| 10000 |  |  | 892 |
| 100 | true |  | 317 |
| 1000 | true |  | 521 |
| 10000 | true |  | 2794 |
| 100 |  | true | 321 |
| 1000 |  | true | 933 |
| 10000 |  | true | 6179 |
| 10000 | true | true | 6504 |


## nouveau_index benchmark
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 143572 |
| 100 |  |  | 291 |
| 1000 |  |  | 453 |
| 10000 |  |  | 1923 |
| 100 | true |  | 318 |
| 1000 | true |  | 692 |
| 10000 | true |  | 4431 |
| 100 |  | true | 279 |
| 1000 |  | true | 562 |
| 10000 |  | true | 5574 |
| 10000 | true | true | 7931 |