<div align="center">

```
███████╗███████╗ █████╗ ██████╗  ██████╗ ██████╗ ███╗   ██╗
██╔════╝██╔════╝██╔══██╗██╔══██╗██╔═══██╗██╔══██╗████╗  ██║
███████╗█████╗  ███████║██████╔╝██║   ██║██████╔╝██╔██╗ ██║
╚════██║██╔══╝  ██╔══██║██╔══██╗██║   ██║██╔══██╗██║╚██╗██║
███████║███████╗██║  ██║██████╔╝╚██████╔╝██║  ██║██║ ╚████║
╚══════╝╚══════╝╚═╝  ╚═╝╚═════╝  ╚═════╝ ╚═╝  ╚═╝╚═╝  ╚═══╝
```

### 📊 Seaborn Complete Guide

> A complete hands-on Seaborn repository — from relational & distribution plots to categorical, regression, matrix plots, and multi-panel figures using Python.

<br/>

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0?style=for-the-badge&logo=python&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=python&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=for-the-badge)

</div>

---

## 📌 About

This is my **complete Seaborn learning journal** — covering all major plot types, function classifications, and real-world statistical data visualization using IPL, Iris, Tips, and other datasets.

Built to master:
- Understanding Figure-level vs Axis-level functions
- Relational, Distribution, Categorical, and Regression plots
- Matrix plots — heatmaps and cluster maps
- Multi-panel figures using FacetGrid, PairGrid & JointGrid
- Seaborn's superior aesthetics and built-in statistical estimation

---

## 💡 Why Seaborn?

Seaborn is built on top of Matplotlib, but it takes data visualization several steps further:

| Feature | Matplotlib | Seaborn |
|--------|------------|---------|
| **Abstraction** | Low-level API, verbose | High-level API, concise & readable |
| **Aesthetics** | Basic defaults | Beautiful themes & color palettes out of the box |
| **Statistical Graphs** | Manual computation required | Built-in statistical aggregation & estimation |
| **DataFrame Support** | Limited | Native Pandas DataFrame integration |
| **Plot Variety** | Standard chart types | More graph types including violin, swarm, joint, pair plots |

**Key advantages at a glance:**

- 🧱 **Abstraction layer** — Seaborn wraps Matplotlib's complexity so you write less code for better-looking plots
- 🎨 **Better aesthetics** — Polished default themes (`darkgrid`, `whitegrid`, `ticks`, etc.) and curated color palettes
- 📈 **More graph types** — Specialized plots like `violinplot`, `swarmplot`, `pairplot`, `jointplot`, and `residplot` that Matplotlib doesn't offer natively

> 📖 Official API Reference: [https://seaborn.pydata.org/api.html](https://seaborn.pydata.org/api.html)

---

## 🗺️ Seaborn Roadmap

```
Seaborn
│
├── 🔧 Types of Functions
│   ├── Figure-Level Functions   → Control the whole figure (FacetGrid-based)
│   └── Axis-Level Functions     → Plot on a single Matplotlib Axes
│
└── 📊 Main Plot Categories
    ├── Relational Plots         → Statistical relationships between variables
    ├── Distribution Plots       → Shape & spread of data
    ├── Categorical Plots        → Categorical variable comparisons
    ├── Regression Plots         → Linear model fits & residuals
    ├── Matrix Plots             → Grid-based heatmaps & clustermaps
    └── Multi-Plots              → FacetGrid, PairGrid, JointGrid
```

---

## 🔧 Types of Functions

### Figure-Level Functions
- Operate on the **entire figure** using a `FacetGrid` internally
- Return a `FacetGrid` object (not an Axes)
- Support faceting with `row=`, `col=`, and `hue=` parameters
- Examples: `relplot()`, `displot()`, `catplot()`, `lmplot()`

### Axis-Level Functions
- Operate on a **single Matplotlib Axes**
- Can be embedded inside any `plt.subplots()` layout
- Return an `Axes` object
- Examples: `scatterplot()`, `histplot()`, `boxplot()`, `regplot()`

| | Figure-Level | Axis-Level |
|---|---|---|
| **Returns** | `FacetGrid` | `Axes` |
| **Faceting** | ✅ Built-in | ❌ Manual |
| **Subplot control** | Limited | Full |
| **Best for** | Multi-panel views | Single plot embedding |

---

## 📚 Topics Covered

### 01 — 🟢 Seaborn Basics & Relational Plots

| # | Topic | Description |
|---|-------|-------------|
| 01 | 🔗 Relational Plots — Overview | Statistical relationships, bivariate analysis |
| 02 | 🔵 `scatterplot` | Basic scatter, `hue`, `size`, `style`, `palette` |
| 03 | 📈 `lineplot` | Trend visualization, confidence intervals, time-series |
| 04 | 🌐 `relplot` | Figure-level wrapper for scatter & line with faceting |

### 02 — 📦 Distribution Plots

| # | Topic | Description |
|---|-------|-------------|
| 05 | 📊 `histplot` | Univariate & bivariate histograms, KDE overlay |
| 06 | 〰️ `kdeplot` | Kernel Density Estimation — 1D & 2D |
| 07 | 🎻 `ecdfplot` | Empirical Cumulative Distribution Function |
| 08 | 🌊 `displot` | Figure-level distribution wrapper with `kind` parameter |
| 09 | 🔔 `rugplot` | Marginal tick marks along axes |

### 03 — 🟣 Categorical Plots

| # | Topic | Description |
|---|-------|-------------|
| **Categorical Scatter** | | |
| 10 | 🟡 `stripplot` | Jittered categorical scatter plot |
| 11 | 🐝 `swarmplot` | Non-overlapping categorical scatter |
| **Categorical Distribution** | | |
| 12 | 📦 `boxplot` | Quartiles, median, and outliers |
| 13 | 🎻 `violinplot` | Distribution shape combined with box summary |
| **Categorical Estimate** | | |
| 14 | 📊 `barplot` | Mean (or custom estimator) with confidence intervals |
| 15 | 🔵 `pointplot` | Estimate with error bars, connects groups with lines |
| 16 | 🔢 `countplot` | Frequency count of categorical values |
| **Figure-Level** | | |
| 17 | 🗂️ `catplot` | Unified figure-level API for all categorical plots |

### 04 — 🔵 Advanced Seaborn

| # | Topic | Description |
|---|-------|-------------|
| 18 | 🪟 Facet & `FacetGrid` | Manual multi-panel layouts with `map()` |
| 19 | 🔗 `pairplot` | All pairwise variable relationships in one grid |
| 20 | 🧩 `PairGrid` | Customizable version of pairplot |
| 21 | 🤝 `jointplot` | Bivariate + marginal distribution in one figure |
| 22 | 🔲 `JointGrid` | Manual customization of joint + marginal plots |
| 23 | 📐 Regression — `regplot` | Axis-level linear regression with confidence band |
| 24 | 📐 Regression — `lmplot` | Figure-level regression, supports faceting |
| 25 | 〰️ `residplot` | Residuals from a linear fit — check model assumptions |
| 26 | 🔥 `heatmap` | Matrix visualization — correlation, pivot tables |
| 27 | 🌲 `clustermap` | Hierarchically clustered heatmap |

---

## 🧩 Plot Classification at a Glance

### 1. 🔗 Relational Plots
> **Purpose:** Visualize the statistical relationship between two or more numerical variables (Bivariate Analysis)

```
relplot()              ← Figure-level wrapper
├── scatterplot()      ← Axis-level
└── lineplot()         ← Axis-level
```

### 2. 📦 Distribution Plots
> **Purpose:** Understand the distribution, spread, and shape of univariate or bivariate data

```
displot()              ← Figure-level wrapper
├── histplot()         ← Axis-level
├── kdeplot()          ← Axis-level
├── ecdfplot()         ← Axis-level
└── rugplot()          ← Axis-level (marginal ticks)
```

### 3. 🟣 Categorical Plots
> **Purpose:** Compare distributions or estimates across categorical groups

```
catplot()              ← Figure-level wrapper
│
├── Categorical Scatter
│   ├── stripplot()    ← Jittered points per category
│   └── swarmplot()    ← Non-overlapping points
│
├── Categorical Distribution
│   ├── boxplot()      ← Quartiles + outliers
│   └── violinplot()   ← KDE + box summary
│
└── Categorical Estimate (Central Tendency)
    ├── barplot()      ← Mean with CI
    ├── pointplot()    ← Estimate connected across groups
    └── countplot()    ← Frequency per category
```

### 4. 📐 Regression Plots
> **Purpose:** Fit and visualize linear relationships between variables

```
├── regplot()          ← Axis-level; simple and flexible
├── lmplot()           ← Figure-level; supports hue/col/row faceting
└── residplot()        ← Axis-level; residuals from linear fit
```

### 5. 🔥 Matrix Plots
> **Purpose:** Visualize data arranged in a grid (correlation matrices, pivot tables)

```
├── heatmap()          ← Color-encoded matrix cells
└── clustermap()       ← Heatmap with hierarchical clustering
```

### 6. 🪟 Multi-Plots (Grid Figures)
> **Purpose:** Build complex multi-panel layouts for deeper comparative analysis

```
├── FacetGrid          ← Custom multi-panel using any plot function
├── pairplot()         ← Auto pairwise plots for all variables
├── PairGrid           ← Manual version of pairplot
├── jointplot()        ← Bivariate plot + marginal distributions
└── JointGrid          ← Manual version of jointplot
```

---

## 🗂️ Repository Structure

```bash
seaborn-complete-guide/
│
├── 📓 01-seaborn.ipynb       # Basics, Relational & Distribution plots
├── 📓 02-seaborn.ipynb       # Categorical, Regression, Matrix & Multi-plots
└── 📄 README.md
```

---

## ⚙️ How to Run

```bash
# 1. Clone the repository
git clone https://github.com/amit-0333/seaborn-complete-guide.git

# 2. Navigate into the folder
cd seaborn-complete-guide

# 3. Install dependencies
pip install seaborn matplotlib numpy pandas jupyter

# 4. Launch Jupyter Notebook
jupyter notebook

# Or open directly in Google Colab
```

---

## 🧪 Real-World Datasets Used

| Dataset | Used For |
|---------|----------|
| `iris.csv` | Pairplot, scatter — species classification by petal/sepal |
| `tips.csv` | Categorical plots — tip vs day/sex/time |
| `titanic.csv` | Barplot, countplot — survival rate by class/gender |
| `flights.csv` | Heatmap — monthly passenger volume over years |
| `fmri.csv` | Lineplot — brain signal over time by region & event |
| `penguins.csv` | Pairplot, violin — multi-species comparison |
| `tips` (seaborn built-in) | Regression, jointplot, lmplot |

---

## 🧩 My Approach to Every Plot

```
1. 📖 Identify the data type — numerical, categorical, or mixed
2. 🔨 Choose Figure-level or Axis-level function based on layout needs
3. 🎨 Customize — hue, palette, style, size, legend
4. 📊 Apply to a real dataset with meaningful variables
5. ✅ Document the use case — univariate / bivariate / categorical / regression
```

---

## 🎯 Learning Goals

- [x] Understand Figure-level vs Axis-level function distinction
- [x] Build relational plots — scatterplot, lineplot, relplot
- [x] Explore distribution plots — histplot, kdeplot, ecdfplot, displot
- [x] Create categorical scatter plots — stripplot, swarmplot
- [x] Build categorical distribution plots — boxplot, violinplot
- [x] Use categorical estimate plots — barplot, pointplot, countplot
- [x] Use catplot as unified figure-level categorical interface
- [x] Build FacetGrid and faceted multi-panel views
- [x] Use pairplot & PairGrid for multivariate analysis
- [x] Use jointplot & JointGrid for bivariate + marginal views
- [x] Fit regression lines with regplot, lmplot, and residplot
- [x] Build heatmaps and clustermaps for matrix data
- [ ] Deep dive into custom theming and color palettes
- [ ] Build a complete EDA case study using Seaborn

---

## 🛠️ Tech Stack

- 🐍 **Python** — Core programming language
- 🎨 **Seaborn** — Primary statistical visualization library
- 📊 **Matplotlib** — Underlying rendering engine
- 🔢 **NumPy** — Numerical arrays and operations
- 🐼 **Pandas** — DataFrame-based data handling
- 📓 **Jupyter / Google Colab** — Interactive notebooks

---

## 🙏 Credits & Acknowledgement

> This repository is built while learning from **[Campus X](https://www.youtube.com/@campusx-official)** — an amazing free Data Science education channel.
> Notebooks are based on class materials from Campus X. All credit for the curriculum and teaching goes to them.
> I've added my own notes, practice, and experiments on top of the class content.

---

## 👨‍💻 Author

**Amit Kumar**

[![GitHub](https://img.shields.io/badge/GitHub-amit--0333-181717?style=flat&logo=github)](https://github.com/amit-0333)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Amit%20Kumar-0077B5?style=flat&logo=linkedin)](https://www.linkedin.com/in/amit-kumar-a62a3640a/)
[![Kaggle](https://img.shields.io/badge/Kaggle-amitkumar038975-20BEFF?style=flat&logo=kaggle)](https://www.kaggle.com/amitkumar038975)

---

<div align="center">

> 📝 *This repository is continuously updated as I learn new visualization techniques.*

⭐ **Star this repo if it helped you learn Seaborn!**

</div>
