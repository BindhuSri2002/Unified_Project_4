# 📱 Google Play Store Apps – Exploratory Data Analysis

> A beginner-friendly, end-to-end walk-through that scrubs, explores and visualises the **Google Play Store Apps** dataset.  
> Built with `pandas`, `seaborn`, `matplotlib` and a lot of curiosity.

---

## 🧭 Table of Contents
1. [Business Objective](#business-objective)  
2. [Dataset Snapshot](#dataset-snapshot)  
3. [Pipeline at a Glance](#pipeline-at-a-glance)  
4. [Setup & Installation](#setup--installation)  
5. [Quick-start](#quick-start)  
6. [Key Insights](#key-insights)  
7. [Notebooks & Scripts](#notebooks--scripts)  
8. [Folder Structure](#folder-structure)  
9. [Contributing](#contributing)  
10. [License](#license)

---

## 💡 Business Objective
Understand what makes an Android app successful:
* Which categories dominate the market?  
* Do size & rating influence installs?  
* Where are the outliers and data-quality red-flags?

---

## 📊 Dataset Snapshot
| #Rows   | #Cols | Numeric | Text | Missing |
|---------|-------|---------|------|---------|
| 10 346  | 15    | 6       | 9    | ≤ 15 %  |

**Core columns**  
`App` | `Category` | `Rating` | `Reviews` | `Size (MB)` | `Installs` | `Price` | `Content Rating` | `Genres`

---

## 🚧 Pipeline at a Glance
1. **Load** – `pandas.read_csv()`  
2. **Clean** – strip `+`/`,`, convert units, handle `"Varies with device"`  
3. **Impute** – category-aware mean for `Rating`  
4. **EDA** – distributions, correlation heat-map, scatter & box plots  
5. **Insights** – top categories, rating vs installs, review drivers

---

## ⚙️ Setup & Installation
```bash
git clone https://github.com/<your-username>/google-play-store-eda.git
cd google-play-store-eda

# optional but recommended
python -m venv venv
source venv/bin/activate      # Windows: venv\Scripts\activate

pip install -r requirements.txt
