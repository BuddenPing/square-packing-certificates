N146 — update to the existing exact square-packing submission

New certified upper bound (rounded upward): 12.5837822039508342919134679370511513667729
Previous submitted bound: 12.58378220395096600473550813141036063202933591115003177771784379017885104413666461645116413867382945
Exact improvement: 1.317128220401943592092652564497380822204946789899394176764996311828456462620366738294461851416156994E-13
The exact rational side and complete 146-owner witness are in n146.cert.json.
This is a further verified upper-bound refinement, not a new count or an
optimality claim. See COMPARISON.json for exact fractions and source hashes.

Credit: PingYou Ltd — new refinement.
Ryan Xu — original layout. Robert Barnett — preceding refinement and source
certificate. Evan Daniel — contact solver/source custody and earlier N146
regularization. The full prior construction lineage is retained.

After extracting the ZIP, enter its n146 directory and run:
  python3 VERIFY.py
Use Python 3.10+ without -O. No third-party packages or network are needed.
This checks the full 146-square geometry with exact separating axes and an
independent rational polygon algorithm, all 10,585 pairs, the prior witness,
strict improvement, hashes, negative controls, native conversion identity,
and binding of the saved native reports. It also checks the inherited
physical inventory and every recorded equation subset. The coupled metric
solve is documented by its saved states and independent audit; the portable
verifier does not rerun the transcendental numerical solver.

Optional fresh native replay:
  python3 -B native/replay_upstream.py --witness pingyou-n146-rational.yaml
This requires Python 3.14 with mpmath 1.4.1, PyYAML 6.0.3, jsonschema 4.26.0 and
strif 3.1.0 plus their dependencies. Both unchanged Squares Project verifiers
are pinned at 074ac28d4ceb9a1897303f936d794771cfc6a7bd; sources/licenses are
included. The supplied native report was freshly run on this exact YAML.

Native conversion identity alone:
  python3 -B native/convert_witness.py n146.cert.json pingyou-n146-rational.yaml --check

METHOD.txt describes the declared 663-incidence coupled realization and its
limits. construction/inherited/ contains source states and diagnostics;
only root n146.cert.json is the current submission. The authoritative
certificate bytes are unchanged from the banked witness; historic internal
paths in archival metadata are provenance only. New package instructions
and comparisons use local relative paths. SHA256SUMS covers every package
file except itself. No new license is asserted for third-party source data.
