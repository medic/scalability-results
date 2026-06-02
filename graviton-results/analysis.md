# Graviton benchmark data: m5 vs m6g vs m7g

## Pricing (us-east-1, on-demand)

| Instance | Arch | vCPU / RAM | $/hr | $/yr (1 inst) | vs m5 |
|---|---|---|---|---|---|
| m5.2xlarge | x86 (Intel) | 8 / 32 GiB | $0.3840 | $3,363.84 | — |
| m6g.2xlarge | Graviton2 | 8 / 32 GiB | $0.3080 | $2,698.08 | −20% (−$665.76/yr) |
| m7g.2xlarge | Graviton3 | 8 / 32 GiB | $0.3264 | $2,859.26 | −15% (−$504.58/yr) |

Per-instance figures. Savings Plans / Reserved / Spot change the absolute dollars.

## Scalability — JMeter `sync` load test

Averaged across runs per concurrency level (2–3 runs each):

| Type | Conc | Runs | Err % | Mean (s) | Median (s) | p95 (s) | Max (s) | Throughput /s |
|---|---|---|---|---|---|---|---|---|
| m5  | 30  | 2 | 0.0 | 80.8  | 83.6  | 84.5  | 84.8  | 0.351 |
| m5  | 60  | 3 | 0.0 | 154.0 | 164.4 | 165.2 | 165.5 | 0.362 |
| m5  | 100 | 3 | 6.3 | 235.4 | 260.8 | 261.8 | 262.3 | 0.382 |
| m6g | 30  | 3 | 0.0 | 68.5  | 70.4  | 71.5  | 71.6  | 0.420 |
| m6g | 60  | 3 | 0.0 | 118.0 | 125.2 | 126.2 | 126.4 | 0.474 |
| m6g | 100 | 3 | 0.0 | 196.3 | 209.2 | 211.1 | 211.6 | 0.472 |
| m7g | 30  | 3 | 0.0 | 51.8  | 53.2  | 54.0  | 54.3  | 0.548 |
| m7g | 60  | 3 | 0.0 | 90.5  | 95.5  | 96.8  | 97.2  | 0.615 |
| m7g | 100 | 3 | 0.0 | 151.2 | 161.6 | 162.6 | 163.0 | 0.613 |

Per-run error detail at concurrency 100:
- m5: runs returned 3.0%, 15.0%, 1.0% errors (avg 6.3%). Max response times ~243–273s.
- m6g: 0% errors across all 3 runs.
- m7g: 0% errors across all 3 runs.

## CouchDB micro-benchmarks

Geometric mean of per-row duration ratios over 35 query rows common to all three
(two runs averaged per type; ratio >1 means the named type was faster than the divisor):

| Comparison | Geomean ratio |
|---|---|
| m5 ÷ m6g  | 1.12 |
| m5 ÷ m7g  | 1.38 |
| m6g ÷ m7g | 1.23 |

Index build times (ms, two runs averaged):

| Operation | m5 | m6g | m7g |
|---|---|---|---|
| view indexing | ~101,584 | ~74,695 | ~57,916 |
| nouveau indexing | ~195,153 | ~162,343 | ~132,012 |

## Throughput per dollar

`sync` throughput at concurrency 100 and CouchDB geomean speedup, each divided by hourly price
and normalized to m5 = 1.00:

| Type | Sync throughput /s ÷ $/hr | normalized | CouchDB geomean ÷ $/hr | normalized |
|---|---|---|---|---|
| m5  | 0.382 / 0.384 = 0.995 | 1.00 | 1.00 / 0.384 = 2.60 | 1.00 |
| m6g | 0.472 / 0.308 = 1.532 | 1.54 | 1.12 / 0.308 = 3.64 | 1.40 |
| m7g | 0.613 / 0.326 = 1.881 | 1.89 | 1.38 / 0.326 = 4.23 | 1.63 |

## Notes / caveats

- Pricing is us-east-1 on-demand. Confirm rates for your region and commitment model.
- The m5 concurrency-100 max response times (~243–273s) sit near a likely request-timeout ceiling; the errors in those runs may be timeouts rather than failures of a different kind.
