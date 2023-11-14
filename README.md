# WCS_COG260

# COG260 Project Proposal
We propose that our project attempts to answer the question of why there is cross-linguistic variation between languages. One potential motivator of cross-linguistic variation may be the difference in environmental factors, like climate, or the diversity of the color spectrum found in the environment. Evidence from cross-sectional studies indicates that languages evolve in a way that is adapted for their unique environmental context; however, causality has yet to be established due to the correlational nature of these studies (Nölle et al., 2020). The phenomenon that different languages have different “basic color terms”, defined by Berlin and Kay (1969) as universally understood, monolexemic words that are not derived from or not used to describe other colors or objects, can be examined under the lens of environmental influence. Specifically, the variation in basic color terms across languages might be explored in relation to the diverse color spectrums in different geographical regions, potentially revealing how environmental factors shape linguistic color categorization. One of the theories regarding the emergence of the color word “blue” supports the idea that a lexicon may be influenced by the “salient features” in an environment, such as bodies of water (Josserand  et al., 2021). At the same time, the physiological account for the emergence of blue puts forth that increased exposure to ultraviolet light may result in a lowered perception of blue in the color spectrum, which would result in the tendency to use a single term encompassing both blue and green (Bornstein, 1973; Josserand  et al., 2021). To determine the validity of these two opposing theoretical frameworks, a formal analysis of the distribution of color lexicons across specific color groups is needed. We propose that there will be no significant difference in the mean number of color terms used in languages across different regions with different latitudes, but the number of color terms for blue and green chips will positively correlate with distance from the equator.
The data cleaning and preparation for this study includes extracting the country names corresponding to each language and its associated index, as well as obtaining latitude information corresponding to all the countries of the languages in the dataset. This effort yields us with two dictionaries: languageData which gives the country name corresponding to the hierarchical keys for language number and language name, and countryData that gives the latitude for a given country name key. We will use a series of statistical tests and models to test the proposed hypothesis. 
Permutation Test
With the null hypothesis that there is no difference in the mean number of color terms used in languages across different latitudes, we will conduct a permutation test. To simulate the null, the latitude assignments among the languages in the dataset will be randomly permuted, keeping the mean number of color terms used by the speakers of that language constant. Performing a large number of permutations, the mean number of color terms used by the speakers of a language for each latitude will be recalculated. The proportion of permutations that result in a mean number of color terms at least as extreme as the observed values in the dataset will be compared against a significance level of 0.05. 
	A summary table for the findings of the permutation test that includes the test statistic, mean of the permutation results, and the p-value will be generated.
# Hypothesis Test
We will conduct a hypothesis test to assess the significance of the correlation between latitude and the number of color terms for the colors blue and green. The correlation calculation will be done using the Pearson correlation if the normality assumption is met, or Kendall’s Tau will be used to determine the correlation between color terms for blue and green and ordinally ordered latitude information. The test statistic relevant for the employed correlation method will be calculated to assess the significance of the correlation.
A scatterplot will be generated to visually represent the relationship and the strength of the correlation, as well as a summary table that outputs the observed correlation, the test statistic, and the p-value of the hypothesis test.
# Regression Model
Using the total number of color terms and the color terms used specifically to describe blue and green as the dependent variables and the latitude as the independent variable, we will model the relationship between the distance from the equator and the number of color terms employed by the speakers of a language. Conditional on the existence of a linear relationship between the variables, a linear regression model will be fitted. The assumptions of the model fitted will be checked, and a goodness of fit test will be conducted by assessing the R2 . The significance of the coefficients of the model will be analyzed.
The linear regression model obtained will be plotted to display the regression line and the equation. 
The Division of Labor
For the preparation of the proposal, the division of labor was as follows:
Ezra worked on the external research and the preliminary code for the creation of languageData and countryData, as well as the generation of some figures given in the Appendix. Elif worked on the external research used to introduce and motivate the proposed hypothesis, the proposal write-up, and generation of some figures given in the Appendix. Both collaborators took part in formulating the hypothesis and planning the project. During the implementation of methods, Elif will conduct the permutation test, while Ezra will perform the hypothesis test. Both will work on the regression model together, as well as the project report write-up.







# References
Berlin, Brent., & Kay, P. (1969). Basic color terms; their universality and evolution. University 
of California Press.
Bornstein, M. H. (1973). Color vision and color naming: A psychophysiological hypothesis of 
cultural difference. Psychological Bulletin, 80(4), 257–285. https://doi.org/10.1037/h0034837
Josserand, M., Meeussen, E., Majid, A. et al. Environment and culture shape both the colour 
lexicon and the genetics of colour perception. Sci Rep 11, 19095 (2021). https://doi.org/10.1038/s41598-021-98550-3
Nölle, J., Fusaroli, R., Mills, G.J. et al. Language as shaped by the environment: linguistic 
construal in a collaborative spatial task. Palgrave Commun 6, 27 (2020).	
https://doi.org/10.1057/s41599-020-0404-9


color terms per chip across rank (ordered distance from the equator) and latitude, respectively. This exploratory analysis aided in the fine tuning of the proposed cognitive hypothesis, and motivated the understanding that the mean number of general color terms in a language is likely to be constant for different regions with different latitudes. An initial executable Python notebook (named main.ipynb) can be found here: https://drive.google.com/drive/folders/1aGtsRJZ92dEfR45GGLgLe_rrQNImH78t?usp=sharing




 

