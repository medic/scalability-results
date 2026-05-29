
CouchDb version: 3.5.0

Database doc count: 903030

## _changes benchmark
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 323 |
| 1000 |  |  |  |  | 613 |
| 10000 |  |  |  |  | 3121 |
| 100 |  | true |  |  | 333 |
| 1000 |  | true |  |  | 707 |
| 10000 |  | true |  |  | 3479 |
| 100 |  |  | 100 |  | 269 |
| 1000 |  |  | 1000 |  | 329 |
| 10000 |  |  | 10000 |  | 884 |
| 100 | Mid Sequence |  |  |  | 325 |
| 1000 | Mid Sequence |  |  |  | 558 |
| 10000 | Mid Sequence |  |  |  | 3274 |
| 100 | Mid Sequence | true |  |  | 330 |
| 1000 | Mid Sequence | true |  |  | 649 |
| 10000 | Mid Sequence | true |  |  | 4064 |
| 100 | Mid Sequence |  | 100 |  | 265 |
| 1000 | Mid Sequence |  | 1000 |  | 325 |
| 10000 | Mid Sequence |  | 10000 |  | 879 |
| 10000 |  |  |  | true | 3962 |
| 10000 |  | true |  | true | 4430 |
| 10000 |  |  | 10000 | true | 1474 |


## _all_docs benchmark
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 257 |
| 1000 |  |  | 369 |
| 10000 |  |  | 751 |
| 100 | true |  | 309 |
| 1000 | true |  | 485 |
| 10000 | true |  | 2435 |
| 10000 |  | true | 2028 |
| 10000 | true | true | 2086 |


## _bulk_get benchmark
| count| Duration (ms) |
|--|--|
| 100 | 313 |
| 1000 | 602 |
| 10000 | 2781 |


## view benchmark
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 57442 |
| 100 |  |  | 261 |
| 1000 |  |  | 339 |
| 10000 |  |  | 827 |
| 100 | true |  | 310 |
| 1000 | true |  | 492 |
| 10000 | true |  | 2588 |
| 100 |  | true | 299 |
| 1000 |  | true | 760 |
| 10000 |  | true | 4445 |
| 10000 | true | true | 6110 |


## nouveau_index benchmark
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 121588 |
| 100 |  |  | 282 |
| 1000 |  |  | 429 |
| 10000 |  |  | 1601 |
| 100 | true |  | 310 |
| 1000 | true |  | 624 |
| 10000 | true |  | 3788 |
| 100 |  | true | 278 |
| 1000 |  | true | 545 |
| 10000 |  | true | 5414 |
| 10000 | true | true | 7530 |
