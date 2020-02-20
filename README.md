# AB-Test

A/B tests are very commonly performed by data analysts and data scientists.

For this project, I analyze the data to understand the results of an A/B test run by an e-commerce website. The goal was to work through this notebook to help the company understand if they should implement the new page, keep the old page, or perhaps run the experiment longer to make their decision.

## Conclusions
- There was not enough evidence to reject the null hypthesis ($H_0$). We should reject $H_1$ and keep the old page.

- The evidence from the various techniques used above all supported this conclusion. However, the analysis and results are limited only based on available data - effects of change aversion and novelty effects may influence the results. Practical considerations may also need to be factored in while making decisions.

- There was even suggestion that the old page very marginally resulted in better conversions.

- Logistic Regression also gives results that agree with the results of A/B testing. Country does not appear to be a very useful factor in the regression model. The fit of logistic regression models does not appear to be great from the Pseudo R square values - The model can be revised for better predictions.

- The duration of the experiment is 14 days. The influence of time may be a major factor in determining the conclusions. It would be good to analyze the data for different subsets of time and look at how the conversion rates differ between control and treatment groups.


## Resources
The below two resources provided a way on dealing with the problem AttributeError: module 'scipy.stats' has no attribute 'chisqprob' when running .fit.summary() for logistic regression:
- http://www.statsmodels.org/stable/generated/statsmodels.discrete.discrete_model.LogitResults.summary2.html?highlight=summary2#statsmodels.discrete.discrete_model.LogitResults.summary2

- https://stackoverflow.com/questions/49814258/statsmodel-attributeerror-module-scipy-stats-has-no-attribute-chisqprob

- Using LaTeX in jupyter notebooks:
https://stackoverflow.com/questions/13208286/how-to-write-latex-in-ipython-notebook

- https://jupyter-notebook.readthedocs.io/en/latest/examples/Notebook/Typesetting%20Equations.html

- https://nbviewer.jupyter.org/github/ipython/ipython/blob/2.x/examples/Notebook/Display%20System.ipynb#LaTeX

- Many other stackoverflow posts

- Course content
