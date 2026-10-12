# Square-packing certificates — PingYou Ltd

## 302 unit squares

A complete exact rational construction with enclosing side

```
22337844230223278442299999/1250000000000000000000000
= 17.8702753841786227538399992
```

Thus **s(302) ≤ 17.870275384179**, rounded upward. This is a feasible upper bound; no local or global optimality is claimed.

The strongest prior public exact certificate located on 12 October 2026 is [Evan Daniel's regularization of Nate Chaoweeraprasit's SQUISH packing (T-146)](https://github.com/jlevy/squares/blob/562fdbdff1d98948f68b36b81b53f9c8165ffd08/packing/frontier/n-302.md), at 17.872029849081179973812429831968. The new side is smaller by **0.001754464902557219972430631968**, approximately **0.0098168%**. The comparison includes pending public reports and larger-count deletion bounds.

### Files and checking

- `n302-squares-project.zip`: complete evidence, construction and native-format package. Extract, enter `n302-squares-project`, and run `python3 VERIFY.py` (Python 3.10+ standard library; run without `-O`).
- `n302.cert.json`: portable exact rational centres and half-angle parameters. Geometry is unchanged from the independently checked witness; internal nongeometric metadata was omitted.
- `pingyou-n302-rational.yaml`: identical exact geometry in Squares Project Witness/v2 form.
- `n302-verified-comparison.pdf` and `n302.svg`: comparison figure and packing diagram.
- `n302-SHA256SUMS`: hashes of the five artifacts above.

All **302 unit squares, 1,208 wall conditions and 45,451 pairs** pass. Three exact geometry checks accept the witness, and two unchanged native Squares Project verifiers pass at revision `074ac28d4ceb9a1897303f936d794771cfc6a7bd`. The package includes exact reconstruction of the physical-owner decoder, derived cubic frame, explicit rational centre table and recomputed finite guard. Replay does not repeat the exploratory owner selection or floating linear solve. These are implementation-level checks, not independent human audits or a proof of optimality.

### Construction and credit

**PingYou Ltd**: new N302 construction. **Ryan Xu**: underlying N70 construction, [#432](https://github.com/jlevy/squares/issues/432). **Evan Daniel**: [retained exact N70 source](https://github.com/evand/square-packing/blob/7dfca4e474e5822479f3da3fadf537fb2dbd0efc/search/regularize/lists/certs/n-070.cert.gz) and prior N302 regularization. **Nate Chaoweeraprasit (SQUISH)**: prior N302 construction, [#481](https://github.com/jlevy/squares/issues/481). Upstream software and schema credit remains with their authors; licenses are included.

Four source patches contribute 16, 9, 9 and 16 whole squares; two upright banks contribute 105 and 147, totalling 302. A positive middle-seam return crosses a retained short return at a root of `2t^3-3t^2-2t+1=0`, prescribing two coherent tilted frames. The full finite realization has 254 upright squares and 24 squares in each mirrored tilt. Its exact guard is included in the bound. The construction note distinguishes this rational witness from the ideal algebraic limit.

No claim is made to invent N70 or patch composition in general. Submission does not imply external maintainer acceptance.

## 153 unit squares

A complete exact rational construction with enclosing side

```
6435006925203522001385040447/500000000000000000000000000
= 12.870013850407044002770080894
```

Thus **s(153) ≤ 12.870013850408**, rounded upward. This is a feasible upper bound; no local or global optimality is claimed.

The strongest prior exact certificate located on 11 October 2026 is [Evan Daniel's regularization of Nate Chaoweeraprasit's SQUISH packing](https://github.com/evand/square-packing/blob/7dfca4e474e5822479f3da3fadf537fb2dbd0efc/search/regularize/lists/certs/n-153.cert.gz), registered as [T-146](https://github.com/jlevy/squares/blob/5b0eb012e09b48b5044aacb439b4cfacf38935f5/packing/frontier/results.yaml#L15630), at exact side 12.872029849081179973762429831968. The new side is smaller by 0.002015998674135970992348937968 (approximately 0.015662%).

### Files and reproduction

- `n153-squares-project.zip`: complete evidence and native-format package. Extract it, enter `n153-squares-project`, and run `python3 VERIFY.py` (Python 3.10+ standard library; do not use `-O`).
- `n153.cert.json`: the original exact rational centres and half-angle parameters, unchanged byte-for-byte.
- `pingyou-n153-rational.yaml`: identical exact geometry in Squares Project Witness/v2 form (JSON syntax valid as YAML).
- `n153-verified-comparison.pdf`: two-page comparison and construction explanation.
- `n153.svg`: illustration from the exact witness.
- `n153-SHA256SUMS`: hashes of the five N153 artifacts above. `SHA256SUMS` covers the current repository files.

The ZIP contains the explicit rational construction table, N70 source, intermediate N153 control, both prior N153 comparison certificates, symbolic return derivation, three exact geometry checks, native conversion and two successful Squares Project verifier receipts. All 153 unit squares, all 11,628 unordered pairs and every wall pass the exact checks. Replay reconstructs the table and guard; it does not repeat exploratory owner selection or a floating-point solve.

The PDF retains its pre-submission status caption. Historical source-path labels in the JSON are mapped to the included witnesses in `evidence/PROVENANCE.txt`; they are not runtime dependencies. The certificate and PDF are the original reviewed bytes.

### Construction and credit

**PingYou Ltd**: new N153 construction. **Ryan Xu**: underlying N70 construction, announced in [#432](https://github.com/jlevy/squares/issues/432). **Evan Daniel**: [exact N70 source retention](https://github.com/evand/square-packing/blob/7dfca4e474e5822479f3da3fadf537fb2dbd0efc/search/regularize/lists/certs/n-070.cert.gz) and refined prior N153 certificate. **Nate Chaoweeraprasit (SQUISH)**: prior N153 construction, [#481](https://github.com/jlevy/squares/issues/481).

The new construction changes the surviving contact pattern of the boundary-patch approach used for [N207](https://github.com/jlevy/squares/issues/503), then recloses that pattern at a different angle. It contains 121 upright squares and tilted populations of 17 and 15. A final factor 5000000000001/5000000000000 expands centres and container only, leaving the small-square sides exactly one. The reported bound includes this guard.

No claim is made to invent N70 or patch composition in general. The package does not claim independent human review or external maintainer acceptance. Included upstream material retains its attribution and accompanying licence terms; this repository adds no new licence grant for third-party material.

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
