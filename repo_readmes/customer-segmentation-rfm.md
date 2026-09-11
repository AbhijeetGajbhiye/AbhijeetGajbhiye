# 📊 Customer Segmentation — RFM Analysis

> Find the customers worth protecting, the customers worth winning back, and the customers not worth chasing.

### The project

RFM (Recency, Frequency, Monetary) analysis on **1,633 online retail orders from ~340 customers**.

Instead of collapsing everything into one score, the analysis separates **Recency** from a combined Frequency/Monetary view so that "recent but low-spend" customers don't get mixed with "high-value but gone quiet" customers.

### What came out

| Segment | Customers | Revenue share | Avg. recency |
| --- | ---: | ---: | ---: |
| Champions | 68 | 55.1% | 14 days |
| At Risk | 45 | 31.2% | 157 days |
| Occasional / Nurturing | 63 | 6.0% | 53 days |
| Loyal | 15 | 4.8% | 34 days |
| Lost | 67 | 1.5% | 185 days |
| New / Low-Spend | 42 | 1.4% | 13 days |

### Key takeaway

**37.7% of customers drive 86.3% of revenue.**

The most interesting segment is **At Risk**: customers who historically behave like high-value buyers but haven't ordered for roughly five months on average.

### Stack

`Python` `Pandas` `RFM` `Data Analysis` `Matplotlib`

### Files

- `rfm_analysis.py` — analysis pipeline
- `online_retail_orders.csv` — raw orders
- `rfm_customer_table.csv` — customer-level output
- `rfm_segment_summary.csv` — segment summary
- `chart*.png` — visual outputs
