# 2024_Data-wrangling_Final-project

# 🎮 Regional Differences in Online Gaming Performance

This project investigates whether geographic regions influence online gaming behaviors and player performance across genres such as FPS, MOBA, RPG, and more. Inspired by regional dominance observed in games like *League of Legends* (Asia) and *Counter-Strike* (Western regions), the study explores whether culture and cognitive development affect gaming tendencies and skill levels.

## 📌 Objective

To examine if player **location** (e.g., Asia, Europe, USA, Others) correlates with:
- **Preferred game genres**
- **Player performance levels**

## 🧠 Background Motivation

Prior research suggests:
- **Cultural preferences** shape game popularity and commitment (Parshakov et al., 2018; Luo et al., 2024)
- **Cognitive factors** (e.g., attention, reward processing, visuospatial skills) may vary across regions (Goldstein & Volkow, 2002; Powers et al., 2013)

This project combines data science with psychological hypotheses to investigate potential regional effects.

## 📂 Dataset

- Source: Uploaded manually to Google Colab
- File: `online_gaming_behavior_dataset.csv`
- Selected variables:
  - `Location`
  - `GameGenre`
  - `PlayerLevel`

## 🛠️ Tools & Libraries

- `pandas` – Data preprocessing
- `matplotlib`, `seaborn` – Data visualization
- `statsmodels` – Multivariate statistical testing via MANOVA

## 📈 Methodology

1. **Data Cleaning**  
   - Checked for missing values, duplicates, and unusual entries  
   - Validated tidy structure of selected variables

2. **Exploratory Visualizations**
   - Count plots:
     - 📊 Game Genre by Region
     - 📊 Player Level by Region
     - 📊 Player Level by Genre
   - Grouped `PlayerLevel` into `Low`, `Medium`, `High` for better pattern detection
   - Heatmap to visualize % distribution of genres by region

3. **Statistical Testing**
   - Performed MANOVA to test if `Location` significantly affects both `PlayerLevel` and `GameGenre` simultaneously

## 🔍 Results

- No strong visual or statistical evidence was found linking region to genre or skill level
- MANOVA showed **no significant multivariate effect** of region on player behavior (Wilks’ Lambda ≈ 1, *p* > 0.05)

> Conclusion: While cultural perceptions suggest regional gaming preferences, the dataset does not support a statistically significant relationship.

## 📊 Key Plots

- `countplot`: Genre distribution across regions  
- `countplot`: Player levels by region and genre  
- `heatmap`: Genre preferences (% normalized) by location  
- `MANOVA`: Statistical test on `Location ~ GameGenre + PlayerLevel`

## 🧪 Statistical Summary

