N105: exact contact refinement

Credit: PingYou Ltd, this new contact refinement and submission.
Original layout: Ryan Xu. Preceding refinement: Francisco Couzo.
Contact solver: Evan Daniel. Native verifiers/schema: the Squares Project.

Certified upper bound, rounded upward to 40 decimal places:
s(105) <= 10.7893037837481588309268366600396176597363
Authoritative exact side: 10789303783748158830926836660039617659736218711424421332884365754662904597598593330008796151/1000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000

This is a complete packing of 105 unit squares. Its exact side is below the
entire interval for the original unpadded source design, by at least
4.290075195451292E-29. It also improves the prior rational certificate.
COMPARISON.json records the exact inequalities and source rounding rule.

The original uniform squeeze only removed certificate clearance. This
stronger result instead retains the 435 inherited corner/side and wall
equations using the guarded source as a seed. The solver projects onto these
contacts, then freezes 32 selected translation coordinates during closure.
This changes the metric realization. Active angles follow from the equations;
free-square orientations are inherited. No angle sweep or random perturbation
is used. The source method and exact version are in PROVENANCE.json.

Verification (Python 3.10+, standard library; do not use -O):
  python3 -B VERIFY.py
Both exact geometry implementations test all 105 squares, 420 walls and
5,460 unordered pairs. Negative controls and native roundtrip conversion
are included. SHA256SUMS binds all retained package files except itself.

Native Squares Project replay (Python 3.14 and mpmath, PyYAML, jsonschema,
strif; dependencies as in the pinned source):
  python3 -B native/replay_upstream.py --witness pingyou-n105-rational.yaml
The two unchanged upstream verifiers are bundled at revision
074ac28d4ceb9a1897303f936d794771cfc6a7bd with their license notices.

Optional contact reconstruction (mpmath, numpy, scipy; network required to
fetch the original pinned solver files and verify their hashes):
  python3 -B RECONSTRUCT.py
The source inputs, equations, 140-digit report and exact emitted certificate
are retained in evidence/. Rounded numerical reports are explanatory; the
rational geometry and exact comparison are the mathematical certificate.

No claim of stationarity, local optimality or global optimality is made.
The solver leaves a residual in frozen translation directions. Feasibility
and strict comparison are established by exact arithmetic, independently
of any floating-point optimality label.

Prior source:
https://raw.githubusercontent.com/franciscouzo/square-packing/93570ef79474fd8c35d1293addf095f9eee6a658/certificates/n105.cert
Original solver:
https://raw.githubusercontent.com/evand/square-packing/77f3c0ab479b9a787478ccc8dae378df219f85ea/search/exact/exactsolve.py
