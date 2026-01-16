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

## 💻 My Approach
I turned raw, messy Medicare data into a strategic roadmap using Python:

* **Data Wrangling:** I merged multiple years of claims data, cleaned up provider (NPI) records, and mapped zip codes to regional territories to see the "where" behind the "what."
* **Market Share Engine:** I built a logic to calculate market share not just by sales volume, but by unique patient counts and prescriber loyalty.
* **Visual Storytelling:** I created 100% stacked bar charts and specialty-based pie charts to make complex market shifts easy to understand at a glance.
* **Diagnostic Cleaning:** I performed a deep-dive audit of the dataset to identify missing values and ensure the analysis was grounded in high-quality data.

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
