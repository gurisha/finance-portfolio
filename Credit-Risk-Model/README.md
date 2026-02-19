# Credit Risk Scoring & Analysis

## Objective

To design and implement a structured credit risk screening framework to evaluate a portfolio of consumer loan applications. The model aims to support disciplined initial credit decisioning, differentiate risk across applicants, and provide portfolio-level visibility into approval quality and risk concentration.

## Data Used

The analysis utilizes applicant-level financial and credit attributes, including:

* Annual income and employment history
* Existing debt and monthly debt obligations
* Loan amount and term
* Credit score and score band classification
* Past defaults, delinquencies, and bankruptcy indicators

Derived risk metrics such as Debt-to-Income (DTI) and Loan-to-Income ratios were calculated to standardize risk exposure across applicants.

## Analysis Performed

A weighted credit risk scorecard was developed using five primary risk drivers:

* Credit Score
* Debt-to-Income (DTI)
* Employment Stability
* Past Defaults
* Delinquency History

Each factor was scored and aggregated into a composite Risk Score, mapped into defined risk tiers (Low, Medium, High, Very High).

In addition to score-based outcomes, structured policy overrides were implemented for material risk events (e.g., bankruptcy, multiple delinquencies, elevated DTI), ensuring alignment with conservative underwriting standards.

A portfolio summary was constructed to assess approval rates, average risk score, and the proportion of higher-risk exposure.

## Key Findings

* The portfolio skews predominantly low risk, supporting a stable overall approval rate.
* Elevated DTI emerged as a primary driver of manual review and enhanced scrutiny.
* Policy override logic appropriately identified and excluded structurally high-risk cases (e.g., bankruptcy and severe delinquency patterns).
* The scorecard effectively differentiates between low-risk and higher-risk applicants while preserving transparency in decision logic.

## Business Implications

The framework demonstrates a disciplined, explainable approach to credit decisioning that balances growth and risk control.

By combining quantitative scoring with policy governance, the model supports:

* Consistent underwriting standards
* Controlled exposure to high-risk borrowers
* Portfolio-level visibility for senior leadership
* Scalable risk assessment processes

This approach can be extended to incorporate pricing strategy, collateral evaluation, and macroeconomic stress considerations in a production environment.
