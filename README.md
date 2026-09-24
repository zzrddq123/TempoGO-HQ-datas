# TempoGO-HQ external data

Large resources for the TempoGO-HQ benchmark, hosted separately from the reviewer code archive.

| file | size | extract to |
|---|---|---|
| `TempoGO-HQ-structures.tar.xz` | 71 MB | `resources/target_structures_mmcif/` |
| `TempoGO-HQ-t0.tar.xz` | 30 MB | `resources/t0/` |
| `TempoGO-HQ-provenance.tar.xz` | 9.4 MB | `private/source_provenance/` |
| `TempoGO-HQ-baseline-predictions.tar.xz` | 2.8 MB | `Results_1389/` |
| `TempoGO-HQ-baseline-engine.tar.xz` | 0.2 MB | `baselines/` |
| `TempoGO-HQ-development-splits.tar.xz` | 0.02 MB | `Results_development/` |

- Structures: 1,389 exact-sequence mmCIF protein structures.
- T0: frozen T0 Swiss-Prot GOA background annotation library.
- Provenance: target-bounded source rows and reconstruction receipts. The full T0 GOA release is referenced by SHA-256 (see `T0_GOA_SOURCE.txt` inside the archive).
- Predictions: frozen prediction tables for the 12 baselines (final metrics are in the reviewer archive's `Results_1389/metrics/`).
- Development splits: train_50 / val_60 subset evaluation of the 12 baselines.
- Engine: baseline orchestration engine source.

The reviewer archive's `download_structures.sh` / `download_extras.sh` fetch these files.
