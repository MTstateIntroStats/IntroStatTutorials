# AppliedStatsInteractive
 
This is an R package which deploys interactive notebooks to accompany an introductory course in applied statistics. The notebooks follow the freely available [OpenIntro Statistics (4Ed)](http://www.openintro.org/os) textbook and supplementary resources. 

You can install this package by running the following command in R (which requires the `devtools` package as a prereqisite): `remotes::install_github("agmath/AppliedStatsInteractive")`

Once the package has been installed you can run the individual notebooks using commands of the following structure: `learnr::run_tutorial(NOTEBOOK_NAME, package = "AppliedStatsInteractive")`

The available notebooks are as follows:
+ 0_StartHere
+ 1_IntroToData
+ 2_IntroToR
+ 3_DescriptiveNumCat
+ 4_DataViz
+ 5_DiscreteDistributions
+ 6_NormalDistribution
+ 7_DiscreteDistributionsLab
+ 8_NormalDistributionLab
+ 9_FoundationsForInference
+ 10_IntroInferenceLab
+ 11_HTandCIprop
+ 12_InferencePractice
+ 13_InferenceCategoricalLab
+ 14_ChiSquare
+ 15_HTandCInum
+ 16_InferencePractice
+ 17_InferenceNumericalLab
+ 18_ANOVA
+ 19_LinearRegression

The notebook named 4_DataViz is an adaptation of the data visualization chapter from Hadley Wickham and Garrett Grolemund's [R for Data Science](https://r4ds.had.co.nz/).

## A Note on Rendering Workbooks

Multiple calls to `learnr::run_tutorial()` in a single R session cause rendering errors in the notebooks -- exercises are not rendered correctly. This can be avoided by closing RStudio and re-opening before rendering a second workbook. If you already rendered the notebook with the rendering error, you should use your file manager to navigate to the folder containing the workbook and delete the *html* file. Calling `learnr::run_tutorial()` now will re-build the html file. I will update this section when a better workaround is discovered.
