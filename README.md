# Square-packing certificates — PingYou Ltd

## 302 unit squares

A refined exact rational certificate for the existing N302 construction, with enclosing side

```
1787027538273375975382555057/100000000000000000000000000
= 17.87027538273375975382555057
```

Thus **s(302) ≤ 17.870275382734**, rounded upward. This is a feasible upper bound; no local or global optimality is claimed.

This supersedes our original [N302 submission](https://github.com/jlevy/squares/issues/564), reducing its side by **0.00000000144486300001444863**. It refines the square-centre realization at the same cubic frame and uses the same guard multiplier. The original release remains available at commit `a0e6fb4185bdfff237e4a8106214119b9c122c7d`.

The earlier public comparator is [Evan Daniel's regularization of Nate Chaoweeraprasit's SQUISH packing (T-146)](https://github.com/jlevy/squares/blob/562fdbdff1d98948f68b36b81b53f9c8165ffd08/packing/frontier/n-302.md), at 17.872029849081179973812429831968. The new side is smaller by **0.001754466347420219986879261968**, approximately **0.0098168%**. The comparison includes pending public reports and larger-count deletion bounds.

### Files and checking

- `n302-squares-project.zip`: complete evidence, construction and native-format package. Extract, enter `n302-squares-project`, and run `python3 VERIFY.py` (Python 3.10+ standard library; run without `-O`).
- `n302.cert.json`: portable exact rational centres and half-angle parameters. Geometry is unchanged from the independently checked witness; internal nongeometric metadata was omitted.
- `pingyou-n302-rational.yaml`: identical exact geometry in Squares Project Witness/v2 form.
- `n302-verified-comparison.pdf` and `n302.svg`: comparison figure and packing diagram.
- `n302-SHA256SUMS`: hashes of the five artifacts above.

All **302 unit squares, 1,208 wall conditions and 45,451 pairs** pass. Three exact geometry checks accept the witness, and two unchanged native Squares Project verifiers pass at revision `074ac28d4ceb9a1897303f936d794771cfc6a7bd`. The package includes the physical-owner lineage, cubic frame, explicit rational centre table and recomputed finite guard. Replay checks the recorded finite realization; it does not repeat the exploratory selection or floating linear solve. The bank owners remain explicit but their centres are realized individually. These are implementation-level checks, not independent human audits or a proof of optimality.

### Construction and credit

**PingYou Ltd**: new N302 construction. **Ryan Xu**: underlying N70 construction, [#432](https://github.com/jlevy/squares/issues/432). **Evan Daniel**: [retained exact N70 source](https://github.com/evand/square-packing/blob/7dfca4e474e5822479f3da3fadf537fb2dbd0efc/search/regularize/lists/certs/n-070.cert.gz) and prior N302 regularization. **Nate Chaoweeraprasit (SQUISH)**: prior N302 construction, [#481](https://github.com/jlevy/squares/issues/481). Upstream software and schema credit remains with their authors; licenses are included.

Four source patches contribute 16, 9, 9 and 16 whole squares; two upright banks contribute 105 and 147, totalling 302. A positive middle-seam return crosses a retained short return at a root of `2t^3-3t^2-2t+1=0`, prescribing two coherent tilted frames. The full finite realization has 254 upright squares and 24 squares in each mirrored tilt. Its exact guard is included in the bound. The construction note distinguishes this rational witness from the ideal algebraic limit.

No claim is made to invent N70 or patch composition in general. Submission does not imply external maintainer acceptance.

## 153 unit squares

A refined exact rational certificate for the existing PingYou Ltd construction:

```
3217503462601758500692520223/250000000000000000000000000
= 12.870013850407034002770080892
```

Thus **s(153) ≤ 12.870013850408**, rounded upward. This is a feasible upper bound, with no claim of local or global optimality.

The original submission was accepted as [T-148](https://github.com/jlevy/squares/blob/074ac28d4ceb9a1897303f936d794771cfc6a7bd/packing/frontier/n-153.md), at `12.870013850407044002770080894`. This certificate reduces that exact side by **1.0000000000002E-14**. The refinement is tracked in the existing [issue #504](https://github.com/jlevy/squares/issues/504); acceptance of the original does not imply acceptance of the refinement.

The existing A=C return, rational orientations and guard `5000000000001/5000000000000` are unchanged. The finite centre/side realization is tighter; some free centres move substantially. The twelve-decimal reporting bound is unchanged.

### Files and verification

- `n153-squares-project.zip`: complete portable evidence and replay package. Extract, enter `n153-squares-project`, and run `python3 VERIFY.py` (Python 3.10+ standard library; run without `-O`).
- `n153.cert.json`: exact rational centre/half-angle triples. Internal nongeometric metadata is omitted; every coordinate string, ordering, count and side matches the reviewed witness.
- `pingyou-n153-rational.yaml`: identical geometry in Squares Project Witness/v2 form.
- `n153-verified-comparison.pdf` and `n153.svg`: refreshed comparison and diagram.
- `n153-SHA256SUMS`: checksums of the five artifacts above.

All **153 unit squares, 612 wall conditions and 11,628 unordered pairs** pass three exact geometry implementations. The package verifies its hashes, recorded rational construction replay, lossless native conversion and deliberate invalid-input controls. Both unchanged Squares Project verifiers at `074ac28d4ceb9a1897303f936d794771cfc6a7bd` also pass; receipts, source, licenses and optional native replay instructions are included. These are implementation-level checks, not independent human audits.

The replay begins with the explicit rational realization table and documented owner lineage. It does not rerun exploratory selection or a floating-point solve. The finite guard is included; the unguarded design value is not substituted for the certified bound.

### Construction and credit

**PingYou Ltd**: construction and refinement. **Ryan Xu**: underlying N70 construction, [#432](https://github.com/jlevy/squares/issues/432). **Evan Daniel**: [retained exact N70 source](https://github.com/evand/square-packing/blob/7dfca4e474e5822479f3da3fadf537fb2dbd0efc/search/regularize/lists/certs/n-070.cert.gz) and exact checking tools. **Nate Chaoweeraprasit (SQUISH)**: earlier N153 comparator, [#481](https://github.com/jlevy/squares/issues/481). Additional upstream software and schema credits and licenses are retained.

Earlier releases remain in Git history; no claim is made to invent N70 or patch composition in general.

## 207 unit squares

A complete exact rational construction with enclosing side

```
148809603730436756319360591381170501178639/10000000000000000000000000000000000000000
= 14.8809603730436756319360591381170501178639
```

Thus **s(207) ≤ 14.880960373044**, rounded upward. This is a feasible upper bound; no global or local optimality is claimed.

The public comparison checked on 11 October 2026 is [Nate Chaoweeraprasit's SQUISH result, submission #481](https://github.com/jlevy/squares/issues/481), with side 14.8855063088416776824135541958084… . The new side is smaller by approximately 0.00454593579800205 (0.03054%).

### Files and reproduction

- `01-squares-project.zip`: complete self-contained evidence and native-format package. Extract it, enter the extracted `01-squares-project` directory, and run `python3 VERIFY.py` (Python 3.10+ standard library; do not use `-O`).
- `n207.cert.json`: exact rational centres and half-angle parameters, with full source/assembly provenance. Its geometry is identical to the certificate inside the ZIP.
- `pingyou-n207-rational.yaml`: the same exact geometry in Squares Project Witness/v2 form (JSON syntax valid as YAML).
- `n207-verified-comparison.pdf`: two-page comparison and construction explanation.
- `n207.svg`: illustration from the exact witness.
- `SHA256SUMS`: hashes of this release's files.

The ZIP includes the N70 source, prior N207 certificate, deterministic exact reconstruction, three exact geometry implementations, two successful upstream Squares Project verifier receipts, format-conversion checks and replay instructions. All 207 unit squares, all 21,321 unordered pairs and every wall pass the exact checks. It also contains the prepared submission draft; historical wording in that draft about publication status predates this repository.

The direct JSON file has two source-path metadata strings made relative for portability. Its exact coordinates, orientations, side and all remaining values are unchanged from the reviewed original; `evidence/document-binding.json` inside the archive retains original/portable hashes. Source references in this file resolve within the extracted package's `evidence/` directory.

### Construction and credit

**PingYou Ltd**: new N207 assembly. **Ryan Xu**: the N70 source construction, announced in [#432](https://github.com/jlevy/squares/issues/432). **Evan Daniel**: exact source retention through [the pinned N70 certificate](https://github.com/evand/square-packing/blob/7dfca4e474e5822479f3da3fadf537fb2dbd0efc/search/regularize/lists/certs/n-070.cert.gz). **Nate Chaoweeraprasit (SQUISH)**: prior N207 comparison.

Two differently placed source patches retain 60 and 69 whole unit squares; 7×6 and 6×6 grids add 42 and 36. Total: 207. A final factor 10000000001/10000000000 expands centres and container only, leaving small-square sides exactly one. The reported bound includes this guard. No claim is made to invent the N70 packing or patch composition in general.

The package does not claim external maintainer acceptance or independent human review. Included upstream material retains its attribution and accompanying licence terms; this repository adds no new licence grant for third-party material.
