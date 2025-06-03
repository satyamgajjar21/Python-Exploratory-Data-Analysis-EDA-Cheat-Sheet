<h1 align="center">Exploratory Data Analysis (EDA) Cheat Sheet</h1>
<p align="center">
  A quick reference for the most common pandas / Matplotlib / Seaborn /
  SciPy commands you need when exploring a new data set.
</p>

---

## 📑 Table of Contents
1. [Correlation](#correlation)
2. [Visualization](#visualization)
3. [Grouping & Pivot Tables](#grouping--pivot-tables)
4. [Heatmaps (pcolor)](#heatmaps-pcolor)
5. [Statistical Tests](#statistical-tests)

> **Tip:** All examples assume your DataFrame is called **`df`**.

---

## Correlation

| Task | Description | Code Snippet |
|------|-------------|-------------|
| **Full dataframe correlation** | Create a correlation matrix for every numeric column. | ```python df.corr() ``` |
| **Selected attributes** | Correlation matrix for chosen columns. | ```python df[['col1', 'col2']].corr() ``` |

---

## Visualization

### Scatter Plot
```python
import matplotlib.pyplot as plt

plt.scatter(df['col_x'], df['col_y'])
plt.xlabel('col_x')
plt.ylabel('col_y')
plt.show()
