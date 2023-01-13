# Delfi

Please access the file with the latest date (20230112)

Chen model performs badly(with nans meaning hitting negative rates) might because:

From the plot of level (PCA component) according to our data, the curve is generally decreasing with a comparatively slight upward trend (maybe representing a mean reversion, maybe not) at the tail. As Chen model consider drift (rolling averages) and volatility with CIR process, the approximation of drift indicates a CIR process with mean $\zeta$ close to zero while the volatility $\alpha$ "too large for $\zeta$ to control", as the CIR model believes that our data of level represents the state of mean-reverting.

We may try to modify the model of drift approximating, either switch to other process or to other indicating values.
