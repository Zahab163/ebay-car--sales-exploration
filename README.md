# Exploring eBay Car Sales Data  
*Dataquest Live Session Project (Guided by Anna Strahl, Completed by Zahabia Ahmed)*

This repository contains the code and analysis from a **Google Colab notebook** developed during a **Dataquest Live Session** guided by **Anna Strahl**.  
Half of the project was completed in the live session, and the remaining work — including deeper cleaning, exploratory analysis, and predictive modeling — was completed independently by me.  

The original notebook can be accessed here: [Colab Project Link](https://colab.research.google.com/drive/16MAu5VYCI8FQxmIhf1F5kafriPyd37PH?usp=sharing)

---

## 📊 Project Summary

This project explores a dataset of used car listings scraped from **eBay Kleinanzeigen**, a German classifieds site. The goal was to clean, transform, and analyze the data, mimicking the role of a data analyst for a used car classifieds service.

### 🔑 Key Steps
- **Data Cleaning**:  
  - Dropped irrelevant columns (`num_photos`, `seller`, `offer_type`).  
  - Cleaned `price` and `odometer` columns, converted to integers, renamed `odometer_km`.  
  - Filtered outliers in `price` (kept values between 100 and 3,895,000).  
  - Cleaned `registration_year` (kept 1900–2016).  
  - Filled missing values in `unrepaired_damage` with `'nicht_angegeben'`.  

- **Exploratory Data Analysis (EDA)**:  
  - **Brand Analysis**: Volkswagen, BMW, Opel, Mercedes-Benz, Audi, and Ford were most common. Luxury brands retained higher value despite similar mileage.  
  - **Mileage-Price Patterns**: Clear inverse relationship — lower mileage cars had higher average prices.  
  - **Damage Impact**: Cars without damage averaged €7,332, while damaged cars dropped to €2,365, showing a strong penalty for unrepaired or ambiguous damage.  

---

## 🔮 Discoveries & Insights
Through my extended work beyond the live session, I discovered:  
- **Mileage strongly drives price** — cars under 50k km averaged nearly triple the price of those above 100k km.  
- **Luxury brands retain value better** — Audi, BMW, and Mercedes-Benz showed higher average prices despite similar mileage.  
- **Damage status is critical** — unrepaired damage or ambiguous descriptions significantly reduce car value.  
- **Predictive modeling is feasible** — cleaned features like mileage, age, and brand can be used to forecast car prices with regression models.

---

## 📈 Next Steps
To build on this project, I plan to:  
- Train and compare **five predictive models** (Linear Regression, Decision Tree, Random Forest, Gradient Boosting, SVR).  
- Visualize **predicted vs. actual prices** for each model.  
- Analyze **feature importance** for tree-based models.  
- Add **visualizations**: mileage vs. price, brand value retention, damage impact, and model comparison charts.  

---

## 📑 Repository Contents
- `notebook.ipynb` → Main Colab notebook with code and explanations  
- `README.md` → Documentation of the project  

---

## 📚 Acknowledgments
Special thanks to **Anna Strahl** and **Dataquest** for the live session guidance on data cleaning and EDA. Completing the project independently helped me deepen my skills in data cleaning, EDA, and machine learning.

---

## 📜 License
This project is for educational purposes. Feel free to fork and adapt for your own learning journey.
