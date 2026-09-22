## 📊 Phase 2: Exploratory Data Analysis, Feature Engineering & Database Integration

In this phase, we processed the Olist Brazilian E-Commerce dataset, engineered predictive features for delivery delays, stored data in a local database, and prepared model artifacts.

### 🗄️ Database & Docker Setup
- **PostgreSQL Database:** The structured Olist relational tables are hosted and managed locally using **Docker**, ensuring a consistent and reproducible database environment.
- **Data Pipeline:** Data is extracted from PostgreSQL, processed using Pandas, and transformed through modular preprocessing steps.

### 🔍 Key Steps Implemented in Phase 2:
1. **Data Joining & Cleaning (`1_Read_Join.ipynb`):** Merged multiple Olist tables (orders, customers, items, sellers, and geolocation).
2. **Target Labeling (`2_Create_Labels.ipynb`):** Defined the binary target variable `is_late` by comparing estimated delivery dates with actual delivery dates.
3. **Data Splitting (`3_Split_Data.ipynb`):** Implemented strict train/test/validation splits to prevent data leakage.
4. **Exploratory Data Analysis (`4_EDA.ipynb`):** Visualized key distributions (e.g., late vs. on-time deliveries, freight value impacts, and geographic delays).
5. **Feature Engineering (`5_Feature_Engineering.ipynb`):** Extracted time-based features, delivery duration metrics, and aggregated order attributes.
6. **Model Training & Validation (`6_Validation.ipynb`):** Trained a baseline Random Forest classifier and evaluated performance using robust metrics.