N146 — exact rational square-packing submission

Original layout: Ryan Xu.
Preceding refinement and source certificate: Robert Barnett.
Earlier comparison: Evan Daniel regularization.
Exact certificate refinement and submission: PingYou Ltd.

New certified side, rounded upward: 12.583782203950967
Exact side (authoritative):
212706675227397903760245606872157807798841438063936454387903056635727898003963615684805096386145327886107738242216669359151930723994424404457105225445545795135/16903238770344720525176157542964020457292350107469085192369697156572885656221218224421809664610386039754206736232577088653206716252450318087651395365606969879

Previous side: 12.58378220395104620345700087404080187257267785933190855204207996206332953979734071875067754299373096
New side:      12.58378220395096600473550813141036063202933591115003177771784379017885104413666461645116413867382945
Decrease:     8.019872149274263044124054334194818187677432423617188447849566067610229951340431990151736169406868849E-14

The complete witness improves the prior published exact upper bound.
It preserves the unit squares and all orientations; only their centers
and enclosure change. See METHOD.txt and PROVENANCE.json for the exact
construction and source lineage. public-frontier.json records the fresh comparison audit.
This is an upper-bound claim, not a
proof of optimality.

Verification (run from this extracted package directory)

  python3 -B VERIFY.py
  python3 -B verify_geometry.py n146.cert.json

This standalone Python 3.10+ verifier requires no external packages or
network. It checks the certificate hashes, reconstructs the exact center
map and enclosure, checks all 146 unit squares, all 584 walls and all
10585 pairs, verifies strict improvement and native conversion.

  python3 -B native/convert_witness.py n146.cert.json pingyou-n146-rational.yaml --check
  python3 -B native/replay_upstream.py --witness pingyou-n146-rational.yaml

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
https://github.com/RobertBarnettProjects/square-packing-research/blob/52cf1cc7ba006731ef76818267216c87bb63281e/certificates/n146.cert
Prior registration: https://github.com/jlevy/squares/issues/505

Upstream verification software and schema:
Joshua Levy, the squares project (https://github.com/jlevy/squares).
See native/UPSTREAM-LICENSE.txt for the unchanged license notice.
No new license is asserted for third-party construction data.
