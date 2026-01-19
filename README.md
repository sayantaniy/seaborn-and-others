# Seaborn 

## What is Seaborn?

Seaborn is a Python library for **statistical data visualization**. It is built on top of **Matplotlib** and works seamlessly with **Pandas DataFrames**.

---

## Why Seaborn?

* High-level, **beautiful default plots**
* Less code than Matplotlib
* Best for **EDA (Exploratory Data Analysis)**
* Strong support for **statistical plots**

---

## Installation & Import

```bash
pip install seaborn
```

```python
import seaborn as sns
import matplotlib.pyplot as plt
```

---

## Built-in Datasets

```python
sns.get_dataset_names()
df = sns.load_dataset('tips')
```

---

## Basic Plot Structure

```python
sns.plot_type(data=df, x='col1', y='col2')
plt.show()
```

---

## Common Plot Types (Very Important)

### 1. Line Plot

```python
sns.lineplot(data=df, x='day', y='total_bill')
```

### 2. Scatter Plot

```python
sns.scatterplot(data=df, x='total_bill', y='tip')
```

### 3. Bar Plot

```python
sns.barplot(data=df, x='day', y='total_bill')
```

### 4. Histogram

```python
sns.histplot(data=df, x='total_bill')
```

### 5. Box Plot

```python
sns.boxplot(data=df, x='day', y='total_bill')
```

### 6. Violin Plot

```python
sns.violinplot(data=df, x='day', y='total_bill')
```

---

## Categorical Plots

```python
sns.countplot(data=df, x='day')
sns.catplot(data=df, x='day', y='total_bill', kind='bar')
```

---

## Relationship Plots

```python
sns.relplot(data=df, x='total_bill', y='tip', kind='scatter')
```

---

## Distribution Plots

```python
sns.kdeplot(data=df, x='total_bill')
```

---

## Heatmap (Very Important)

```python
sns.heatmap(df.corr(), annot=True)
```

---

## Pair Plot

```python
sns.pairplot(df)
```

---

## Styling & Themes

```python
sns.set_style('darkgrid')
sns.set_theme()
```

---

## Hue Parameter

```python
sns.scatterplot(data=df, x='total_bill', y='tip', hue='sex')
```

---

## Seaborn vs Matplotlib

| Feature  | Seaborn         | Matplotlib   |
| -------- | --------------- | ------------ |
| Level    | High-level      | Low-level    |
| Defaults | Attractive      | Basic        |
| Best for | Statistics, EDA | Full control |

---

## Where Seaborn is Used

* Exploratory Data Analysis
* Statistical Visualization
* ML Feature Analysis

---

## One-Line Summary

**Seaborn = Statistical & Elegant Data Visualization Made Easy
