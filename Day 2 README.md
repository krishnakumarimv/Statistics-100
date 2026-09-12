# Statistics 100 — Day 2 / 365

### 📊 Why Statistics Matters

Part of the [Statistics 100](https://github.com/krishnakumarimv/Statistics-100) series — one simple statistics idea a day, no jargon, no math anxiety.

## Topic

You don't need to be a data scientist to use statistics — it's already helping you make decisions every day (delivery time estimates, batting averages, rain forecasts). Today's exercise puts that idea into practice by comparing two datasets using summary statistics.

## Exercise

**Compare two business groups using summary statistics.**

- **Dataset:** Synthetic Sales — 30 days of daily sales (₹ thousands) for two stores, generated with `numpy.random.normal`.
- **Task:** Compute mean, median, and standard deviation for each group, and compare not just the averages but the spread.
- **Hint:** Two groups can have similar means and still behave very differently — the standard deviation tells you which one is more predictable.

## How to run

```bash
pip install numpy matplotlib
jupyter notebook day2_why_statistics_matters.ipynb
```

Run all cells top to bottom. The notebook regenerates the same dataset every time (`np.random.seed(42)`), so your output will match the result below exactly.

## Result

| Metric   | Group A | Group B |
|----------|---------|---------|
| Mean     | 53.5    | 57.8    |
| Median   | 53.1    | 58.8    |
| Std Dev  | 7.2     | 16.8    |
| Min      | 39.7    | 24.7    |
| Max      | 67.6    | 93.3    |

## Interpretation

Group B earns more on average, but its standard deviation is over twice Group A's — meaning its daily sales swing wildly (from ₹24.7k to ₹93.3k) while Group A stays steady (₹39.7k–₹67.6k). If you only looked at the mean, you'd think Group B is simply "better." Looking at spread tells the real story: Group A is the reliable performer, Group B is the volatile one.

## Files

- `day2_why_statistics_matters.ipynb` — full runnable notebook (code + result + interpretation + a boxplot visual)

---

**Tomorrow (Day 3):** *Descriptive vs Inferential Statistics* 👀
