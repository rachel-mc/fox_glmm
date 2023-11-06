# Generalized linear mixed models applied to ecological data on wildlife monitoring

Here we present a report on the analyses of fox abundance, based on the village dataset (https://biotime.st-andrews.ac.uk/selectStudy.php?study=373), which can be reproduced using R.

There are three situations when human beings should intervene in wildlife at the population level: (i) when populations are decreasing or have been depleted, (ii) when populations are rapidly increasing, with implications of economic damage or putting other species at risk, and (iii) to optimise yield of a particular species of economic or societal importance (Caughley, 1994). There are thousands of endangered species which fall within category (i), hundreds of pest or invasive species falling within category (ii), and dozens falling within category (iii) (Verdade et al., 2014a). However, the millions of species which do not fall into any of the three categories above are usually neglected (Verdade et al., 2014b; Fisher, 2011). Decades ago, Caughley (1994) drew attention to these species as potential targets for monitoring. However, long-term monitoring programmes require a high input of resources, and are not feasible without incurring huge expense, especially when dealing with more than a handful of species at a time.
	We have therefore four approaches to wildlife management: (i) biological conservation, (ii) control, (iii) sustainable use and (iv) monitoring without intervention (Verdade et al., 2014b). Unquestionably the most sensitive management approaches are conservation and sustainable use, because errors of assessment or programme implementation can result in species extinction, which is irreversible. Management errors when controlling pest populations typically cause economic damage, but may also cause local extinction of other species in the community (e.g. Moral et al., 2016), or even allow for the introduction of new pests. Finally, monitoring is the simplest and safest alternative, since it implies only detecting fluctuations in population size of the species in a certain region (Verdade et al., 2014a). Therefore, it is a non-invasive alternative. Most importantly, monitoring is itself essential to guiding decision-making and the implementation of any management strategy aimed at conservation, control or sustainable use (Yoccoz et al., 2001; Nichols and Williams, 2006).
 
This project aims to model the abundance of medium and large mammal species in approximately 200 locations in Japan. This study was carried out by the Ministry of Environment of Japan (2014), and used infrared sensor cameras to detect 25 different species from 2005 to 2012. Data is available on number of animals of each species that was observed. Since this response consists of counts of multiple species, the classical Gaussian linear model would not constitute the best approach for analysis. Moreover, since observations are made on the same site at different time occasions, the independence assumption is also not reasonable. The generalized linear mixed modelling (GLMM) framework allows us to flexibilise (1) the normality assumption, and (2) the independence assumption, so as to accommodate the true nature of the response variable and the correlation between observations taken on the same site (Verbeke and Molenberghs, 2000).

By working with multispecies data, it is important to carry out exploratory analyses to understand potential ecological interactions within the community and species assemblies. The first step in this project will be to employ dimension reduction techniques (such as PCA and uMAP) to study the correlations between the different species, as well as to produce different types of visualisations, representing both the temporal and spatial dimensions. As a second step, Poisson and negative binomial generalized linear mixed models will be fitted using R (R Core Team, 2023) and package lme4 (Bates et al., 2015). We will carry out model selection using different types of linear predictors, including e.g. polynomial or spline effects to accommodate nonlinearity over time. Next, we will assess model goodness-of-fit through different diagnostic frameworks, e.g. half-normal plots with a simulated envelope (Moral et al., 2017). Finally, we will carry out inferential analyses and produce a report.

References:

Bates, D., Maechler, M., Bolker, B., Walker, S. (2015). Fitting Linear Mixed-Effects Models Using lme4. Journal of Statistical Software, 67(1), 1-48. doi:10.18637/jss.v067.i01.

Caughley, G. (1994) Directions in conservation biology. Journal of Animal Ecology, 63, 215-244.

Fisher, D.O. (2011) Cost, effort and outcome of mammal rediscovery: Neglect of small species. Biological Conservation, 144(5), 1712-1718.

Monitoring Site 1000 Project, Biodiversity Center, Ministry of Environment of Japan (2014) “Monitoring site 1000 Village survey - Medium and large mammal survey data (2006-2012)” (SAT03zip, downloaded from http://www.biodic.go.jp/moni1000/findings/data/index.html). Accessed 2023.

Moral, R.A., Azevedo, F.C.C., Verdade, L.M. (2016) The use of sheepdogs in sheep production in Southeastern Brazil. Pastoralism Research, Policy and Practice, 6(1), 1-7. 

Nichols, J., Williams, B.K. (2006) Monitoring for conservation. Trends in Ecology and Evolution, 21(12), 668-673.

R Core Team (2022). R: A language and environment for statistical computing. R Foundation for Statistical Computing, Vienna, Austria. URL https://www.R-project.org/.

Verbeke, G. and Molenberghs, G. (2000). Linear Mixed Models for Longitudinal. Data. Springer Series in Statistics. New-York: Springer.

Verdade, L.M., Lyra-Jorge, M.C., Piña, C.I. [Eds.] (2014a) Applied Ecology and Human Dimensions in Biological Conservation. Springer-Verlag, Heidelberg, 228p.

Verdade, L.M., Lyra-Jorge, M.C., Piña, C.I. (2014b) Redirections in conservation biology. p.3-17. In: Verdade, L.M., Lyra-Jorge, M.C., Piña, C.I. [Eds.]. Applied Ecology and Human Dimensions in Biological Conservation. Springer-Verlag, Heidelberg.

Yoccoz, N.G., Nichols, J.D., Boulinier, T. (2001) Monitoring of biological diversity in space and time. Trends in Ecology and Evolution, 16(8), 446-453.

My role involved:
1.	Independent study of GLMM theory and implementation using R;
2.	Practical work with a dataset on the abundance of different species of medium and large mammals observed using camera traps in Japan;
3.	Producing meaningful visualisations of the data as initial exploratory analysis, involving dimension reduction techniques;
4.	Fitting and interpreting GLMMs to the data;
5.	Performing model selection and assessing goodness-of-fit;
6.	Producing a report on the analysis using R Markdown.
I acquired expertise in the theory and implementation of generalized linear mixed models, as well as applied knowledge in ecology and wildlife management.
