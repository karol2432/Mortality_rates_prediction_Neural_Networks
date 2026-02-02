# Mortality Rate Analysis in Poland (2016–2024)

This repository contains an analysis of mortality rates across Polish voivodeships from 2016 to 2024, including descriptive statistics, gender differences, and autocorrelation analysis.

---

## 1. Descriptive Analysis

**Objective:** Examine mortality trends across all 16 voivodeships and monthly distribution for Małopolskie.

**Observations:**
- Sharp increase in 2020–2021 due to COVID-19 pandemic.
- Post-2022: decreased and stabilized, but still above pre-pandemic levels.
- Highest mortality: Łódzkie, Świętokrzyskie, Śląskie, Lubelskie.
- Lowest mortality: Małopolskie, Pomorskie, Wielkopolskie, Podkarpackie.
- Seasonal pattern: higher in autumn-winter, lower in spring-summer.

**Figures:**
- ![Fig. 1.1 – Annual mortality trends (2016–2024) for all voivodeships](path/to/fig1_1.png)
- ![Fig. 1.2 – Monthly mortality distribution for Małopolskie](path/to/fig1_2.png)

---

## 2. Statistical Tests

**Gender differences:**
- OLS regression shows significant differences between men and women in all regions and age groups.

**Changes over time:**
- Friedman test identifies which regions were significantly affected by the pandemic.

**Key Results:**
- **Age 0–64:** median male/female ratio >2 in all regions; significant difference in Podlaskie.
- **Age 65+:** male mortality still higher, greater fluctuations; some regions show no significant differences.

**Figures:**
- ![Fig. 1.3 – Boxplot M/F ratio (0–64)](path/to/fig1_3.png)
- ![Fig. 1.4 – Boxplot M/F ratio (65+)](path/to/fig1_4.png)

---

## 3. Autocorrelation Analysis (ACF & PACF)

**Purpose:** Detect temporal dependencies in mortality data.

**Findings (Małopolskie):**
- Annual seasonality (significant ACF peak at 12 months).
- PACF: lags 1, 2, and 12 most relevant; longer lags negligible.

**Implication:** Lagged variables can be used as input in predictive models.

**Figures:**
- ![Fig. 1.5 – ACF & PACF plots for Małopolskie](path/to/fig1_5.png)

---

## Usage

- Replace `path/to/...` with your actual plot file paths.
- The README focuses on observations and key insights; for methodology details, refer to the main report.

---

## References

1. [Author et al., Year] – Original data sources and statistical references.
2. [Newey-West, HAC estimator references]
3. [Other sources if needed]
