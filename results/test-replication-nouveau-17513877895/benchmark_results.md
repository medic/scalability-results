# CouchDb Performance benchmark 

## Database Info

CouchDb version: 3.5.0

Database doc count: 903030

## _changes benchmark 
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 18 |
| 1000 |  |  |  |  | 78 |
| 10000 |  |  |  |  | 622 |
| 100 |  | true |  |  | 25 |
| 1000 |  | true |  |  | 119 |
| 10000 |  | true |  |  | 949 |
| 100 |  |  | 100 |  | 15 |
| 1000 |  |  | 1000 |  | 21 |
| 10000 |  |  | 10000 |  | 125 |
| 100 | Mid Sequence |  |  |  | 21 |
| 1000 | Mid Sequence |  |  |  | 84 |
| 10000 | Mid Sequence |  |  |  | 609 |
| 100 | Mid Sequence | true |  |  | 24 |
| 1000 | Mid Sequence | true |  |  | 112 |
| 10000 | Mid Sequence | true |  |  | 1009 |
| 100 | Mid Sequence |  | 100 |  | 13 |
| 1000 | Mid Sequence |  | 1000 |  | 21 |
| 10000 | Mid Sequence |  | 10000 |  | 121 |
| 10000 |  |  |  | true | 1494 |
| 10000 |  | true |  | true | 4651 |
| 10000 |  |  | 10000 | true | 975 |


## _all_docs benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 13 |
| 1000 |  |  | 25 |
| 10000 |  |  | 184 |
| 100 | true |  | 21 |
| 1000 | true |  | 78 |
| 10000 | true |  | 600 |
| 10000 |  | true | 1213 |
| 10000 | true | true | 1493 |


## _bulk_get benchmark 
| count| Duration (ms) |
|--|--|
| 100 | 15 |
| 1000 | 60 |
| 10000 | 710 |


