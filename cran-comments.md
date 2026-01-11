## Test environments
* local Windows 11 install, R 4.5.2
* win-builder (devel and release)
* R-hub (Fedora Linux, Ubuntu Linux, macOS)

## R CMD check results
0 errors | 0 warnings | 1 note

* Note: "New submission" -> This is technically a new submission because the package was renamed.

## Reverse dependencies
This is a new submission, so there are no reverse dependencies.

## Comments for CRAN
This is a resubmission to address feedback from the initial review (previously named 'ORscrapper').

Changes made based on reviewer feedback:
1. Package renamed to 'ORscraper' (removed extra 'p') to fix typo.
2. Software and API names in DESCRIPTION are now enclosed in single quotes.
3. Added the explicit API web reference to the DESCRIPTION.
4. Replaced \dontrun{} with \donttest{} in all examples.

This package queries the NCBI ClinVar API via 'rentrez'.
- Tests involving the API are mocked using 'mockery' and do not access the network.
- Vignette uses cached data and performs no live API calls.
- Examples use \donttest{} to avoid external calls during CRAN checks.

SystemRequirements 'poppler-cpp' is declared for the 'pdftools' dependency.