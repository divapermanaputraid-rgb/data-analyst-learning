## Excel Ad-Hoc Analysis — Learning Log (Day 4)

### Context
This session focuses on handling **ad-hoc analytical requests** using Excel.  
The goal is not automation or dashboards, but **fast, correct reasoning** under limited time and imperfect data.

**Typical scenario:**
* Sudden business question
* Partial data
* No clear metric definition upfront

---

### Objective
**Practice:**
* Translating vague questions into measurable metrics
* Inspecting data before analysis
* Avoiding premature conclusions

---

### Type of Request
Ad-hoc business questions, not recurring reports.

**Examples:**
* *“Why did Lite revenue drop last week?”*
* *“Is usage really increasing, or just sessions?”*
* *“Which user segment is driving cost?”*

---

### Analysis Flow Used

**1. Clarify the Question** Before touching Excel:
* What **decision** might this question influence?
* Is this about **activity, revenue, or cost**?
* What **time window** matters?
> Many ad-hoc requests fail because the question is ambiguous.

**2. Data Inspection (Before Any Formula)** Steps:
* Check row count vs expected entities
* Identify **grain** (user, session, transaction, day)
* Scan for missing or duplicated IDs
* Validate date ranges
> **Insight:** Most errors come from skipping this step.

**3. Define the Right Metric** Common trap:
* Using available columns instead of meaningful metrics
* *Example:* Watch hour $\neq$ business value; **Revenue per user** > total revenue.

**4. Minimal Calculation, Maximum Signal** Used Excel functions:
* `SUMIFS`, `COUNTIFS`, `AVERAGEIFS`
* Basic pivot tables
* **Principle:** Prefer simple aggregation, avoid over-engineering.

**5. Sanity Checks** Before answering:
* Does the result direction make **business sense**?
* Is any segment dominating the outcome?
* What could be missing from the data?

---

### Key Learning
* Ad-hoc analysis is about **speed with discipline**, not complexity.
* **Wrong grain = wrong answer**, even with correct formulas.
* Excel is a **thinking tool**, not just a calculation tool.

---

### Common Mistakes Observed
* Jumping into formulas before understanding the question.
* Treating activity metrics as outcomes.
* Trusting totals without checking distribution.

---

### What Needs Improvement
* Faster identification of primary vs supporting metrics.
* Stronger habit of writing assumptions explicitly.
* Clear separation between **observation** and **interpretation**.

  *(Log ini akan diperbarui seiring bertambahnya jenis analisis Excel, termasuk reporting dan analysis lanjutan.)*
