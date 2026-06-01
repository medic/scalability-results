# CouchDb Performance benchmark

## Database Info

CouchDb version: 3.5.0

Database doc count: 903030

## _changes benchmark
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 336 |
| 1000 |  |  |  |  | 638 |
| 10000 |  |  |  |  | 3369 |
| 100 |  | true |  |  | 339 |
| 1000 |  | true |  |  | 685 |
| 10000 |  | true |  |  | 1698 |
| 100 |  |  | 100 |  | 274 |
| 1000 |  |  | 1000 |  | 338 |
| 10000 |  |  | 10000 |  | 931 |
| 100 | Mid Sequence |  |  |  | 333 |
| 1000 | Mid Sequence |  |  |  | 589 |
| 10000 | Mid Sequence |  |  |  | 3042 |
| 100 | Mid Sequence | true |  |  | 339 |
| 1000 | Mid Sequence | true |  |  | 689 |
| 10000 | Mid Sequence | true |  |  | 3968 |
| 100 | Mid Sequence |  | 100 |  | 277 |
| 1000 | Mid Sequence |  | 1000 |  | 340 |
| 10000 | Mid Sequence |  | 10000 |  | 930 |
| 10000 |  |  |  | true | 3841 |
| 10000 |  | true |  | true | 4817 |
| 10000 |  |  | 10000 | true | 1907 |


## _all_docs benchmark
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 267 |
| 1000 |  |  | 375 |
| 10000 |  |  | 1189 |
| 100 | true |  | 317 |
| 1000 | true |  | 511 |
| 10000 | true |  | 2644 |
| 10000 |  | true | 2199 |
| 10000 | true | true | 3368 |


## _bulk_get benchmark
| count| Duration (ms) |
|--|--|
| 100 | 315 |
| 1000 | 632 |
| 10000 | 3091 |


## view benchmark
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 74305 |
| 100 |  |  | 275 |
| 1000 |  |  | 353 |
| 10000 |  |  | 890 |
| 100 | true |  | 317 |
| 1000 | true |  | 520 |
| 10000 | true |  | 2778 |
| 100 |  | true | 324 |
| 1000 |  | true | 893 |
| 10000 |  | true | 6032 |
| 10000 | true | true | 7528 |


## nouveau_index benchmark
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 142668 |
| 100 |  |  | 298 |
| 1000 |  |  | 461 |
| 10000 |  |  | 1949 |
| 100 | true |  | 320 |
| 1000 | true |  | 706 |
| 10000 | true |  | 4445 |
| 100 |  | true | 324 |
| 1000 |  | true | 570 |
| 10000 |  | true | 5584 |
| 10000 | true | true | 7834 |
