# CouchDb Performance benchmark 

## Database Info

CouchDb version: 3.5.0

Database doc count: 903030

## _changes benchmark 
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 39 |
| 1000 |  |  |  |  | 95 |
| 10000 |  |  |  |  | 639 |
| 100 |  | true |  |  | 43 |
| 1000 |  | true |  |  | 130 |
| 10000 |  | true |  |  | 1069 |
| 100 |  |  | 100 |  | 58 |
| 1000 |  |  | 1000 |  | 34 |
| 10000 |  |  | 10000 |  | 144 |
| 100 | Mid Sequence |  |  |  | 43 |
| 1000 | Mid Sequence |  |  |  | 100 |
| 10000 | Mid Sequence |  |  |  | 634 |
| 100 | Mid Sequence | true |  |  | 39 |
| 1000 | Mid Sequence | true |  |  | 135 |
| 10000 | Mid Sequence | true |  |  | 982 |
| 100 | Mid Sequence |  | 100 |  | 34 |
| 1000 | Mid Sequence |  | 1000 |  | 36 |
| 10000 | Mid Sequence |  | 10000 |  | 168 |
| 10000 |  |  |  | true | 1569 |
| 10000 |  | true |  | true | 1922 |
| 10000 |  |  | 10000 | true | 1398 |


## _all_docs benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 26 |
| 1000 |  |  | 40 |
| 10000 |  |  | 204 |
| 100 | true |  | 30 |
| 1000 | true |  | 87 |
| 10000 | true |  | 630 |
| 10000 |  | true | 1269 |
| 10000 | true | true | 1587 |


## _bulk_get benchmark 
| count| Duration (ms) |
|--|--|
| 100 | 26 |
| 1000 | 75 |
| 10000 | 738 |


## view benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 120096 |
| 100 |  |  | 27 |
| 1000 |  |  | 53 |
| 10000 |  |  | 304 |
| 100 | true |  | 46 |
| 1000 | true |  | 162 |
| 10000 | true |  | 1230 |
| 100 |  | true | 93 |
| 1000 |  | true | 595 |
| 10000 |  | true | 5707 |
| 10000 | true | true | 6326 |


## nouveau_index benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 185412 |
| 100 |  |  | 126 |
| 1000 |  |  | 326 |
| 10000 |  |  | 2075 |
| 100 | true |  | 78 |
| 1000 | true |  | 348 |
| 10000 | true |  | 3223 |
| 100 |  | true | 47 |
| 1000 |  | true | 241 |
| 10000 |  | true | 1735 |
| 10000 | true | true | 3091 |


