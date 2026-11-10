# ccbench-uplink-final

**Final** uplink round-robin congestion-control benchmark data over Starlink.

Original experiment name (see `NAMA-ASLI.txt`): `final-uplink-starlink-20261109T220531Z`

## Overview

- Test: **uplink**, round-robin
- Duration per round: **30 seconds**
- Rounds: **20** (`rr-01` … `rr-20`)
- Congestion-control algorithms per round: `indigo`, `pcc`, `vivace` (+ reference `_refNN_cubic` where applicable)
- Data: gzipped data-link / ack-link logs

## Layout

```
data/
  data/
    uplink/
      rr-01/ … rr-20/   (per-round per-algorithm logs)
  provenance/
    patches/
final-uplink-starlink-20261109T220531Z.console.log
final-uplink-starlink-20261109T220531Z.collect.log
NAMA-ASLI.txt
```

## Notes

- This is the validated "FINAL" run of the uplink round-robin series (earlier trials were marked TIDAK-SAH/invalid in the collection pipeline).
- Provenance patches are stored under `data/provenance/patches/`.
