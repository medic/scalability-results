## Database Info

CouchDb version: 3.5.0

Database doc count: 903030

## _changes benchmark
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 326 |
| 1000 |  |  |  |  | 629 |
| 10000 |  |  |  |  | 3095 |
| 100 |  | true |  |  | 333 |
| 1000 |  | true |  |  | 677 |
| 10000 |  | true |  |  | 3712 |
| 100 |  |  | 100 |  | 276 |
| 1000 |  |  | 1000 |  | 332 |
| 10000 |  |  | 10000 |  | 932 |
| 100 | Mid Sequence |  |  |  | 327 |
| 1000 | Mid Sequence |  |  |  | 581 |
| 10000 | Mid Sequence |  |  |  | 3324 |
| 100 | Mid Sequence | true |  |  | 330 |
| 1000 | Mid Sequence | true |  |  | 620 |
| 10000 | Mid Sequence | true |  |  | 1659 |
| 100 | Mid Sequence |  | 100 |  | 270 |
| 1000 | Mid Sequence |  | 1000 |  | 332 |
| 10000 | Mid Sequence |  | 10000 |  | 783 |
| 10000 |  |  |  | true | 2451 |
| 10000 |  | true |  | true | 4979 |
| 10000 |  |  | 10000 | true | 1889 |


## _all_docs benchmark
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 259 |
| 1000 |  |  | 370 |
| 10000 |  |  | 1153 |
| 100 | true |  | 309 |
| 1000 | true |  | 520 |
| 10000 | true |  | 2618 |
| 10000 |  | true | 2180 |
| 10000 | true | true | 2414 |


## _bulk_get benchmark
| count| Duration (ms) |
|--|--|
| 100 | 311 |
| 1000 | 609 |
| 10000 | 2957 |


## view benchmark
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 95933 |
| 100 |  |  | 269 |
| 1000 |  |  | 345 |
| 10000 |  |  | 887 |
| 100 | true |  | 311 |
| 1000 | true |  | 558 |
| 10000 | true |  | 2825 |
| 100 |  | true | 317 |
| 1000 |  | true | 898 |
| 10000 |  | true | 5815 |
| 10000 | true | true | 7588 |


## nouveau_index benchmark
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 161419 |
| 100 |  |  | 342 |
| 1000 |  |  | 513 |
| 10000 |  |  | 2470 |
| 100 | true |  | 378 |
| 1000 | true |  | 771 |
| 10000 | true |  | 5087 |
| 100 |  | true | 294 |
| 1000 |  | true | 612 |
| 10000 |  | true | 5814 |
| 10000 | true | true | 8309 |