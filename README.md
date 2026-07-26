# Bangalore Tech Salary Decoder

A data analysis project decoding compensation patterns across 1,000 Bengaluru tech professionals — built in a 2-hour live coding sprint using Python and Pandas.

## The Problem

Every job-seeking student guesses what CTC to ask for. No free tool breaks salary down quantitatively by role, experience, company type, skills, and education tier. This project builds that analysis from scratch on realistic (synthetic) tech compensation data.

## Key Findings

- **Product Managers earn the highest median CTC (31.3 LPA)** — nearly 2x Data Analysts, the lowest-paid role (16.9 LPA).
- **SDE Backend salaries jump +72% between 0–1 and 2–3 years of experience** (11.6 → 20.0 LPA) — the steepest inflection point in the entire career curve.
- **System Design carries the highest skill premium among SDEs (+20.5%)**, ahead of Kubernetes (+7.9%) and ML (+12.4%). AWS showed a slight *negative* premium (-4.3%), suggesting cloud basics have become table-stakes rather than a differentiator.

## What This Project Covers

| Step | Description |
|---|---|
| **Data Cleaning** | Standardized 42 role-title variants into 9 canonical roles, parsed 4 different CTC string formats (including Indian comma notation) into a consistent LPA float, fixed whitespace/casing inconsistencies across company type and education tier |
| **Exploratory Analysis** | CTC distribution by role, experience-based salary curves using `pd.cut`, skill premium analysis using `str.contains`, company-type premium comparison |
| **Advanced Analysis** | Identified most-underpaid professionals relative to their peer group (same role, company type, and experience band) using `groupby` + `transform` |
| **Reporting** | Formatted, readable console report summarizing all findings |

## Tech Stack

- Python
- Pandas
- NumPy

## Repository Contents

- `LiveProject_Salary_Decoder_VaibhavSingh.ipynb` — full analysis notebook, commented section-by-section
- `bangalore_tech_salaries.csv` — dataset (1,015 rows, synthetic)
- `requirements.txt` — dependencies

## Running It Locally

```bash
git clone https://github.com/<your-username>/bangalore-tech-salary-decoder.git
cd bangalore-tech-salary-decoder
pip install -r requirements.txt
jupyter notebook LiveProject_Salary_Decoder_VaibhavSingh.ipynb
```

## Notes

Dataset is synthetic, generated to reflect realistic Indian tech compensation patterns. Built as part of a live project sprint with The Unlox Academy.

---
**Vaibhav Singh** | [LinkedIn](#) | [GitHub](#)
