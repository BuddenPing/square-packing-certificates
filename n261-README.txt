N261 — update to the existing exact square-packing submission

New certified upper bound (rounded upward): 16.6787798753429098149372205115301919485639
Previous submitted side: 16.67877987534311177538201229039169882372946695066848863796146138603739655815655211812930432555251660
Improvement over the previous submission: 2.019604447917788615068751656007081556534289642082783756682816594473685717657441133221661674451364419E-13
Additional gain over the intermediate banked refinement: 3.069959170155787555910986804433919493207709523463718128251119049316099175447444650954481825141456089E-15
The exact rational side and complete 261-owner witness are in n261.cert.json.
This is a further verified upper-bound refinement, not a new count or an
optimality claim. See COMPARISON.json for exact fractions and source hashes.

Credit: PingYou Ltd — new refinement.
Ryan Xu — original layout. Robert Barnett — preceding refinement and source
certificate. Evan Daniel — contact solver and source custody. The full prior
construction lineage is retained.

After extracting the ZIP, enter its n261 directory and run:
  python3 VERIFY.py
Use Python 3.10+ without -O. No third-party packages or network are needed.
This checks all 261 unit squares and 33,930 unordered pairs with exact
separating axes and an independent rational polygon algorithm, both prior
witnesses, strict comparisons, hashes, negative controls and native identity.
It reconstructs every one of the 34,974 declared support rows from the exact
source and ordered physical marks; their original full-file SHA256 must
match. It checks every final support inequality, the exact displacement map,
minimum common repair and bounding crop. This can take around a minute.

The compact lossless word encoding avoids bundling a 97 MB redundant matrix.
The original header and all ordered marks are retained, and all coefficients
and gaps are exact functions of the included physical source. No row is
approximated or omitted from the standalone reconstruction/check.

The earlier coupled metric solve is documented by all saved attempts and an
independent audit; VERIFY.py does not rerun that transcendental solver.
Its raw N261 state is invalid and is retained ONLY as a diagnostic under
construction/inherited/. The valid intermediate witness is centre-input.
Only root n261.cert.json is the updated submission. See METHOD.txt.

Optional fresh native replay:
  python3 -B native/replay_upstream.py --witness pingyou-n261-rational.yaml
This requires Python 3.14 with mpmath 1.4.1, PyYAML 6.0.3, jsonschema 4.26.0
and strif 3.1.0 plus dependencies. Both unchanged Squares Project verifiers
are pinned at 074ac28d4ceb9a1897303f936d794771cfc6a7bd; sources/licenses are
included. The supplied native report was freshly run on this exact YAML.

Native conversion identity alone:
  python3 -B native/convert_witness.py n261.cert.json pingyou-n261-rational.yaml --check

The final fixed-frame step bounds each centre coordinate and side increment
by 1e-6 BEFORE repair/cropping. It is not a Euclidean-radius constraint or an
unqualified final displacement bound. Exact repair changes the final
componentwise maximum by less than 2.506e-21 beyond that bound.

The authoritative certificate bytes are unchanged from the banked witness.
Historic internal paths in archival metadata are provenance only; new
package instructions and comparisons use local relative paths. SHA256SUMS
covers every package file except itself. No new license is asserted for
third-party source data. The two geometric criteria share the same input;
separate implementations are not independent human audits.
