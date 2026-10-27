# RC3 — 03 review issues

| ID | Status | Evidence |
|---|---|---|
| R01 | Logic fixed in RC2 | Applied expression and function retained; browser export regression required |
| R02 | Logic fixed in RC2 | Scientific notation and Euler constant supported |
| R03 | Logic fixed in RC2 | No fixed-domain probe |
| R04-A | Fixed in RC3 | PNG failure callback uses translation lookup |
| R04-B | Fixed in RC3 | Existing error, score and coordinate text retranslated on language switch |
| R05 | Logic fixed in RC2 | Storage access guarded |
| R06 | Logic fixed in RC2 | Input trimmed |
| R07 | Logic fixed in RC2 | Buttons use bounded zoomAt |

Original approved embedded logo unchanged.

R04 browser checks: language switching of compound errors, RMSE and coordinates, and PNG error text passed.

## RC4 documentation closure

- R01–R07 retain RC3 independent script-level acceptance from 03; no source changes.
- README/CHANGELOG candidate labels corrected; LICENSE and .gitignore retained.
- User-reported physical gesture and offline opening acceptance added to TEST-REPORT.md.
