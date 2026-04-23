# Phase 2 Assumptions and Decisions

## Confirmed Decisions

### 1. Limited reporting window
Phase 2 uses only two full weeks of traffic data:

**14/03/2026 to 27/03/2026**

This decision was made to keep ingestion, validation, and transformation manageable while still providing a realistic analysis window.

### 2. Site file used as reference/master
The TIRTL sites file is treated as the reference source for site-level enrichment, including available descriptive location fields supplied with the dataset.

### 3. No incident attribution in this phase
Incident data is excluded from Phase 2. The current phase is focused on building a clean traffic reporting layer before attempting multi-source analysis.

### 4. No external geography inference
No attempt will be made in this phase to infer road names, corridor groupings, suburb boundaries, or external geography beyond what is explicitly provided in the site reference file.

### 5. Raw files preserved unchanged
Raw source files are retained as downloaded and are not modified. Any standardisation, cleaning, or enrichment is handled in SQL staging objects rather than by editing source files.

## Operating Assumptions

- daily traffic files follow a broadly consistent column structure
- the selected site file contains sufficient attributes to support basic location enrichment
- raw load issues, if found, will be documented in load notes and file inventory
- transformations will prioritise traceability and reporting usability over unnecessary complexity

## Future Exclusions or Changes
Any exclusions, file issues, or structural anomalies discovered during ingestion or profiling will be documented and added here if they materially affect the reporting dataset.
