N261 — exact rational square-packing submission

Original layout: Ryan Xu.
Preceding refinement and source certificate: Robert Barnett.
Exact certificate refinement and submission: PingYou Ltd.

New certified side, rounded upward: 16.678779875343112
Exact side (authoritative):
264082550134815183799578811397805867521545872101293786829032093683011557790603895828914069201246435266409885720741941674734690338883664199871946111673353/15833445378412762477050048065812278781960763734594433066474650859634653749966841623961990993055780656797317123193633281851761026493708306954105758998705

Previous side: 16.67877987534320774669774826773269092518323465115679640414669826015999513908367661185859533652413313
New side:      16.67877987534311177538201229039169882372946695066848863796146138603739655815655211812930432555251660
Decrease:     9.597131573597734099210145376770048830776618523687412259858092712449372929101097161653262388317201735E-14

The complete witness improves the prior published exact upper bound.
It preserves the unit squares and all orientations; only their centers
and enclosure change. See METHOD.txt and PROVENANCE.json for the exact
construction and source lineage. public-frontier.json records the fresh comparison audit.
This is an upper-bound claim, not a
proof of optimality.

Verification (run from this extracted package directory)

  python3 -B VERIFY.py
  python3 -B verify_geometry.py n261.cert.json

This standalone Python 3.10+ verifier requires no external packages or
network. It checks the certificate hashes, reconstructs the exact center
map and enclosure, checks all 261 unit squares, all 1044 walls and all
33930 pairs, verifies strict improvement and native conversion.

  python3 -B native/convert_witness.py n261.cert.json pingyou-n261-rational.yaml --check
  python3 -B native/replay_upstream.py --witness pingyou-n261-rational.yaml

The native replay requires Python 3.14 and mpmath 1.4.1, PyYAML 6.0.3,
jsonschema 4.26.0 and strif 3.1.0, with their dependencies. It checks the
included upstream source hashes, then runs both unchanged Squares Project
verifiers pinned at 074ac28d4ceb9a1897303f936d794771cfc6a7bd. The two
verifiers allow exact boundary contact and test every square pair.

The .yaml file uses JSON syntax, valid YAML 1.2. The exact centers use
[x, y, t], where t = tan(theta/2). All number strings are exact rationals.
SHA256SUMS binds every package file except itself.

Sources and credit

Prior published certificate:
https://github.com/RobertBarnettProjects/square-packing-research/blob/52cf1cc7ba006731ef76818267216c87bb63281e/certificates/n261.cert
Prior registration: https://github.com/jlevy/squares/issues/505

Upstream verification software and schema:
Joshua Levy, the squares project (https://github.com/jlevy/squares).
See native/UPSTREAM-LICENSE.txt for the unchanged license notice.
No new license is asserted for third-party construction data.
