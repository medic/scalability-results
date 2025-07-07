# CouchDb Performance
## Database Info
CouchDb version: 3.5.0

Database doc count: 903030



## _changes 
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 19 |
| 1000 |  |  |  |  | 60 |
| 10000 |  |  |  |  | 551 |
| 100 |  | true |  |  | 20 |
| 1000 |  | true |  |  | 107 |
| 10000 |  | true |  |  | 925 |
| 100 |  |  | 100 |  | 14 |
| 1000 |  |  | 1000 |  | 18 |
| 10000 |  |  | 10000 |  | 110 |
| 100 | Mid Sequence |  |  |  | 16 |
| 1000 | Mid Sequence |  |  |  | 65 |
| 10000 | Mid Sequence |  |  |  | 548 |
| 100 | Mid Sequence | true |  |  | 21 |
| 1000 | Mid Sequence | true |  |  | 108 |
| 10000 | Mid Sequence | true |  |  | 928 |
| 100 | Mid Sequence |  | 100 |  | 13 |
| 1000 | Mid Sequence |  | 1000 |  | 20 |
| 10000 | Mid Sequence |  | 1000 |  | 107 |
| 10000 |  |  |  | Yes | 1434 |
| 10000 |  | true |  | Yes | 1861 |
| 10000 |  |  | 10000 | Yes | 943 |
## _all_docs 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 11 |
| 1000 |  |  | 22 |
| 10000 |  |  | 152 |
| 100 | true |  | 15 |
| 1000 | true |  | 67 |
| 10000 | true |  | 544 |
| 10000 |  | Yes | 1172 |
| 10000 | true | Yes | 1437 |
