# CouchDb Performance benchmark 

## Database Info

CouchDb version: 3.5.0

Database doc count: 903030

## _changes benchmark 
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 30 |
| 1000 |  |  |  |  | 103 |
| 10000 |  |  |  |  | 596 |
| 100 |  | true |  |  | 38 |
| 1000 |  | true |  |  | 128 |
| 10000 |  | true |  |  | 978 |
| 100 |  |  | 100 |  | 35 |
| 1000 |  |  | 1000 |  | 33 |
| 10000 |  |  | 10000 |  | 136 |
| 100 | Mid Sequence |  |  |  | 33 |
| 1000 | Mid Sequence |  |  |  | 95 |
| 10000 | Mid Sequence |  |  |  | 609 |
| 100 | Mid Sequence | true |  |  | 35 |
| 1000 | Mid Sequence | true |  |  | 113 |
| 10000 | Mid Sequence | true |  |  | 970 |
| 100 | Mid Sequence |  | 100 |  | 34 |
| 1000 | Mid Sequence |  | 1000 |  | 33 |
| 10000 | Mid Sequence |  | 10000 |  | 128 |
| 10000 |  |  |  | true | 1450 |
| 10000 |  | true |  | true | 1826 |
| 10000 |  |  | 10000 | true | 987 |


## _all_docs benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 27 |
| 1000 |  |  | 37 |
| 10000 |  |  | 190 |
| 100 | true |  | 27 |
| 1000 | true |  | 75 |
| 10000 | true |  | 624 |
| 10000 |  | true | 1201 |
| 10000 | true | true | 1531 |


## _bulk_get benchmark 
| count| Duration (ms) |
|--|--|
| 100 | 26 |
| 1000 | 69 |
| 10000 | 693 |


## view benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 118539 |
| 100 |  |  | 25 |
| 1000 |  |  | 46 |
| 10000 |  |  | 269 |
| 100 | true |  | 35 |
| 1000 | true |  | 129 |
| 10000 | true |  | 1133 |
| 100 |  | true | 85 |
| 1000 |  | true | 584 |
| 10000 |  | true | 5432 |
| 10000 | true | true | 6031 |


## nouveau_index benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 185710 |
| 100 |  |  | 110 |
| 1000 |  |  | 962 |
| 10000 |  |  | 2028 |
| 100 | true |  | 74 |
| 1000 | true |  | 357 |
| 10000 | true |  | 3234 |
| 100 |  | true | 50 |
| 1000 |  | true | 241 |
| 10000 |  | true | 1660 |
| 10000 | true | true | 3016 |


