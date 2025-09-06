I created a synthetic dataset of 100 houses with features like size, bedrooms, and distance from the city center.
After cleaning and exploring the data, I built a linear regression model to predict house prices.
The model performs very well, with an R² of 0.994, meaning it explains over 99% of the variation in prices.
On average, predictions are within about 8 units of the actual price, which is very accurate given the price range.
The coefficients make sense: bigger houses and more bedrooms increase price, while being farther from the city decreases it.
This shows the model captures the expected real estate path

R² score: 0.994

That’s very close to 1, which means your model explains 99.4% of the variation in house prices.

In plain English: “The model is very accurate at predicting prices using size, bedrooms, and distance.”

RMSE: ~7.7

Since your prices range from ~100 to ~475, an average error of only 7.7 is tiny.

“On average, the model’s predictions are off by about 7–8 units, which is small compared to the price scale.”

Coefficients

Size (2.93) → Each extra square meter adds about 3 units to the price.

Bedrooms (8.86) → Each additional bedroom adds about 9 units to the price.

Distance (-2.06) → Each km farther from the city center reduces the price by about 2 units.

Intercept (10.89)

This is the base price when size, bedrooms, and distance are 0 (not realistic, but mathematically needed for the regression).

Plot (Actual vs Predicted)

If the scatter points hug the red diagonal line, it shows your predictions are very close to the true prices.
Residuals vs. Predicted Prices
The scatter plot shows residuals (actual – predicted prices) plotted against predicted values.

The residuals are tightly clustered around the horizontal line at zero, which suggests:

No major bias in predictions.

Homoscedasticity — the variance of errors remains fairly constant across prediction values.

The model isn’t systematically over- or under-predicting for any price range.



Histogram of Residuals
The histogram appears roughly symmetric and bell-shaped.

This implies that most predictions are close to the actual values, with only a few outliers.

A well-centered distribution around zero is a good sign — it means errors are balanced.
Q-Q Plot
The Q-Q plot compares the distribution of residuals to a normal distribution.

If the points fall along the diagonal line, it suggests the residuals are approximately normally distributed.

This is important for validating assumptions in linear regression and for confidence in statistical inference.

Nahom W