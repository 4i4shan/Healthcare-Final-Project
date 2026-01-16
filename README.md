# 🏥 Cracking the Cannibalization Code: A Healthcare Analytics Study

## 🌟 The Big Picture
In the high-stakes world of pharmaceutical sales, launching a new product is a double-edged sword. This project dives into a classic **"Big Pharma"** dilemma: **How do you introduce a new drug variant without destroying your existing market leader?**

Acting as a Healthcare Commercial Analytics Leader, I analyzed Medicare claims data to track the rollout of a new anesthesia drug (**Product 2**) and its impact on the company’s reigning champion (**Product 1**). This wasn't just about crunching numbers; it was about identifying shifting prescribing habits and finding growth in a crowded market.

---

## 🧩 The Challenge
The anesthesia market is booming as the population ages and surgeries become more common. However, with new products come new risks. I used data to answer three critical questions:

* **Market Shifts:** Is our new variant (Product 2) winning over competitors, or is it just taking sales away from our own Product 1?
* **The Competition:** How are rivals like Fentanyl and Propofol reacting to our new product launch?
* **The "Who" and "Where":** Which medical specialists (Anesthesiologists vs. CRNAs) are the quickest to switch, and which US regions are the most loyal to the old brands?

---

## 🧪 Methodology: How We Solved It
As a group, we structured our Python workflow into five distinct phases to move from raw data to executive-level insights:

### 1. Data Consolidation & Engineering
Since the Medicare claims data was provided in multiple parts, we used the glob library to dynamically read and concatenate all CSV files into a single master DataFrame.

Key Challenge: Handling large-scale data efficiently.

The Solution: We implemented optimized merging strategies to join provider demographics, patient data, and zip-to-territory mappings without losing record integrity.

### 2. The "Data Scrubbing" Phase
Before any analysis, we performed a thorough diagnostic check:

Handling Nulls: We identified missing NPI (National Provider Identifier) and specialty data.

Normalization: We standardized specialty names and product categories to ensure that "Product 1" and its "Variant" were tracked accurately across different claim formats.

### 3. Multi-Dimensional Market Share Calculation
We didn't settle for just "Total Sales." To understand the true market shift, we calculated three different versions of Market Share:

Claim Share: Total volume of prescriptions.

Patient Share: The number of unique individuals treated (to see if the variant was being used on the same patients or new ones).

HCP Share: The percentage of healthcare providers actually prescribing the drug.

### 4. Specialty & Geographic Profiling
We wanted to know who was driving the change. We used Pandas grouping and aggregation to:

Isolate the top 5 medical specialties (Anesthesiology, CRNAs, etc.).

Compare their adoption rates of the variant from 2016 to 2018.

Map these results to four major U.S. Census Regions to identify geographic "blind spots."

### 5. Visual Storytelling (Matplotlib & Seaborn)
The final phase was turning numbers into a narrative. We built:

100% Stacked Bar Charts: To show the "shrinkage" of Product 1 as the Variant grew.

Comparative Pie Charts: To visualize the prescriber mix for our brands versus competitors like Fentanyl.

## 🛠 Project Architecture
Data Integration: Cleaning and joining Claims, NPI, Specialty, and Territory data.

Feature Engineering: Creating time-based flags for "Baseline" (2016) and "Post-Launch" (2018) periods.

Statistical Aggregation: Calculating year-over-year percentage growth and cannibalization rates.
---

## 🛠️ The Toolkit
* **Language:** Python 3.x
* **Data Heavy-Lifters:** `Pandas` and `NumPy` for processing and complex merging.
* **Visualization:** `Matplotlib` and `Seaborn` for building the market share dashboards.
* **Environment:** Jupyter Notebook.

---

## 📂 Inside this Repo
* **`ClaimsAnalysis_WorkingFile.ipynb`**: The full analytical journey—from loading the raw data to the final visualizations.
* **`BIA 810 Final Project Statement.docx`**: The original business case and strategic framework that guided the project.
* **`ClaimsAnalysis_WorkingFile.html`**: A quick-look version of the results (no code-running required!).
