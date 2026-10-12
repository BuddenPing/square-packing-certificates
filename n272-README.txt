N272: exact contact-preserving refinement

Credit: PingYou Ltd, this new contact refinement and submission.
Original arrangement: Nate Chaoweeraprasit / SQUISH.
Contact solver: Evan Daniel. Native verifiers/schema: the Squares Project.
Original component provenance is retained in construction/source-summary.csv.

Certified upper bound, rounded upward to 40 decimal places:
s(272) <= 16.9655864748376706357560070334220455696299
Authoritative exact side: 1696558647483767063575600703342204556962987576825904423514291493830293022275118026464939778830359993334240647227/100000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000

This complete packing improves the published rational certificate by
5.2607994895195202931e-16. It also improves an independently reconstructed,
exact-certified pre-KKT inherited-contact projection by 5.2607994895195186966e-16.
COMPARISON.json records the exact inequalities. The source documents about
1e-30 certification overhead but does not publish an exact unpadded scalar
or guard formula. No such formula is presumed.

The original common-center squeeze only removed certificate clearance.
This stronger result retains all 1,564 inherited corner/edge and wall
incidences, with 22 translations frozen during contact closure. Active
angles follow from the equations. The orientations of two free squares
(indices 115 and 116, zero based) are inherited. No angle sweep, random
perturbation, or new contact topology is used. The 100- and 120-digit
contact-side results agree within 1.17e-89.

Verification (Python 3.10+, standard library; do not use -O):
  python3 -B VERIFY.py
The independent exact geometry implementations each inspect all 272 squares,
1,088 walls and 36,856 unordered pairs for the new witness, prior witness
and inherited-contact projection. Hashes, source bindings, native conversion,
negative controls and the optional scoped dual bound are checked as well.

Native Squares Project replay (Python 3.14; mpmath, PyYAML, jsonschema, strif):
  python3 -B native/replay_upstream.py --witness pingyou-n272-rational.yaml
Two unchanged upstream verifiers are bundled at revision
074ac28d4ceb9a1897303f936d794771cfc6a7bd with their license notices.

Optional contact reconstruction (mpmath, numpy, scipy):
  python3 -B construction/reproduce.py
Construction equations, exact witnesses, numerical reports and solver
source are in construction/. An additional rational dual lower bound
applies to specified source separation branches and a stated angular
neighborhood; see construction/CONSTRUCTION.txt for its precise scope.
It is not presented as a guarantee about an unpublished source generator.

No claim of stationarity, local optimality or global optimality is made.
The mathematical claim is exact feasibility and the stated strict
comparisons, independently of numerical optimizer labels.

Prior source:
https://raw.githubusercontent.com/itsnaka/squish-certs/56fa71f949234b63534772b3f3b4f1320fbf2afd/squish-submission-2026-10-11/n272/n272.cert.json
Original solver:
https://raw.githubusercontent.com/evand/square-packing/31523f87316bdfda00f5459dd9077928e264f133/search/exact/exactsolve.py
