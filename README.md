[![DOI](https://img.shields.io/badge/DOI-10.82901%2Fnemar.on007719-blue)](https://doi.org/10.82901/nemar.on007719)

<!-- nemar:provenance -->
## Provenance

This dataset is mirrored on NEMAR from OpenNeuro.

- Source: [ds007719](https://openneuro.org/datasets/ds007719)
- DOI: [10.18112/openneuro.ds007719.v1.0.0](https://doi.org/10.18112/openneuro.ds007719.v1.0.0)

## Contributed notes (version 1.0.1)

- The SNIRF files do not open in MNE-Python 1.13: read_raw_snirf stops with "The time unit None is not supported by MNE" (checked on sub-s24 and sub-s58). The files need regenerating with SNIRF v1.1 TimeUnit, LengthUnit and dataUnit; this version changes no SNIRF file.
- trial_type in the events.tsv files uses single-letter codes (G, H, J, L, Z); the events.json files hold only the template description of trial_type, so the meaning of the codes is not stated in this dataset.
- 34 of the 65 events.tsv files are not sorted by onset (BIDS validator warning EVENT_ONSET_ORDER).
- participants.tsv lists 10 participants with no subject folder: sub-s07, sub-s39, sub-s46, sub-s49, sub-s56, sub-s64, sub-s72, sub-s73, sub-s74 and sub-s77 (all their values are n/a).
- Associated paper: doi:10.1162/imag.a.1208. The link rests on matching facts (the same three creators among its authors, 65 participants, 5-minute resting state, LUMO at 12.5 Hz); the paper does not name this record. Likely device, per this inferred paper link: LUMO (Gowerlabs Ltd., London, UK; section 2.2); it is not written into the nirs.json sidecars because the link is inferred. Its section 2.1 states that the study was approved by Wales Research Ethics Committee; its Funding section names the Gianna Angelopoulos Programme for Science and Technology Innovation, the Isaac Newton Trust, a Cambridge NeuroWorks Fellowship and an Alzheimer's Society Clinical Research Fellowship.
- dataset_description.json still holds template text. The OpenNeuro record doi:10.18112/openneuro.ds007719.v1.0.0 lists the creators Emilia Butters, Gemma Bale and John O'Brien; cite that record and the paper.
