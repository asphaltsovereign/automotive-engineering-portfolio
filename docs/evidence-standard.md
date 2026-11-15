# Engineering evidence standard

| Label | Meaning |
|---|---|
| Verified software check | A named command ran on the stated source/environment; log is retained |
| Hardware measurement | Actual instrumented observation with procedure, calibration/reference and raw record |
| Simulation | Model-generated output with assumptions and parameter/version provenance |
| Historical reported result | Preserved earlier record; not reproduced in the current consolidation |
| Design target | Requirement or acceptance criterion, not an achieved result |
| Not run / unavailable | No supporting execution or artifact is available |

Every result should identify source commit, data hash, environment/dependency versions, procedure, denominator and failure conditions. Retain negative results and limitations. Link requirements to the actual implementation and check. A screenshot is a UI observation, not a substitute for a raw dataset or physical measurement.

Use small commits representing actual source recovery, a coherent documentation change, a test/fix or a verified result. Use current dates. Preserve real Git history during transfers. Do not create empty commits, fake issue closures, backdated work or an activity schedule designed to imitate engineering.

Public examples must be synthetic or properly licensed and de-identified. Remove credentials, customer/vehicle identifiers, exact location and private academic/business documents. Keep unpublished invention mechanisms and institutional/team material outside public repositories until disclosure and attribution are resolved.
