# CouchDb Performance benchmark 

## Database Info

CouchDb version: 3.5.1

Database doc count: 903030

## _changes benchmark 
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 29 |
| 1000 |  |  |  |  | 100 |
| 10000 |  |  |  |  | 677 |
| 100 |  | true |  |  | 38 |
| 1000 |  | true |  |  | 136 |
| 10000 |  | true |  |  | 1050 |
| 100 |  |  | 100 |  | 31 |
| 1000 |  |  | 1000 |  | 36 |
| 10000 |  |  | 10000 |  | 151 |
| 100 | Mid Sequence |  |  |  | 31 |
| 1000 | Mid Sequence |  |  |  | 92 |
| 10000 | Mid Sequence |  |  |  | 673 |
| 100 | Mid Sequence | true |  |  | 37 |
| 1000 | Mid Sequence | true |  |  | 124 |
| 10000 | Mid Sequence | true |  |  | 1023 |
| 100 | Mid Sequence |  | 100 |  | 33 |
| 1000 | Mid Sequence |  | 1000 |  | 34 |
| 10000 | Mid Sequence |  | 10000 |  | 138 |
| 10000 |  |  |  | true | 1321 |
| 10000 |  | true |  | true | 3026 |
| 10000 |  |  | 10000 | true | 972 |


## _all_docs benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 24 |
| 1000 |  |  | 36 |
| 10000 |  |  | 207 |
| 100 | true |  | 29 |
| 1000 | true |  | 82 |
| 10000 | true |  | 3603 |
| 10000 |  | true | 911 |
| 10000 | true | true | 1219 |


## _bulk_get benchmark 
| count| Duration (ms) |
|--|--|
| 100 | 32 |
| 1000 | 76 |
| 10000 | 721 |


## view benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 122021 |
| 100 |  |  | 28 |
| 1000 |  |  | 49 |
| 10000 |  |  | 252 |
| 100 | true |  | 42 |
| 1000 | true |  | 131 |
| 10000 | true |  | 936 |
| 100 |  | true | 81 |
| 1000 |  | true | 582 |
| 10000 |  | true | 5588 |
| 10000 | true | true | 5805 |


## nouveau_index benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 2761777 |
| 100 |  |  | 127 |
| 1000 |  |  | 208 |
| 10000 |  |  | 1321 |
| 100 | true |  | 85 |
| 1000 | true |  | 280 |
| 10000 | true |  | 2330 |
| 100 |  | true | 40 |
| 1000 |  | true | 241 |
| 10000 |  | true | 1785 |
| 10000 | true | true | 2495 |


