# CouchDb Performance benchmark 

## Database Info

CouchDb version: 3.5.0

Database doc count: 903030

## _changes benchmark 
| limit| since| include_docs| seq_interval| keys| Duration (ms) |
|--|--|--|--|--|--|
| 100 |  |  |  |  | 41 |
| 1000 |  |  |  |  | 129 |
| 10000 |  |  |  |  | 918 |
| 100 |  | true |  |  | 44 |
| 1000 |  | true |  |  | 155 |
| 10000 |  | true |  |  | 1514 |
| 100 |  |  | 100 |  | 32 |
| 1000 |  |  | 1000 |  | 41 |
| 10000 |  |  | 10000 |  | 168 |
| 100 | Mid Sequence |  |  |  | 33 |
| 1000 | Mid Sequence |  |  |  | 110 |
| 10000 | Mid Sequence |  |  |  | 954 |
| 100 | Mid Sequence | true |  |  | 37 |
| 1000 | Mid Sequence | true |  |  | 186 |
| 10000 | Mid Sequence | true |  |  | 1588 |
| 100 | Mid Sequence |  | 100 |  | 36 |
| 1000 | Mid Sequence |  | 1000 |  | 39 |
| 10000 | Mid Sequence |  | 10000 |  | 163 |
| 10000 |  |  |  | true | 1868 |
| 10000 |  | true |  | true | 2530 |
| 10000 |  |  | 10000 | true | 1143 |


## _all_docs benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| 100 |  |  | 24 |
| 1000 |  |  | 46 |
| 10000 |  |  | 270 |
| 100 | true |  | 35 |
| 1000 | true |  | 111 |
| 10000 | true |  | 832 |
| 10000 |  | true | 1738 |
| 10000 | true | true | 2094 |


## _bulk_get benchmark 
| count| Duration (ms) |
|--|--|
| 100 | 33 |
| 1000 | 84 |
| 10000 | 980 |


## view benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 127889 |
| 100 |  |  | 29 |
| 1000 |  |  | 53 |
| 10000 |  |  | 356 |
| 100 | true |  | 36 |
| 1000 | true |  | 156 |
| 10000 | true |  | 1321 |
| 100 |  | true | 87 |
| 1000 |  | true | 688 |
| 10000 |  | true | 6207 |
| 10000 | true | true | 7022 |


## nouveau_index benchmark 
| limit| include_docs| keys| Duration (ms) |
|--|--|--|--|
| indexing |  |  | 227048 |
| 100 |  |  | 118 |
| 1000 |  |  | 394 |
| 10000 |  |  | 2838 |
| 100 | true |  | 85 |
| 1000 | true |  | 428 |
| 10000 | true |  | 4479 |
| 100 |  | true | 73 |
| 1000 |  | true | 352 |
| 10000 |  | true | 2294 |
| 10000 | true | true | 4029 |


