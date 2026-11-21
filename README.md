# The Transcripts Were Never There: A Full-Pile Audit of the Linguistic Atlas of the Gulf States Web Archive, and a Failed Calibration for ASR Re-Transcription

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.24409285.svg)](https://doi.org/10.5281/zenodo.24409285)

Dialectology / language resources · 2026

Author: Atharva Chourey
Affiliation: Atharva Chourey Lab (independent research lab)
ORCID: 0009-0009-9423-1718 (https://orcid.org/0009-0009-9423-1718)

*Manuscript — not yet peer-reviewed.*

## Abstract

The Linguistic Atlas of the Gulf States (LAGS; interviews 1968–83) survives online as 1,082 informant folders of audio at the Linguistic Atlas Project; its formal products — most recently DASS2019 — have used only 64 speakers. We pre-registered a transcription-fidelity audit of the pile: re-transcribe every informant's audio with a general automatic speech recognition (ASR) ruler and score agreement with the original transcriptions. The audit's first finding is that the comparison cannot be run: the folders contain no transcriptions. The per-informant `.xml` is an audio segment index, not a transcript; each folder's only text is a biography; verbatim transcripts exist only for DASS2019's 64, in a separate tree. We therefore report (i) a census and index-integrity audit, and (ii) the pre-registered calibration gate on the curated anchor. The census finds 983 of 1,082 folders (90.9%) hold audio and index, totalling 70,542 segment MP3s across 5,807 reels; but the index disagrees with the files in both directions — 939 indexed segments (1.45%) absent on disk and 962 files unindexed (1,901 in all), including a column-scrambled index and a folder whose 81 indexed segments have no audio. The calibration gate **fails**: re-transcribing two DASS2019 speakers' pile MP3 segments (reel 1; 18,425 reference words) with Whisper large-v3 yields word agreement of 57.4% and 64.9% (pooled 61.9%), far below the pre-registered 85% fitness bar. Per the pre-registration, no fidelity claim is made for the ~850 never-audited informants: the stranded majority of a foundational dialect survey is auditable only for completeness and index integrity.

*Keywords:* dialectology; Linguistic Atlas of the Gulf States; speech archives; automatic speech recognition; Whisper; transcription audit; pre-registration; archive integrity

## Key results

- **The transcripts were never there** — outside DASS2019's curated 64 speakers, the pile holds no verbatim transcripts at all: the per-informant `.xml` is an audio segment index, and each folder's only text is a biography. The pre-registered fidelity comparison (P3) is therefore void as registered — reported, never redefined.
- **The audio survives (P1: pass, narrowly)** — 983 of 1,082 informant folders (90.9%) hold both a segment index and at least one MP3, clearing the pre-registered 90% completeness bar: 70,542 segment MP3s across 5,807 reels. 97 folders hold audio but no index; INF304 holds an index but no audio; INF206A holds neither.
- **The index disagrees with the files in both directions** — 939 of 64,607 indexed segments (1.45%, across 192 folders) name files absent on disk, and 962 of 64,630 on-disk files (1.49%, across 195 folders) appear in no index: 1,901 mismatches in all, including a column-scrambled index and one folder whose index points at a different ("LAWS") tree.
- **The calibration fails, as the pre-registration says it must (P2: fail)** — Whisper large-v3 re-transcription of two DASS2019 speakers' reel-1 segments agrees with the curated transcripts on 57.4% and 64.9% of words (pooled 61.9%; 18,425 reference words), 23.1 points below the registered 85% fitness bar. The general ASR ruler is declared unfit, and **no fidelity claim is made for the ~850 never-audited informants**.
- **Disagreement concentrates (P4)** — the top 5 of 24 scored segments hold 43.5% of all disagreement tokens; by topic, Public Institutions (22.8%), Family (18.1%) and Dwellings (17.9%) lead.

## Read the paper

- [paper.md](paper.md) — full text (Markdown, with figures)
- [paper.pdf](paper.pdf) — full text (PDF)

## Sources and fidelity

Every quantitative claim in the paper is traced to its source file in [SOURCES.md](SOURCES.md). The audit was pre-registered (with five dated amendments) before the comparison runs; the census table, analysis tables and per-segment ASR records are preserved in the lab's project record, and the audit scripts are listed in SOURCES.md. The LAGS audio itself remains the Linguistic Atlas Project's (University of Georgia) and is not redistributed here.

## Licence

This work is licensed under a [Creative Commons Attribution 4.0 International Licence (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/). You may share and adapt it with attribution to Atharva Chourey, Atharva Chourey Lab.

## Cite this work

Chourey, Atharva (Atharva Chourey Lab). Public manuscript record, v1.0.0-publication. Zenodo. https://doi.org/10.5281/zenodo.24409285
