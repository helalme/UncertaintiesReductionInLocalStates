## Analyzing and predicting local states in Homogenization-localization problems using statistics, data science and ML approaches
Homogenization is one of the very common techniques used in micro and multiscale mechanics. Since many properties of a material at visible length-scale have their origin at lower lenghscale, we apply homogenization techniques in order to have an assessement of local property distribution. Estimating properties at lower length-scale is known as localization. We have showed in [another repository](https://github.com/helalme/DataDrivenMSE/tree/master/UncertaintyReductionInHomogenization) that homogenized properties might have uncertainties with high bias and variance, we also showed how to reduce these uncertainties usig machine learning techniques, avoiding huge computational cost. 

For better product design we need to have a very good assessement of the local states/properties as well. In this repository, we will show how to predict local states for a statistically equivalent RVE reducing uncertainties. We will use statistics, data science and machine learning techniques to analyze, visualize and predict local states with reasonable accuracies, which in turn reduce high computational cost.

The background problem, boundary conditions etc. everything is same for this repository as described in [URHP](https://github.com/helalme/DataDrivenMSE/tree/master/UncertaintyReductionInHomogenization) 
repository. This means we will have 6 set of local data/states/properties for 6 different cubic RVE ranging from 28.75 $\mu m$ to 128.75 $\mu m$ of side lengths. Since the dominant component is $$\sigma_{33}$$ in both lenghscales, we will consider this component only for this problem.

One thing is to be noted that the number of local states are different for every size of RVE. We can consider several locations for a property, like nodal points, Gauss points, etc. To reduce the data size we will consider one value of $$\sigma_{33}$$ for each element from FE-mesh, that is centrodal point. Using the distributions of $\sigma_{33}$ from the lower sized RVE, we will try to predict local states of a higher sized true SERVE.
