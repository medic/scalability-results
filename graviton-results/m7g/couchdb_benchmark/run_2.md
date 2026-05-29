## Database Info

CouchDb version: 3.5.0

Database doc count: 903030

## _changes benchmark
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 327 |
| 1000 |  |  |  |  | 555 |
| 10000 |  |  |  |  | 3064 |
| 100 |  | true |  |  | 328 |
| 1000 |  | true |  |  | 651 |
| 10000 |  | true |  |  | 3550 |
| 100 |  |  | 100 |  | 270 |
| 1000 |  |  | 1000 |  | 328 |
| 10000 |  |  | 10000 |  | 890 |
| 100 | Mid Sequence |  |  |  | 321 |
| 1000 | Mid Sequence |  |  |  | 558 |
| 10000 | Mid Sequence |  |  |  | 1296 |
| 100 | Mid Sequence | true |  |  | 329 |
| 1000 | Mid Sequence | true |  |  | 652 |
| 10000 | Mid Sequence | true |  |  | 2462 |
| 100 | Mid Sequence |  | 100 |  | 263 |
| 1000 | Mid Sequence |  | 1000 |  | 326 |
| 10000 | Mid Sequence |  | 10000 |  | 884 |
| 10000 |  |  |  | true | 2014 |
| 10000 |  | true |  | true | 4244 |
| 10000 |  |  | 10000 | true | 1702 |


## _all_docs benchmark
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 259 |
| 1000 |  |  | 365 |
| 10000 |  |  | 1115 |
| 100 | true |  | 308 |
| 1000 | true |  | 486 |
| 10000 | true |  | 1602 |
| 10000 |  | true | 2006 |
| 10000 | true | true | 3253 |


## _bulk_get benchmark
| count| Duration (ms) |
|--|--|
| 100 | 312 |
| 1000 | 597 |
| 10000 | 2809 |


## view benchmark
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 57500 |
| 100 |  |  | 259 |
| 1000 |  |  | 341 |
| 10000 |  |  | 759 |
| 100 | true |  | 310 |
| 1000 | true |  | 522 |
| 10000 | true |  | 1541 |
| 100 |  | true | 298 |
| 1000 |  | true | 744 |
| 10000 |  | true | 4558 |
| 10000 | true | true | 6175 |


## nouveau_index benchmark
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 121497 |
| 100 |  |  | 282 |
| 1000 |  |  | 412 |
| 10000 |  |  | 1594 |
| 100 | true |  | 316 |
| 1000 | true |  | 609 |
| 10000 | true |  | 2751 |
| 100 |  | true | 272 |
| 1000 |  | true | 533 |
| 10000 |  | true | 5289 |
| 10000 | true | true | 7406 |
