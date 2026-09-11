# 💳 CredResolve Collections Analytics

> A data-forensics investigation into whether reported recovery growth was real — and where the actual opportunity was hiding.

### The question

A reported **11% month-on-month recovery improvement** looked impressive.

The analysis asked a more useful question:

**Was the improvement real, or was the metric being distorted by calendar days and data-quality issues?**

### Headline finding

The 11% improvement was a **calendar-day artifact**.

After normalizing for the number of days in each month, recovery per day stayed around **₹5.8–₹6.1M/day** across Jan–Jul 2026.

The real actionable finding was a **coverage gap**:

> **22.2% of the loan book — 6,656 of 30,000 accounts, worth ₹231 Cr outstanding — had never been assigned to any collection activity.**

### What this repo contains

```text
raw/              source data
pipeline/         Python + SQL ETL
sql/              staging, golden data, metrics, forensics
golden_dataset/   cleaned outputs + DQ logs
notebook/         executed analysis
reports/          DQ report + production design + executive memo
dashboard/        offline executive dashboard
architecture/     production system diagram
```

### Data-quality work

- duplicate payment ingestion detection
- entity-resolution checks
- timezone normalization
- inconsistent call-disposition mapping
- borrower / agent snapshot reconciliation

### Reproducibility

Two independent pipelines — **Python and SQL** — were cross-checked against one another on the headline numbers.

The result is not just a dashboard; it's a **reproducible analytics investigation**.
