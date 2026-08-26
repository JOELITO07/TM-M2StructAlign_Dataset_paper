# Data in Brief manuscript preparation notes

## Working branch

`data-in-brief-dataset-manuscript`

The original `main` branch was left unchanged.

## Data source frozen for this draft

- Dataset repository: `JOELITO07/Dataset_Structural_GPCRs`
- Public data URL: https://github.com/JOELITO07/Dataset_Structural_GPCRs
- Dataset branch inspected: `master`
- Exact dataset commit used for the manuscript: `3e339cae97116fa04f98769b7324c3443334bc97`
- No GitHub release/DOI was present when this manuscript draft was prepared.

## Verified dataset components described in the manuscript

- 284 full-length human GPCR sequences in 9 groups/subclasses.
- Seven deterministic `_19` subsets (19 proteins each; 133 sequence instances total).
- `GPCRdb/sequences/`: FASTA, GFF3, topology files, and `dataset_summary.csv`.
- `GPCRdb/alphafold_pdb/`: AlphaFold DB PDB coordinate files.
- `GPCRdb/alphafold_json/`: AlphaFold predicted-aligned-error JSON records.
- `GPCRdb/distances/`: C-alpha distance matrices and residue-index maps.
- `GPCRdb/weights/`: PAE-derived confidence weights.
- `GPCRdb/reference_alignments/`: reference FASTA/MSF alignments.
- `GPCRdb/precomputed/`: method-specific precomputed alignments and baseline tables.
- `Tests/`: Caretta, FoldMason, mTM-align, MUSTANG, TM-M2StructAlign, and US-align execution artifacts.
- `scripts/`: acquisition, conversion, structural-matrix, metric-preparation, and aligner-workflow scripts.

## Repository facts corrected relative to older documentation

The manuscript follows the current repository tree rather than stale README descriptions. In particular:

- The current repository does **not** contain `GPCRdb/resultados_software/`; precomputed alignment files are documented under `GPCRdb/precomputed/` and execution artifacts under `Tests/`.
- The current AlphaFold JSON files contain `predicted_aligned_error` matrices, so PAE data are documented as available.
- The Data in Brief article does not claim that experimental RCSB PDB structures are part of the current public dataset unless such files are explicitly present in a future version.

## Data in Brief template requirements addressed

- Title includes the word `dataset`.
- Abstract describes collection, contents, and reuse potential without reporting comparative conclusions.
- Specifications Table completed.
- Five `Value of the Data` bullets supplied.
- Background kept focused on motivation and relation to the companion manuscript.
- Data Description documents repository folders/files.
- Experimental Design, Materials and Methods documents acquisition and derivation workflows.
- Limitations, Ethics, CRediT, Acknowledgements/Funding, Competing Interests, and generative-AI disclosure included.
- Bibliography replaced with dataset-relevant references and kept below the Data in Brief maximum of 20 references.

## Items to complete before journal submission

1. Mint a versioned archive/DOI (for example, Zenodo) for the exact dataset release and replace/add the DOI in the Specifications Table and dataset citation.
2. Confirm final author order, corresponding author, affiliations, and CRediT roles with all co-authors.
3. Confirm the exact Data in Brief `Subject` category in the journal submission form.
4. Compile the manuscript, inspect tables/page breaks, and remove line numbering if required for PDF-to-Word conversion according to the template workflow.
5. Upload any journal-required declaration files separately in the Elsevier submission system.
6. If the public dataset changes after commit `3e339cae...`, either preserve this commit as the cited snapshot or update the manuscript to a new frozen release.
