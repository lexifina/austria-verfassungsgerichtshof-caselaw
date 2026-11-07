# Reproducing this repository

Input: the RIS OGD API v2.6 (Judikatur, Applikation Vfgh, decision texts only), fetched up to 2026-11-07
by `tools/fetch.py` (at most 8 requests a second); austria-law `main` for the overlay.

```
python tools/fetch.py <fetched> --apps Vfgh
python tools/build.py verfassungsgerichtshof <fetched> <empty folder> --today 2026-11-07 --retrieved 2026-11-07
```
