# CouchDb Performance benchmark 

## Database Info

CouchDb version: 3.5.0

Database doc count: 903030

## _changes benchmark 
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 18 |
| 1000 |  |  |  |  | 82 |
| 10000 |  |  |  |  | 573 |
| 100 |  | true |  |  | 25 |
| 1000 |  | true |  |  | 120 |
| 10000 |  | true |  |  | 994 |
| 100 |  |  | 100 |  | 15 |
| 1000 |  |  | 1000 |  | 20 |
| 10000 |  |  | 10000 |  | 123 |
| 100 | Mid Sequence |  |  |  | 22 |
| 1000 | Mid Sequence |  |  |  | 78 |
| 10000 | Mid Sequence |  |  |  | 634 |
| 100 | Mid Sequence | true |  |  | 24 |
| 1000 | Mid Sequence | true |  |  | 111 |
| 10000 | Mid Sequence | true |  |  | 952 |
| 100 | Mid Sequence |  | 100 |  | 13 |
| 1000 | Mid Sequence |  | 1000 |  | 21 |
| 10000 | Mid Sequence |  | 1000 |  | 117 |
| 10000 |  |  |  | true | 1481 |
| 10000 |  | true |  | true | 1889 |
| 10000 |  |  | 10000 | true | 979 |


## _all_docs benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 13 |
| 1000 |  |  | 25 |
| 10000 |  |  | 173 |
| 100 | true |  | 17 |
| 1000 | true |  | 66 |
| 10000 | true |  | 618 |
| 10000 |  | true | 1222 |
| 10000 | true | true | 1525 |


## _bulk_get benchmark 
| count| Duration (ms) |
|--|--|
| 100 | 20 |
| 1000 | 59 |
| 10000 | 717 |


