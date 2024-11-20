# Simulated IFRS 17 Solution Pipeline

This repository provides a Python-based simulation pipeline for implementing an International Financial Reporting Standard (IFRS) 17 solution. It uses synthetic data to model insurance policy cash flows, calculate liabilities, and visualize financial metrics. The solution is designed to be a comprehensive framework for understanding IFRS 17 concepts and testing actuarial models.

---

## Features

- **Synthetic Data Generation**: Creates realistic insurance policy data, including premiums, claims, and various expenses.
- **Cash Flow Modeling**: Calculates present value for premiums, claims, and directly attributable expenses.
- **Contractual Service Margin (CSM)**: Computes the unearned profit for an insurance contract.
- **Risk Adjustment Calculation**: Provides a simplified approach to calculate risk adjustments over the coverage period.
- **Liability Modeling**: Computes total liabilities by combining cash flows, risk adjustments, and CSM.
- **Financial Reporting**: Summarizes key metrics for financial reporting.
- **Visualization**: Includes histograms and other visual tools to analyze the distribution of liabilities.

---

## Key Requirements of IFRS 17

1. **Scope**  
   - Applies to all insurance contracts (including reinsurance).  
   - Covers investment contracts with discretionary participation features if issued by insurance entities.  
   - Excludes certain contracts, such as product warranties issued by manufacturers and financial guarantee contracts covered under IFRS 9.

2. **Measurement Models**  
   IFRS 17 introduces three approaches for measuring insurance contract liabilities:  
   - **General Measurement Model (GMM) / Building Block Approach (BBA):**  
     - Default model for most insurance contracts.  
     - Liabilities are measured using the present value of future cash flows, a risk adjustment, and a contractual service margin (CSM).  
   - **Premium Allocation Approach (PAA):**  
     - Simplified model for short-duration contracts (e.g., non-life insurance) where it is a reasonable approximation of GMM.  
   - **Variable Fee Approach (VFA):**  
     - Applied to insurance contracts with direct participation features, where the policyholder shares in investment returns.

3. **Key Components**  
   - **Fulfillment Cash Flows (FCF):**  
     - Current estimates of future cash inflows and outflows.  
   - **Risk Adjustment for Non-Financial Risk:**  
     - Reflects the compensation required for uncertainty in the amount and timing of cash flows.  
   - **Contractual Service Margin (CSM):**  
     - Represents unearned profit from the insurance contract, recognized as revenue over the service period.

4. **Discount Rates**  
   - Future cash flows are discounted using rates that reflect the time value of money and the characteristics of the insurance liabilities.

5. **Recognition of Revenue and Expenses**  
   - Revenue is recognized as insurance services are provided.  
   - Expenses are matched to the period when the services are delivered.

6. **Aggregation of Contracts**  
   - Contracts are grouped into portfolios with similar risks and managed together.  
   - Portfolios are further divided into:  
     - Contracts that are onerous at initial recognition.  
     - Contracts that have no significant risk of becoming onerous.  
     - Remaining contracts.

7. **Presentation and Disclosure**  
   - Clear separation of insurance service results (underwriting) and financial results.  
   - Enhanced disclosures about assumptions, risks, and the financial position of insurance contracts.

8. **Reinsurance Contracts**  
   - Requires separate accounting for reinsurance contracts held and issued, ensuring transparency in risk transfer mechanisms.

9. **Transition Requirements**  
   - Entities must adopt IFRS 17 retrospectively where possible, or use a modified retrospective or fair value approach if full retrospective application is impractical.

---

## Objectives of IFRS 17

- **Comparability:** Ensures consistency in reporting insurance contracts globally.  
- **Transparency:** Provides detailed insights into profitability and risks.  
- **Accountability:** Links financial performance to the provision of insurance services.
