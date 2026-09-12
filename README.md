# An Enhanced Legal Research and Document Generation Framework Using RAG

A Retrieval-Augmented Generation (RAG) framework for legal information retrieval and analysis, built to reduce hallucination and improve traceability of AI-generated legal answers by grounding them in retrieved source documents.

## Overview

Large Language Models are unreliable for legal work because they can hallucinate facts, rely on outdated knowledge, and produce answers that can't be traced back to a source. This project addresses that by combining dense semantic retrieval with evidence-grounded generation:

- Legal documents are chunked and embedded using **all-MiniLM-L6-v2**, then stored in a **ChromaDB** vector database.
- At query time, relevant chunks are retrieved via semantic search and used as grounding context for generating answers.
- The system is benchmarked on **LegalBench-RAG** using the **Precision@k** metric across four datasets: **ContractNLI**, **CUAD**, **MAUD**, and **PrivacyQA**.

### Results (Precision@1)

| Dataset | Precision@1 |
|---|---|
| ContractNLI | 10.03% |
| CUAD | 67.12% |
| MAUD | 17.72% |
| PrivacyQA | 69.07% |

## Authors

Yashwanth Adimulam, Rohith Agudu, Harshith Amanchi, Shaista Farhat, M.A. Jabbar — Dept. of CSE (AI & ML), Vardhaman College of Engineering.

## Contents

- `team_01_report/` — full project report (LaTeX source + compiled PDF)
- `team_01_implementation_paper/` — IEEE-format implementation paper (LaTeX source + compiled PDF), including RAG architecture and workflow diagrams
- `team_01_review_paper/` — review paper source
- `team_01_ppt.pptx` — project presentation
- `team 01 poster.pdf` — project poster
- `team_01_plag_report.pdf` — plagiarism report
- `team_01_major_project.pdf` — consolidated project document
