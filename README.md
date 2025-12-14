# 🤰 Mental Health in Pregnancy During COVID-19

## 📌 Project Overview
This project analyzes the impact of the **COVID-19 pandemic** on the mental health of pregnant women. By examining a dataset containing demographic information, medical history, and psychometric scores (EPDS for depression and PROMIS for anxiety), this analysis aims to uncover correlations between socioeconomic factors, maternal age, and mental well-being during a global crisis.

The study highlights how factors like **income inequality** and **maternal age** significantly influenced perceived threats to life and baby safety during the pandemic.

## 📂 Dataset Description
The dataset consists of survey responses from pregnant women during the COVID-19 pandemic. Key features include:

| Feature | Description |
| :--- | :--- |
| **Maternal_Age** | Age of the mother (years). |
| **Household_Income** | Total household income (2019). |
| **Maternal_Education** | Highest education level completed (1-7 scale). |
| **EPDS** | *Edinburgh Postnatal Depression Scale* score (higher = more severe). |
| **PROMIS_Anxiety** | Anxiety score (7-35; higher = greater anxiety). |
| **GAbirth** | Gestational age at birth (weeks). |
| **Delivery_Mode** | Vaginal or Caesarean-section. |
| **Threaten_Life** | Perceived danger to own life due to COVID-19 (0-100). |
| **Threaten_Baby_Danger** | Perceived risk to unborn baby due to COVID-19 (0-100). |
| **NICU_Stay** | Whether the newborn required intensive care (Yes/No). |

## 🛠️ Tech Stack
* **Language:** Python 3.x
* **Data Manipulation:** Pandas, NumPy
* **Visualization:** Matplotlib, Seaborn, Plotly Express
* **Environment:** Jupyter Notebook / Google Colab

## 📊 Methodology
1.  **Data Cleaning**:
    * Removed irrelevant columns (`OSF_ID`, `Language`).
    * Handled missing values by dropping null rows in critical psychometric columns.
    * Converted `Gestational_Age_At_Birth` from weeks to months for better readability.
2.  **Feature Engineering**:
    * Categorized `Birth_Weight` and `Birth_Length` into **"Healthy"** or **"Unhealthy"** classes based on medical standards.
3.  **Exploratory Data Analysis (EDA)**:
    * **Univariate Analysis**: Studied distributions of income, education, and delivery modes.
    * **Bivariate Analysis**: Explored relationships between Income vs. Anxiety, and Age vs. Depression (EPDS).
    * **Probabilistic Analysis**: Calculated the conditional probability of high anxiety given high/low depression scores.

## 💡 Key Insights
* **Socioeconomic Impact**: Individuals living below the poverty line (<$70k) were significantly more susceptible to high Anxiety and Depression. Nearly **70%** of this group showed elevated symptoms.
* **Income & Mental Health**: There is a strong positive correlation between income and mental well-being. High-income individuals had only a **33%** chance of being diagnosed with high anxiety/depression.
* **Universal Concern for Infants**: While concern for personal safety varied by income, worry for the **newborn's safety** was universally high across all demographics.
* **Maternal Age Vulnerability**: Women aged **43+** were found to be more worried about the impact of COVID-19, which may correlate with higher anxiety and post-pregnancy depression in this group. Conversely, women aged 25-42 reported lower worry levels.
* **Comorbidity**: There is an **81% likelihood** that women with high EPDS scores also experience high anxiety, compared to just 14% for those with low EPDS scores.
* **C-Section Rates**: A notable increase (13%) in C-section deliveries was observed in women over the age of 38.

## 📈 Visualizations
The notebook includes interactive and static charts such as:
* *Distribution of Anxiety Scores by Household Income* (Plotly Histogram).
* *Distribution of Anxiety Scores by Maternal Education* (Plotly Histogram).
* *Grouped Analysis of Perceived Threats to Baby by Income*.

## 🚀 How to Run
1.  Clone the repository:
    ```bash
    git clone https://github.com/siddharthjha123/Mental-Health-In-Pregnancy-During-Covid-EDA.git
    ```
2.  Install dependencies:
    ```bash
    pip install pandas numpy seaborn matplotlib plotly
    ```
3.  Open the notebook:
    ```bash
    jupyter notebook "Mental Health in Pregnancy During Covid - 19.ipynb"
    ```

## 🤝 Contributing
Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/).
