# CouchDb Performance benchmark

## Database Info

CouchDb version: 3.5.0

Database doc count: 903030

## _changes benchmark
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 325 |
| 1000 |  |  |  |  | 580 |
| 10000 |  |  |  |  | 2767 |
| 100 |  | true |  |  | 338 |
| 1000 |  | true |  |  | 682 |
| 10000 |  | true |  |  | 1748 |
| 100 |  |  | 100 |  | 274 |
| 1000 |  |  | 1000 |  | 333 |
| 10000 |  |  | 10000 |  | 926 |
| 100 | Mid Sequence |  |  |  | 326 |
| 1000 | Mid Sequence |  |  |  | 564 |
| 10000 | Mid Sequence |  |  |  | 1489 |
| 100 | Mid Sequence | true |  |  | 333 |
| 1000 | Mid Sequence | true |  |  | 657 |
| 10000 | Mid Sequence | true |  |  | 2725 |
| 100 | Mid Sequence |  | 100 |  | 268 |
| 1000 | Mid Sequence |  | 1000 |  | 329 |
| 10000 | Mid Sequence |  | 10000 |  | 910 |
| 10000 |  |  |  | true | 4190 |
| 10000 |  | true |  | true | 2529 |
| 10000 |  |  | 10000 | true | 1978 |


## _all_docs benchmark
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 259 |
| 1000 |  |  | 368 |
| 10000 |  |  | 1139 |
| 100 | true |  | 310 |
| 1000 | true |  | 526 |
| 10000 | true |  | 1598 |
| 10000 |  | true | 2329 |
| 10000 | true | true | 3631 |


## _bulk_get benchmark
| count| Duration (ms) |
|--|--|
| 100 | 317 |
| 1000 | 609 |
| 10000 | 2949 |


## view benchmark
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 96030 |
| 100 |  |  | 264 |
| 1000 |  |  | 344 |
| 10000 |  |  | 885 |
| 100 | true |  | 311 |
| 1000 | true |  | 546 |
| 10000 | true |  | 2828 |
| 100 |  | true | 312 |
| 1000 |  | true | 904 |
| 10000 |  | true | 5931 |
| 10000 | true | true | 7511 |


## nouveau_index benchmark
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 160769 |
| 100 |  |  | 300 |
| 1000 |  |  | 506 |
| 10000 |  |  | 2473 |
| 100 | true |  | 315 |
| 1000 | true |  | 794 |
| 10000 | true |  | 4970 |
| 100 |  | true | 278 |
| 1000 |  | true | 575 |
| 10000 |  | true | 5676 |
| 10000 | true | true | 8200 |