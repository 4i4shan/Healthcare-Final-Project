# 🏥 Cracking the Cannibalization Code: A Healthcare Analytics Study
## 🌟 The Big Picture
In the high-stakes world of pharmaceutical sales, launching a new product is a double-edged sword. Our team dived into a classic "Big Pharma" dilemma: How do you introduce a new drug variant without destroying your existing market leader?

Acting as a Healthcare Commercial Analytics team, we analyzed Medicare claims data to track the rollout of a new anesthesia drug (Product 2) and its impact on our company’s reigning champion (Product 1). This wasn't just about crunching numbers; we worked together to identify shifting prescribing habits and uncover growth opportunities in a crowded market.

## 🧩 The Challenge
The anesthesia market is booming as the population ages and surgeries become more common. However, with new products come new risks. Our team used data to answer three critical questions:

Market Shifts: Was our new variant winning over competitors, or was it just taking sales away from our own established brand?

The Competition: How were rivals like Fentanyl and Propofol reacting to our new product launch?

The "Who" and "Where": Which medical specialists were the quickest to switch, and which US regions remained most loyal to the older brands?

## 🧪 Methodology: How We Solved It
As a group, we structured our Python workflow into five distinct phases to move from raw data to executive-level insights:

### 1. Data Consolidation & Engineering
Since the Medicare claims data was provided in multiple parts, we used the glob library to dynamically read and concatenate all CSV files into a single master DataFrame.

The Collaborative Solution: We implemented optimized merging strategies to join provider demographics, patient data, and zip-to-territory mappings while ensuring total record integrity.

### 2. The "Data Scrubbing" Phase
Before beginning our analysis, we performed a collective diagnostic check:

Handling Nulls: We identified and addressed missing NPI (National Provider Identifier) and specialty data to prevent bias.

Normalization: We standardized specialty names and product categories to ensure that "Product 1" and its "Variant" were tracked accurately across different claim formats.

### 3. Multi-Dimensional Market Share Calculation
We didn't settle for just "Total Sales." To understand the true market shift, our team calculated three different versions of Market Share:

Claim Share: Total volume of prescriptions.

Patient Share: The number of unique individuals treated (to see if the variant was reaching new patient populations).

HCP Share: The percentage of healthcare providers actually prescribing the drug.

### 4. Specialty & Geographic Profiling
We wanted to know who was driving the change. Using Pandas grouping and aggregation, we:

Isolated the top 5 medical specialties (Anesthesiology, CRNAs, etc.).

Compared their adoption rates of the variant from 2016 to 2018.

Mapped these results to four major U.S. Census Regions to identify geographic "blind spots."

### 5. Visual Storytelling (Matplotlib & Seaborn)
The final phase was turning our collective findings into a narrative. We built:

100% Stacked Bar Charts: To show the "shrinkage" of Product 1 as the Variant grew.

Comparative Pie Charts: To visualize the prescriber mix for our brands versus competitors.

## 🛠 Our Project Architecture
Data Integration: Cleaning and joining Claims, NPI, Specialty, and Territory data.

Feature Engineering: Creating time-based flags for "Baseline" (2016) and "Post-Launch" (2018) periods.

Statistical Aggregation: Calculating year-over-year percentage growth and cannibalization rates.

## 🛠️ The Toolkit
Language: Python 3.x

Data Heavy-Lifters: Pandas and NumPy for processing and complex merging.

Visualization: Matplotlib and Seaborn for building the market share dashboards.

Environment: Jupyter Notebook.

## 📂 Inside this Repo
ClaimsAnalysis_WorkingFile.ipynb: Our full analytical journey—from loading the raw data to the final visualizations.

BIA 810 Final Project Statement.docx: The original business case and strategic framework that guided our group.

ClaimsAnalysis_WorkingFile.html: A quick-look version of our results (no code-running required!).
