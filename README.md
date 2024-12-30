# Analyzing the Impact of the Earned Income Tax Credit (EITC)  

## Overview  
This project analyzes the labor supply responses of single women to the expansion of the Earned Income Tax Credit (EITC), a policy designed to provide tax relief to low-income individuals. The dataset focuses on single women and leverages key demographic and economic variables to explore the policy's effects on earned income, labor participation, and household dynamics.  

The analysis builds on the foundational work of **Eissa and Liebman (1996)**, which highlighted the role of the EITC in incentivizing labor supply. Using econometric methods such as **difference-in-differences (DiD)** and regression modeling, this project estimates the causal impact of EITC on labor market outcomes and examines the validity of the **parallel trends assumption**.  

## Dataset  
The dataset includes the following variables:  
- **state**: State's FIPS code (factor variable).  
- **year**: Calendar year.  
- **urate**: State's unemployment rate for the given year.  
- **children**: Number of children in the household.  
- **nonwhite**: Indicator for non-White individuals.  
- **finc**: Family household income.  
- **earn**: Earned income.  
- **unearn**: Unearned income.  
- **age**: Age of the mother.  
- **ed**: Years of schooling.  
- **work**: Indicator variable for current employment (1 if employed, 0 otherwise).  

## Research Questions  
1. How does having children affect the labor supply response to EITC?  
2. What is the causal impact of EITC expansion on earned income and employment?  
3. Are the assumptions underlying the difference-in-differences model, such as parallel trends, valid for this dataset?  
4. What insights can be gained from placebo treatment models in this context?  

## Analysis Highlights  
- **Treatment vs. Control Groups**: Women with children are analyzed as the treatment group, while those without children serve as the control group.  
- **Pre and Post-EITC Effects**: A dummy variable distinguishes pre- and post-EITC periods to estimate the policy's temporal impact.  
- **Difference-in-Differences (DiD)**: Used to compare labor outcomes between the treatment and control groups while controlling for state and year fixed effects.  
- **Conditional DiD Regression**: Regression models provide more nuanced estimates of the EITC effect, controlling for individual-level covariates like age, education, and income.  
- **Placebo Treatment Models**: Analyzed to verify that observed effects are not due to spurious correlations or unrelated trends.  

## Key Findings  
1. The EITC expansion significantly increased labor participation among single women with children.  
2. Parallel trends assumption holds for pre-treatment periods, validating the DiD approach.  
3. Placebo tests confirm the robustness of the estimated treatment effects.  
4. State-level unemployment rates and individual characteristics such as education and age influence the magnitude of the EITC effect.  

## Tools and Methods  
- **Programming**: R  
- **Statistical Techniques**:  
  - Difference-in-differences (DiD)  
  - Regression modeling  
  - Parallel trends validation  
  - Placebo treatment analysis  
- **Output**: Reproducible analysis provided in an R Markdown file.  

## References  
- Eissa, Nada, and Jeffrey B. Liebman. 1996. *Labor Supply Responses to the Earned Income Tax Credit*. Quarterly Journal of Economics, 111(2): 605-637.  

## How to Use  
1. Clone the repository to your local machine.  
2. Open the R Markdown file in RStudio.  
3. Run the analysis and knit the file to generate a comprehensive report.  

## License  
This project is open-source under the [MIT License](LICENSE).  
