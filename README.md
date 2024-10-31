## Statistical Inference
### Introduction
As a commodity to be consumed, the quality of wine is of great importance, though it can differ greatly from wine to wine. A possible factor that influences the quality of a wine is its composition, so this study will aim to use statistical inference to determine if there is a significant difference between the compositions of different quality wines.

The dataset used is the Wine Quality dataset from the UCI machine learning repository, and it consists of red and white variants of vinho verde wine. For this study, we will only be using red wine and we will classify each wine as either "low" or "high" quality.

Wine quality is linked to what is referred to as the sugar-acid balance, so understanding how the acidity of a wine affects its quality is of significant importance (White, 2019). Therefore, the variables of interest are:

Fixed Acidity: A major wine constituent, contributing greatly to its taste, imparting the sourness or tartness that is a fundamental feature in wine taste.

Volatile Acidity: The steam distillable acids present in wine, primarily acetic acid but also lactic, formic, butyric, and propionic acids, imparting a vinegar-like taste.

### Question
Do fixed acidity and volatile acidity differ between different qualities of red wine?

### Discussion
The p-values obtained by asymptotics are 0.0001168400 for the mean difference in fixed_acidity and 3.480735e-39 for the mean difference in volatile_acidity. For both hypothesis tests, the p-value was less than the significance level of 0.1, so the null hypothesis was rejected both times. This means the original sample provides sufficient evidence to conclude that fixed_acidity and volatile_acidity differ between different qualities of red wine. This difference in acidity between good and poor quality red wines offers considerable value for determining red wine quality. Checking the acidity of red wine might help consumers pick the finest wine for their requirements.

The two confidence intervals we obtained (via asymptotics) for the mean difference in fixed_acidity and the mean difference in volatile_acidity are (0.1905108, 0.4731508) and (-0.1294351, -0.1012779) respectively. Fixed acidity is measured in g(tartaric acid)/dm^3 and volatile acidity is measured in g(acetic acid)/dm^3. We can see that the confidence interval for volatile acidity is negative, which means that low quality red wines have a greater amount of volatile acidity. This is corroborated by external research, as excessive volatile acidity in wine is known to lead to deterioration of said wine, resulting in a pungent flavour (Vilela-Moura et al., 2011).

The extreme p-values, for the most part, validate our initial expectation that high and low quality red wines exhibit significant differences in acidity. This implies that acidity is indeed a critical element in determining a red wine's quality. In the future, we can investigate the chemical composition of acidity in greater detail to determine which components have the greatest impact on different qualities of red wine, or even if the effect of acidity on wine quality holds for other types of wine.
