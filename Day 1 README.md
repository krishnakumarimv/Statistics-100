# Statistics 100 — Day 1 Exercise

## 🧩 Task

Use Python to **summarize a small business dataset** and identify what statistics can answer.

## 📊 Dataset

**Synthetic Sales**
A small hand-crafted dataset of 14 days of sales data across two regions (Chennai and Coimbatore), with daily units sold and revenue — used to practice descriptive statistics, grouping, and correlation in `pandas`.

## ✅ Expected Output

- Runnable notebook cell(s)
- Result (summary statistics, region-wise comparison, correlation)
- 2–3 sentence interpretation of the findings

## 🚀 How to Run

1. Clone this repo / download `Statistics_Day1_Exercise.ipynb`
2. Open it in Jupyter Notebook, JupyterLab, VS Code, or Google Colab
3. Run all cells top to bottom (`Cell → Run All`)
4. No external dataset download needed — the sales data is defined directly in the notebook

## 📁 Files

| File | Description |
|---|---|
| `Statistics_Day1_Exercise.ipynb` | Full solution notebook: dataset, descriptive stats, region comparison, correlation, and interpretation |

## 🔑 Approach

Four basic statistical tools are applied to the sales data:
- `.describe()` for overall summary statistics (mean, spread, quartiles)
- `.groupby()` to compare regions on mean, median, and standard deviation
- `.corr()` to check whether units sold and revenue move together
- A simple max lookup to find the best-performing day

## 📈 Result Summary

- **Chennai** sells more on average (52.6 units/day) than **Coimbatore** (36.6), but is also more volatile (higher standard deviation)
- **Correlation** between units sold and revenue is 0.998 — revenue is driven almost entirely by volume, not price changes
- **Best day:** Day 6, Chennai, 90 units, ₹17,800 revenue

## 💡 Key Takeaway

Descriptive and inferential statistics can answer real business questions — what's typical, how consistent performance is, which regions or days stand out, and whether two variables are actually related — all using a handful of `pandas` one-liners and no AI model at all.

---

*Part of the [Statistics 100](https://whatsapp.com/channel/0029VbCHNrh59PwTRYmQsQ0i) daily learning series on WhatsApp.*
