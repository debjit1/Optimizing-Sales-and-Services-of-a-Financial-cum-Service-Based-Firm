# Maximizing Sales and Optimizing Services of a Financial cum Service-Based Firm

## BDM Capstone Project

A data-driven Business Data Management (BDM) capstone project focused on
improving mutual fund sales, increasing Assets Under Management (AUM),
and aligning client portfolios with their risk profiles for **Unique
Enterprise**, a financial and service-based firm.

**Author:** Debjit Mondal\
**Program:** IIT Madras BS Degree Program\
**Project:** BDM Capstone Project

------------------------------------------------------------------------

## 📌 Project Overview

Unique Enterprise primarily operates in mutual fund sales and also
provides services such as insurance, income tax return (ITR) filing,
money transfers, and air/railway ticket booking.

The project addresses two major business challenges:

1.  **Maximizing profit from mutual fund sales** by replacing ad-hoc
    fund recommendations with a structured, data-driven approach.
2.  **Aligning client portfolios with risk profiles** through systematic
    risk assessment and portfolio analysis.

The project uses historical transaction data, mutual fund returns, NAV
data, and client risk-assessment responses to generate actionable
insights for sales and advisory decisions.

------------------------------------------------------------------------

## 🎯 Objectives

-   Analyze quarterly mutual fund investment and redemption trends.
-   Track and understand Assets Under Management (AUM) movement.
-   Assess client risk tolerance using a structured questionnaire.
-   Categorize clients into Low, Medium, and High risk profiles.
-   Categorize mutual funds using historical return volatility.
-   Use **K-Means clustering** to group mutual funds into risk
    categories.
-   Analyze the existing risk exposure of client portfolios.
-   Identify top-performing mutual funds within different risk
    categories and time horizons.
-   Provide data-driven recommendations to improve AUM, customer
    retention, and profitability.

------------------------------------------------------------------------

## 📊 Data Used

The analysis was based on business data covering approximately **March
2022 to February/March 2025**, including:

### 1. Mutual Fund Transaction Data

-   New investment/purchase transactions
-   Redemption transactions
-   Scheme information
-   NAV
-   Units
-   Transaction amount
-   Investor and portfolio information

The purchase dataset contains **5,365 records**, while the redemption
dataset contains **261 records**.

### 2. Historical Mutual Fund Returns

Historical returns were analyzed over multiple time horizons:

-   6 months
-   1 year
-   5 years
-   10 years
-   15 years
-   Inception date
-   Expense ratio

The processed historical-return dataset contains **1,208 records**.

### 3. Quarterwise NAV Data

Quarterly NAV data was consolidated and used to calculate AUM and
analyze investment value over time.

The processed dataset contains approximately **90,889 records** covering
quarterly data from March 2022 to March 2025.

### 4. Client Risk Assessment

A risk-assessment questionnaire was developed in consultation with the
business owner. Responses were collected using Google Forms and printed
forms.

At the time of the final analysis, **15 clients** had completed the
assessment.

------------------------------------------------------------------------

## 🔬 Methodology

### Data Preprocessing

Transaction records were separated into purchase and redemption
datasets. Historical NAV data originally supplied in DOCX format was
processed and consolidated into spreadsheet format.

For AUM estimation, units held as of **28 February 2025** were valued
using the relevant Q1-2025 NAV data.

### Investment and Redemption Trend Analysis

Quarterly investment inflows and redemption outflows were analyzed using
spreadsheet-based grouping and Pivot Tables.

This helped identify:

-   Growth patterns
-   Major inflow periods
-   Redemption spikes
-   Effects of business campaigns

### AUM Analysis

AUM was calculated using the number of units held and the applicable NAV
for each mutual fund at different time points.

Since the firm's mutual fund earnings are linked to AUM, tracking AUM is
important for understanding potential revenue growth.

### Client Risk Assessment

Clients were classified using the risk-assessment score:

  Risk Category     Risk Score
  --------------- ------------
  High Risk              \> 67
  Medium Risk           51--67
  Low Risk                ≤ 50

### Mutual Fund Risk Categorization

Historical return volatility was measured using standard deviation.

**K-Means clustering**, implemented using scikit-learn, was then used to
divide mutual funds into:

-   Low Risk
-   Moderate Risk
-   High Risk

### Portfolio Risk Exposure

Existing client portfolios were evaluated against the risk categories of
the funds they held.

Clients were classified according to the category containing the
majority of their investment exposure:

-   Aggressive / High-risk exposure
-   Moderate-risk exposure
-   Low-risk exposure

### Fund Performance Ranking

Mutual funds were ranked within each risk category using average returns
across different investment horizons.

This produced lists of top-performing funds that can support more
personalized recommendations.

------------------------------------------------------------------------

## 🛠️ Tools & Technologies

-   **Microsoft Excel / Spreadsheets** --- data organization, filtering,
    Pivot Tables, calculations, and charts
-   **Python** --- data analysis and processing
-   **Pandas** --- data wrangling and exploratory analysis
-   **NumPy** --- numerical computation
-   **Scikit-learn** --- K-Means clustering and risk categorization
-   **Matplotlib** --- data visualization
-   **Google Colab** --- Python-based analysis environment
-   **Google Forms** --- client risk assessment data collection

------------------------------------------------------------------------

## 📈 Key Findings

### Investment Trends

Two major business campaigns produced noticeable increases in mutual
fund inflows. The largest investment period occurred around Q1 2024,
when investments approached **₹4 crore**.

The analysis indicates that structured institutional/corporate campaigns
can be an effective way to attract new investors.

### Redemption Trends

Redemption activity increased sharply around Q4 2023 and Q1 2024, with
redemption values exceeding **₹1.8 crore** in both quarters.

A major portion of this spike was attributed to withdrawals by two
high-value investors, demonstrating the effect that a small number of
large clients can have on overall redemption levels.

### AUM Trends

AUM increased gradually from Q3 2022 through Q3 2023, followed by a
strong increase during 2024. The analysis associated major AUM growth
with successful investment campaigns.

### Client Risk Assessment

Among the 15 assessed clients:

-   **8** were categorized as Medium Risk
-   **6** were categorized as High Risk
-   **1** was categorized as Low Risk

The limited survey participation means these results should not be
treated as representative of the entire client base.

### Mutual Fund Risk Classification

K-Means clustering categorized the available mutual fund schemes into:

-   **716 Low-risk funds**
-   **356 Moderate-risk funds**
-   **136 High-risk funds**

### Existing AUM Risk Distribution

The final report found that AUM was concentrated mainly in moderate- and
high-risk schemes, with only a small proportion in low-risk schemes.

The reported risk distribution was approximately:

-   **52.08% Moderate Risk**
-   **46.14% High Risk**
-   **1.8% Low Risk**

### Performance by Investment Horizon

The analysis found that:

-   Gold ETF funds performed strongly over shorter horizons.
-   Five-year top-performing funds were predominantly equity-based and
    high-risk.
-   High-risk equity funds dominated the long-term 10- and 15-year
    performance rankings.
-   Moderate-risk funds also provided comparatively balanced long-term
    growth.

These observations are intended to support risk- and horizon-based
recommendations rather than blanket fund recommendations.

------------------------------------------------------------------------

## 💡 Recommendations

Based on the analysis, the project recommends:

1.  **Conduct regular institutional/corporate campaigns** because
    previous campaigns generated strong investment inflows.
2.  **Monitor high-value investors closely** to reduce the impact of
    large redemptions on AUM.
3.  **Perform risk assessments for new clients** before making
    investment recommendations.
4.  **Periodically reassess existing clients** as their financial goals
    and risk tolerance may change.
5.  **Identify portfolio-risk mismatches** and suggest suitable
    rebalancing where appropriate.
6.  **Use investment horizon together with risk appetite** when
    selecting funds.
7.  **Consider low-risk funds for shorter-term needs, moderate-risk
    funds for medium-term goals, and higher-risk funds for suitable
    long-term investors.**
8.  **Diversify across risk categories** according to the client's
    objectives and risk appetite.
9.  **Regularly monitor portfolios and market conditions** so that
    recommendations remain aligned with client goals.

-------------------------------------------------------
------------------------------------------------------------------------

## 🔐 Data Privacy

The underlying business data contains investor and transaction-related
information. Sensitive or personally identifiable business/client data are not uploaded for privacy concern
------------------------------------------------------------------------

## 📚 Project Reports

The project was developed through proposal, midterm, and final-report
stages.

-   **Proposal:** Optimizing Sales and Services of a Financial cum
    Service-Based Firm
-   **Midterm Report:** Maximizing Sales and Optimizing Services of a
    Financial cum Service-Based Firm
-   **Final Report:** Maximizing Sales and Optimizing Services of a
    Financial cum Service-Based Firm

The final analysis builds on the earlier problem definition, data
collection plan, and analytical approach.

------------------------------------------------------------------------

## ⚠️ Limitations

-   The client risk-assessment sample was limited to 15 respondents.
-   Detailed commission statements were not disclosed by the business
    because of its partnering agency's policy.
-   AUM estimation assumes that no transactions occurred after 28
    February 2025 because later transaction/NAV data was unavailable.
-   Mutual fund performance varies with market conditions; historical
    performance should not be treated as a guarantee of future returns.
-   K-Means categorization is an analytical classification based on
    return volatility and should be used as a decision-support tool
    rather than as a substitute for professional financial advice.

------------------------------------------------------------------------

## 🎓 Academic Context

This project was completed as part of the **BDM Capstone Project** under
the IIT Madras BS Degree Program.

The project applies data management, descriptive analysis, statistical
analysis, visualization, and machine-learning-based clustering to a
real-world business problem.

------------------------------------------------------------------------

## 👤 Author

**Debjit Mondal**\
IIT Madras BS Degree Program\
BDM Capstone Project

------------------------------------------------------------------------

## 📌 Disclaimer

This repository documents an academic business-data-analysis project.
The analysis and recommendations are based on the data and assumptions
available during the project period and should not be interpreted as
personalized financial advice or a guarantee of investment performance.
