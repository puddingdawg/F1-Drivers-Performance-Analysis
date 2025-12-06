# F1-Drivers-Performance-Analysis
Determining the Best Formula 1 Driver Based on Their Performance and Expertise Using R
# 🏎️ Formula 1 Driver Performance Analysis (2020-2024)

### 📌 Project Overview
[cite_start]This research project explores the question: **Who is the best Formula 1 driver in the past five seasons based on their performance and expertise?** [cite: 833]

Formula 1 is a sport where car performance often overshadows individual driver skill. [cite_start]To address this, we utilized statistical modeling to isolate individual driver contributions from external factors such as team quality, race-specific conditions, and seasonal variances[cite: 836]. [cite_start]By stripping away these advantages, this analysis establishes a fairer basis for evaluating driver performance[cite: 838].

### 📂 Repository Contents
* [cite_start]**`Formula 1 Driver Performance Analysis Research Paper.pdf`**: The complete academic paper detailing the regression analysis, methodology, and results[cite: 821].
* [cite_start]**`Formula 1 Driver Performance Analysis Presentation Slides.pdf`**: A presentation deck summarizing the research question, statistical models, and key visualizations[cite: 1, 12].

### 📊 Methodology & Statistical Models
[cite_start]We constructed a sequence of **9 Regression Models**, progressively adding complexity to improve predictive power and control for omitted variable bias[cite: 924, 1023].

#### Statistical Techniques Used:
* [cite_start]**Linear Regression:** To analyze the relationship between independent variables (Experience, Age, Grid Position) and Final Race Position[cite: 913].
* [cite_start]**Logistic Regression (Logit):** To predict binary outcomes, specifically **Podium Finishes** and **Race Completion (DNF)**[cite: 918].
* [cite_start]**Fixed Effects Models:** applied to control for unobserved but consistent characteristics across four key dimensions[cite: 925]:
    * [cite_start]**Driver FE:** Captures inherent talent and decision-making[cite: 926].
    * [cite_start]**Team FE:** Controls for engineering quality and car performance (e.g., Red Bull vs. Haas)[cite: 931].
    * [cite_start]**Season FE:** Accounts for regulation changes and yearly competitiveness[cite: 929].
    * [cite_start]**Race FE:** Controls for track-specific characteristics like layout and weather[cite: 927].

#### Model Performance:
* [cite_start]The analysis demonstrated a steady improvement in explanatory power, with **Adjusted R-squared increasing from 0.199 (Model 1) to 0.664 (Model 9)**[cite: 839].
* [cite_start]We assessed model quality using **F-tests** and **RMSE** (Root Mean Squared Error) to prevent overfitting[cite: 940].

### 💡 Key Findings
1.  [cite_start]**Starting Grid is Critical:** Starting grid position consistently remained the strongest predictor of race outcomes across all models[cite: 842].
2.  [cite_start]**Experience vs. Identity:** While experience and age were initially significant, they lost predictive value once Driver Fixed Effects were introduced, suggesting that *who* the driver is matters more than their tenure[cite: 1026, 1029].
3.  [cite_start]**The "Best" Drivers (2020-2024):** After filtering for drivers who competed in all five seasons to ensure fair comparison, the model identified **Lando Norris** and **George Russell** as the top performers[cite: 761, 762].
4.  **Championship vs. Statistics:** The model identified discrepancies between championship points and statistical "Fixed Effects." [cite_start]For example, while Max Verstappen won the 2024 Championship, our model ranked Fernando Alonso higher in individual impact for that season[cite: 1096]. [cite_start]This suggests Verstappen's results were heavily bolstered by the Red Bull team advantage, which was absorbed by the Team Fixed Effect in our model[cite: 1100].

### 📈 Visualizations
*Please refer to the Presentation Slides for detailed charts.*
* [cite_start]**Driver Fixed Effects:** Visualizing the inherent skill level of drivers (lower coefficient = better performance)[cite: 391, 393].
* [cite_start]**Team Advantage:** Showing the significant performance gap between teams like Red Bull Racing and Alfa Romeo[cite: 1193].
* [cite_start]**Odds Ratios:** Analysis of the probability of podium finishes based on variables like Fastest Lap[cite: 667].

---
[cite_start]*Created by Group 4 (MGEC45) [cite: 3]*
