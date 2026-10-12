# Square-packing certificates — PingYou Ltd

## Contact refinements: 105 and 272 unit squares

Registration requests: [N105 #568](https://github.com/jlevy/squares/issues/568) and [N272 #569](https://github.com/jlevy/squares/issues/569). Submitted 12 October 2026; awaiting maintainer review.

| n | Certified upper bound, rounded upward | Comparison |
|---:|---|---|
| 105 | 10.7893037837481588309268366600396176597363 | More than 4.29007519545e-29 below the entire previous nominal-source rounding interval |
| 272 | 16.9655864748376706357560070334220455696299 | Approximately 5.26079948951952e-16 below the previous published certificate |

These are new metric realizations of inherited contact systems. N105 retains 435 feature incidences; N272 retains 1,564. Every physical unit square is included and exactly verified. Ordinary uniform contractions that merely remove old certificate padding are not claimed as new construction results.

For N105, an inverse-dilation control reproduces the previous side and all 97 nonfree source rows. For N272, the final witness also improves a separately certified pre-stationarity contact projection by approximately 5.2607994895195187e-16. No unpublished N272 generator formula is assumed. Further comparison details and limitations are in the packages.

- N105: [rational certificate](n105.cert.json), [native Witness/v2](pingyou-n105-rational.yaml), [complete package](n105-squares-project.zip), [method and replay](n105-README.txt), [checksums](n105-SHA256SUMS).
- N272: [rational certificate](n272.cert.json), [native Witness/v2](pingyou-n272-rational.yaml), [complete package](n272-squares-project.zip), [method and replay](n272-README.txt), [checksums](n272-SHA256SUMS).

Both packages pass separate exact separating-axis and rational polygon checks, negative controls, native-format identity checks, and both unchanged Squares Project verifiers at `074ac28d4ceb9a1897303f936d794771cfc6a7bd`. Extract either archive, enter its `n105-squares-project` or `n272-squares-project` directory, and run `python3 -B VERIFY.py` without `-O`. These results establish feasible upper bounds; no local or global optimality is claimed.

**Credit:** PingYou Ltd, new contact refinements and submissions. N105 builds on Ryan Xu's layout and Francisco Couzo's refinement. N272 builds on Nate Chaoweeraprasit / SQUISH's arrangement, including its SQUISH s(240) and former Kingbird catalogue s(182) components. Evan Daniel supplied the contact solver. Original software and schema credits and licenses are retained.

The authoritative release of these packages is pinned at `260aaf50230483654802790589c2dfce73237604`. Submission is distinct from maintainer acceptance.

## Exact certificate refinements: 146 and 261 unit squares

Registration requests: [N146 #566](https://github.com/jlevy/squares/issues/566) and [N261 #567](https://github.com/jlevy/squares/issues/567), submitted 12 October 2026 and awaiting maintainer review.

| n | Certified upper bound, rounded upward | Reduction from the preceding exact certificate |
|---:|---:|---:|
| 146 | **12.583782203950967** | approximately 8.01987214927426e-14 |
| 261 | **16.678779875343112** | approximately 9.59713157359773e-14 |

These bounds refine [Robert Barnett's certificates](https://github.com/RobertBarnettProjects/square-packing-research/tree/52cf1cc7ba006731ef76818267216c87bb63281e), registered in [Squares Project #505](https://github.com/jlevy/squares/issues/505). **Ryan Xu** supplied the original layouts, **Robert Barnett** the preceding refinements, and **PingYou Ltd** these exact certificate refinements. The prior N146 comparison also retains **Evan Daniel's** regularization credit.

Every unit square and orientation is preserved. A single exact contraction of the square centers reaches the first pair contact; exact cropping removes remaining wall clearance. The rational witnesses include permitted boundary contacts. No overlap tolerance is used. The bounds establish feasible packings, with no claim of local or global optimality.

- **N146:** [exact certificate](n146.cert.json), [native Witness/v2](pingyou-n146-rational.yaml), [portable verification package](n146-squares-project.zip), [method and provenance](n146-README.txt), [checksums](n146-SHA256SUMS).
- **N261:** [exact certificate](n261.cert.json), [native Witness/v2](pingyou-n261-rational.yaml), [portable verification package](n261-squares-project.zip), [method and provenance](n261-README.txt), [checksums](n261-SHA256SUMS).

Both pass exact construction replay, complete unit-square/wall/pair checks, and both unchanged Squares Project native verifiers at `074ac28d4ceb9a1897303f936d794771cfc6a7bd`. The public-frontier comparison was refreshed on 12 October 2026. Submission and maintainer acceptance are separate stages.

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

A refined exact rational certificate for the existing PingYou Ltd construction:

```
3720240092889639048018577779/250000000000000000000000000
= 14.880960371558556192074311116
```

Thus **s(207) ≤ 14.880960371559**, rounded upward. This is a feasible upper bound, with no claim of local or global optimality.

The original submission was accepted as [T-147](https://github.com/jlevy/squares/blob/074ac28d4ceb9a1897303f936d794771cfc6a7bd/packing/frontier/n-207.md), at `14.8809603730436756319360591381170501178639`. This certificate reduces that exact side by **1.4851194398617480221170501178639E-9**. The refinement is tracked in the existing [issue #503](https://github.com/jlevy/squares/issues/503); acceptance of the original does not imply acceptance of the refinement.

The inherited-frame prescription and whole-owner assembly are retained. This replay uses a new rational approximation to that frame and reduces the centre/container guard from `10000000001/10000000000` to `5000000000001/5000000000000`. It is not an angle search.

### Files and verification

- `01-squares-project.zip`: complete portable evidence and replay package. Extract, enter `01-squares-project`, and run `python3 VERIFY.py` (Python 3.10+ standard library; run without `-O`).
- `n207.cert.json`: exact rational centre/half-angle triples. Internal nongeometric metadata is omitted; every coordinate string, ordering, count and side matches the reviewed witness.
- `pingyou-n207-rational.yaml`: identical geometry in Squares Project Witness/v2 form.
- `n207-verified-comparison.pdf` and `n207.svg`: refreshed comparison and diagram.
- `n207-SHA256SUMS`: checksums of the five artifacts above.

All **207 unit squares, 828 wall conditions and 21,321 unordered pairs** pass three exact geometry implementations. The package verifies its hashes, recorded rational construction replay, lossless native conversion and deliberate invalid-input controls. Both unchanged Squares Project verifiers at `074ac28d4ceb9a1897303f936d794771cfc6a7bd` also pass; receipts, source, licenses and optional native replay instructions are included. These are implementation-level checks, not independent human audits.

The replay begins with the explicit rational realization table and documented owner lineage. It does not rerun exploratory selection or a floating-point solve. The finite guard is included; the unguarded design value is not substituted for the certified bound.

### Construction and credit

**PingYou Ltd**: construction and refinement. **Ryan Xu**: underlying N70 construction, [#432](https://github.com/jlevy/squares/issues/432). **Evan Daniel**: [retained exact N70 source](https://github.com/evand/square-packing/blob/7dfca4e474e5822479f3da3fadf537fb2dbd0efc/search/regularize/lists/certs/n-070.cert.gz) and exact checking tools. **Nate Chaoweeraprasit (SQUISH)**: earlier N207 comparator, [#481](https://github.com/jlevy/squares/issues/481). Additional upstream software and schema credits and licenses are retained.

Earlier releases remain in Git history; no claim is made to invent N70 or patch composition in general.

