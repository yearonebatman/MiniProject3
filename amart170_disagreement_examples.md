# Disagreement Examples — amart170 (validator) & ttb615 (author)

4 of the 50 validated records for ttb615's project set disagreed before discussion (`HasRecovered` 1, `ActivityPattern` 3). All 4 were resolved as **ValidatorKept** after ttb615 reviewed the commit timestamps and repository evidence; see `amart170_validation_log.csv`.

---

### Example 1: mpmccode/mpmc (HasRecovered)
* **Parties:** Author `ttb615`, Validator `amart170`
* **Author:** `Yes (minimal)`
* **Validator:** `No`
* **Reason:** The longest continuous period of zero commits was a 10-month hiatus from December 2024 through September 2025. Following the gap, exactly 4 commits were logged on a single day (2025-10-21) via two small pull requests (#23, #24) adjusting carbon mass parameters in sample input files (`c2h4`, `c2h4p`). A single-day batch of 4 minor configuration corrections after nearly a year of silence represents isolated external maintenance rather than genuine, sustained project recovery.
* **Resolution:** **ValidatorKept** (Adjudicated as `No`).

---

### Example 2: geodynamics/aspect (ActivityPattern)
* **Parties:** Author `ttb615`, Validator `amart170`
* **Author:** `cyclical`
* **Validator:** `steady`
* **Reason:** ASPECT exhibits continuous, unbroken software development spanning 23,494 commits across 347 authors with zero gaps of 3 or more months since 2014. Annual commit velocity has remained stable between 1,600 and 2,200 commits per year for over a decade. A project sustaining a high, uninterrupted baseline of daily pull request merges and continuous integration runner maintenance without multi-month declines fits the definition of a steady project rather than a cyclical one.
* **Resolution:** **ValidatorKept** (Adjudicated as `steady`).

---

### Example 3: hyperopt/hyperopt-sklearn (ActivityPattern)
* **Parties:** Author `ttb615`, Validator `amart170`
* **Author:** `irregular`
* **Validator:** `cyclical`
* **Reason:** The author classified the activity trajectory as `irregular` due to periods of silence. However, inspecting the monthly time series reveals distinct, structured release intervals: an initial active burst (2013–2014), followed by an 18-month dormancy broken by a planned Python 3 and scikit-learn migration (2016), followed again by quiet intervals punctuated by concentrated multi-commit maintenance sprints (e.g., the 2025 sklearn 1.5/1.6 upgrade). This periodic hibernate-and-release cadence represents a cyclical maintenance lifecycle rather than unstructured random bursts.
* **Resolution:** **ValidatorKept** (Adjudicated as `cyclical`).

---

### Example 4: ziotom78/Healpix.jl (ActivityPattern)
* **Parties:** Author `ttb615`, Validator `amart170`
* **Author:** `irregular`
* **Validator:** `cyclical`
* **Reason:** The author selected `irregular`, but the project's extended hiatuses correspond directly to the upstream Julia language release and compatibility roadmap. The longest 9-month pause was explicitly documented in commit messages as holding back changes until Julia 0.6 stabilized without breaking 0.5 backwards compatibility, followed immediately by 692 commits when the `julia06` branch was merged. The project alternates between dormant periods and upgrade cycles tied directly to language runtime milestones.
* **Resolution:** **ValidatorKept** (Adjudicated as `cyclical`).
