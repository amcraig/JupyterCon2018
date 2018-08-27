# Handling Missing Data in Jupyter Notebooks

*We're using the MissingNo package*

[GitHub Link](https://github.com/matthewbrems/jupytercon-missing-data-2018)

Great Resource: [Chris Albon](https://chrisalbon.com/)

## How big of a problem is missing data?
* We can only infer from what we observe
* 10 of missing data can throw off regression lines by staggering amounts

**Imputation**: filling in the blanks

Given some data, lets try to fill in the missing gaps with simulation.

Missing Data can substantially undermine our analyses and inferences

## The Three Types of Missing Data 
### MCAR: Missing Completely At Random
No systematic reason for why the data was missing e.g. a biologist knocks off pitri dishes off table by accident

Conditional on data we have not observed

### MAR: Missing At Random
"I administer a survey that includes a question about income. Those who are female are less likely to respond to the question about income" 

Conditional on data we have observed, but we can correct, perhaps with weights

### NMAR: Not Missing At Random
"I administer a survey that includes a question about income. Those who have lower incomes are less likely to respond to the question about income"

* The data of interest are systematically different for respondnets and nonrespondents

## Methods of working with Missing Data
1. we can avoid it
2. we can ignore it
3. we can account for it

## Definitions and Examples

Unit Nonresponse: e.g. User took survey and didn't fill it in. a empty data point (user felt uncomfortable answering)

Item Nonresponse: e.g. Some questions in survey are missing

Complete-Case Analysis: Drops and observation with any missing value

Available-Case Analysis: Drops no observations and calculates result based on available data

Deductive Imputation: uses logic

Mean/Median/Mode Imputation: for any NA, replace with mean (or median or mode)

Regression Imputation: for any NA, replace it with a value predicted from a regression line

Hot-Deck Imputation: Divide sample units into classes(i.e. age and sex). For any NA value in a given class, replace NA with a random observed value from that class

