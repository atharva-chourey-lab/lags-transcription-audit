# Sources Map — The Transcripts Were Never There (LAGS full-pile audit)

Author: Atharva Chourey
Affiliation: Atharva Chourey Lab (independent research lab)

*Manuscript — not yet peer-reviewed.*

This file maps every key number, verdict and reference in `paper.md` to the source file it was taken from. Nothing in the paper was taken from a source outside this list.

## Primary sources

- `~/workspace/lags-transcription-audit/MANUSCRIPT.md` (submission-package copy: `~/workspace/submission-packages/lags/MANUSCRIPT.md`) — the full manuscript draft (not submitted to any venue). `paper.md` in this repository is that manuscript with only the header/status block and the §7 closing status sentence converted to the lab's publication format; no result, number or claim was altered.
- `~/workspace/lags-transcription-audit/PREREGISTRATION.md` — the registered design, fixed 2026-11-18 before any comparison beyond the Campaign-10 sample INF001; `AMENDMENT-1.md` … `AMENDMENT-5.md` — the five dated amendments, each written before the run it affects.
- `~/workspace/lags-transcription-audit/NOVELTY.md` — the novelty scrub (narrowed-but-open, full-pile form only).
- `~/workspace/lags-transcription-audit/RESULTS-EXHAUSTED.md` — the exhaustion run record: headline, the P1–P4 scorecard, and the calibration-sample rescope account. `RESULTS.md` is the earlier mid-run record, superseded by RESULTS-EXHAUSTED.md.
- `~/workspace/lags-transcription-audit/data/census.csv` and `data/census_summary.json` — the per-folder census and its summary.
- `~/workspace/lags-transcription-audit/data/analysis_tables.json` — the index-integrity and analysis tables.
- `~/workspace/lags-transcription-audit/results/p2_p4_score.json`, `results/calibration_by_informant.csv`, `results/p4_by_segment.csv`, `results/p4_by_topic.csv` — the calibration and concentration scores; per-segment ASR records are preserved under `results/asr/` in the project record.
- `~/workspace/lags-transcription-audit/scripts/` — census.py, census_fix.py, asr_audit.py, complete_027.py, analysis.py, analyse_results.py, manual_complete.py.

## External sources

- Linguistic Atlas Project (University of Georgia), LAGS web archive — Speakers index and informant folders, https://www.lap.uga.edu/Projects/LAGS/Speakers/ (census as of 18 November 2026). The audio remains the Linguistic Atlas Project's and is not redistributed.
- DASS2019 — Kretzschmar et al. 2019, *Transcriptions of the Digital Archive of Southern Speech* (the curated 64-speaker anchor; verbatim transcripts). Underlying corpora: *Digital Archive of Southern Speech*, LDC2012S03; NLP version, LDC2016S05.
- Whisper large-v3 (Radford et al. 2023), run via faster-whisper / CTranslate2 with Silero VAD; agreement scored with jiwer. The fine-tuned-ruler contrast is Coats 2026 (DASS2019_NLP, LREC 2026).

## Key numbers and their sources

| Claim in paper | Value | Source file |
|---|---|---|
| Informant folders in the Speakers index | 1,082 | data/census.csv; RESULTS-EXHAUSTED.md |
| Folders holding audio + index (P1) | 983 (90.9%) — PASS vs the registered ≥90% bar | data/census_summary.json; PREREGISTRATION.md |
| Audio but no index / index but no audio / neither | 97 / 1 (INF304) / 1 (INF206A) | data/census.csv |
| Segment MP3s / reels | 70,542 / 5,807 | data/census_summary.json |
| Indexed segments absent on disk | 939 of 64,607 (1.45%), across 192 folders | data/analysis_tables.json |
| On-disk files unindexed | 962 of 64,630 (1.49%), across 195 folders | data/analysis_tables.json |
| Total index–file mismatches | 1,901 | data/analysis_tables.json |
| Calibration, INF025 | 57.4% word agreement (7,515 reference words) | results/calibration_by_informant.csv |
| Calibration, INF027 | 64.9% (10,910 reference words; one decode-failed segment scored as deletions — a floor) | results/calibration_by_informant.csv; AMENDMENT-4.md |
| Calibration, pooled (P2) | 61.9% (18,425 words) vs the registered 85% bar — FAIL, ruler declared unfit | results/p2_p4_score.json; PREREGISTRATION.md |
| Fidelity comparison outside the curated 64 (P3) | VOID as registered — no transcripts exist to compare against | RESULTS-EXHAUSTED.md; AMENDMENT-1.md |
| Disagreement concentration (P4) | Top-5 of 24 segments hold 43.5% of disagreement tokens (3,058 of 7,023); topics: Public Institutions 22.8%, Family 18.1%, Dwellings 17.9% | results/p4_by_segment.csv; results/p4_by_topic.csv |

## Novelty and framing notes

- The claim is an audit with a registered calibration failure — a census and index-integrity result, plus a *negative* calibration verdict — stated with its declared limitations (calibration rests on two informants and one reel each; census figures are as of 18 November 2026 against a live site). All limitations in the paper's §6 are carried over unedited.
- No fidelity or transcription-quality claim is made for the ~850 informants outside DASS2019, per the pre-registration; the paper's §4.5 reports P3 as void rather than redefining it.
- Status: public manuscript, not peer-reviewed, not submitted to any venue.
