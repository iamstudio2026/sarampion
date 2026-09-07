# Ruta de Atención Integrada para Sarampión — Tamaulipas

Measles integrated care pathway. A single-file, offline-capable decision
support tool built for first-level health workers during the 2026 measles
response in Tamaulipas, Mexico — Servicio Nacional de Salud Pública (SNSP),
CeCoSaBi v1.0, February 2026.

Open `index.html` in any browser. No build, no server, no network — it is
meant to work on a nurse's phone in a health centre with poor connectivity.

## Why it is a single HTML file

Field staff needed the pathway on the device already in their pocket, in a
health centre that may have no reliable connection, and printable when the
clinic prefers paper. Anything requiring installation or a login would not
have been used. That constraint drove every technical decision here.

## What it covers

**Clinical pathway.** Triage at first contact against the case definition —
fever with maculopapular rash plus cough, coryza, conjunctivitis or Koplik
spots — branching into suspected-case handling or ordinary care. The suspected
branch walks through immediate airborne isolation and PPE, notification to the
district epidemiologist and registration in the SNSP platform, day-zero
specimen collection (measles/rubella IgM serum, nasopharyngeal swab for PCR,
urine for viral isolation, with cold chain to InDRE/LESP), and classification
and management including vitamin A and 21-day home isolation.

**Parallel epidemiological module.** Case investigation timeline across travel,
schools, waiting rooms, shelters and migrant routes; active house-to-house
search within micro-areas through the community spokesperson network; and
post-exposure prophylaxis windows — MMR for contacts within 72 hours,
immunoglobulin for vulnerable contacts within six days.

**Operations.** Checklists by level of care, operational plan, laboratory and
treatment reference, community protocol, and regionalization.

**Management.** GOLI + CCSB command structure and response indicators.

## Design notes

Tab-based navigation, mobile-first with safe-area handling for notched phones,
and a print stylesheet so any section can be taken to the field on paper.
Images degrade gracefully if assets are missing.

## Context

Written by [Vicente Ernesto González-Aramayo, PhD](https://github.com/vicenternesto86),
epidemiologist (INSP Mexico) and Director of the Centro Coordinador de Salud
para el Bienestar in Tamaulipas, as operational support for the state measles
response.

Published as a reference implementation of an outbreak decision-support tool.
The clinical content reflects Mexican national guidance as of February 2026 and
the local operational structure — adapt both before reuse in another
jurisdiction.
