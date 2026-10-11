# Square-packing certificates — PingYou Ltd

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

Verification, comparison review and package preparation were assisted by OpenAI Codex. The package does not claim external maintainer acceptance or independent human review. Included upstream material retains its attribution and accompanying licence terms; this repository adds no new licence grant for third-party material.
