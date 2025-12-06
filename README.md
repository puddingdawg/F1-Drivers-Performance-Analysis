# F1-Drivers-Performance-Analysis
Determining the Best Formula 1 Driver Based on Their Performance and Expertise Using R

# 🏎️ Formula 1 Driver Performance Analysis (2020-2024) By William, Rita and Jayden

### 📌 Project Overview
This research project explores the question: **Who is the best Formula 1 driver in the past five seasons based on their performance and expertise?**

Formula 1 is a sport where car performance often overshadows individual driver skill. To address this, we utilized statistical modeling to isolate individual driver contributions from external factors such as team quality, race-specific conditions, and seasonal variances. By stripping away these advantages, this analysis establishes a fairer basis for evaluating driver performance.

### 📂 Repository Contents
* **`Formula 1 Driver Performance Analysis Research Paper.pdf`**: The complete academic paper detailing the regression analysis, methodology, and results.
* **`Formula 1 Driver Performance Analysis Presentation Slides.pdf`**: A presentation deck summarizing the research question, statistical models, and key visualizations.

### 📊 Methodology & Statistical Models
We constructed a sequence of **9 Regression Models**, progressively adding complexity to improve predictive power and control for omitted variable bias.

#### Statistical Techniques Used:
* **Linear Regression:** To analyze the relationship between independent variables (Experience, Age, Grid Position) and Final Race Position.
* **Logistic Regression (Logit):** To predict binary outcomes, specifically **Podium Finishes** and **Race Completion (DNF)**.
* **Fixed Effects Models:** Applied to control for unobserved but consistent characteristics across four key dimensions:
    * **Driver FE:** Captures inherent talent and decision-making.
    * **Team FE:** Controls for engineering quality and car performance (e.g., Red Bull vs. Haas).
    * **Season FE:** Accounts for regulation changes and yearly competitiveness.
    * **Race FE:** Controls for track-specific characteristics like layout and weather.

#### Model Performance:
* The analysis demonstrated a steady improvement in explanatory power, with **Adjusted R-squared increasing from 0.199 (Model 1) to 0.664 (Model 9)**.
* We assessed model quality using **F-tests** and **RMSE** (Root Mean Squared Error) to prevent overfitting.

### 💡 Key Findings
1.  **Starting Grid is Critical:** Starting grid position consistently remained the strongest predictor of race outcomes across all models.
2.  **Experience vs. Identity:** While experience and age were initially significant, they lost predictive value once Driver Fixed Effects were introduced, suggesting that *who* the driver is matters more than their tenure.
3.  **The "Best" Drivers (2020-2024):** After filtering for drivers who competed in all five seasons to ensure fair comparison, the model identified **Lando Norris** and **George Russell** as the top performers.
4.  **Championship vs. Statistics:** The model identified discrepancies between championship points and statistical "Fixed Effects." For example, while Max Verstappen won the 2024 Championship, our model ranked Fernando Alonso higher in individual impact for that season. This suggests Verstappen's results were heavily bolstered by the Red Bull team advantage, which was absorbed by the Team Fixed Effect in our model.

### 📈 Visualizations
*Please refer to the Presentation Slides for detailed charts.*
* **Driver Fixed Effects:** Visualizing the inherent skill level of drivers (lower coefficient = better performance).
* **Team Advantage:** Showing the significant performance gap between teams like Red Bull Racing and Alfa Romeo.
* **Odds Ratios:** Analysis of the probability of podium finishes based on variables like Fastest Lap.

---
*Created by Group 4 (MGEC45)*
