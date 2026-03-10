## Test environments
* local Windows 11, R 4.5.2
* R-hub (debian-clang, fedora-gcc, macos-arm64)

## R CMD check results
0 errors | 0 warnings | 0 notes

## Reverse dependencies
There are no reverse dependencies.

## CRAN Package Check Results update
This version (0.1.1) fixes the ERRORs reported on 2026-03-10:
* Fixed regex fragility in extract_chip_id() by implementing basename(), preventing absolute path interference on CRAN servers.
* Added skip_on_cran() to test_search_ncbi_clinvar.R to prevent test failures caused by remote NCBI API dynamic responses.