# Understanding Ridge Regression.

***Ridge Regression is one of the foundational regularization techniques in machine learning and statistics. It’s especially useful when dealing with multicollinearity or overfitting in linear models. I’ve broken it down into 5 key points based on my understanding and study.***
---
##### 1) How the Coefficients Get Affected?
- In Ridge Regression, we introduce a penalty on the size of the coefficients, which forces them to shrink. Unlike Lasso, Ridge doesn’t reduce them to exact zero, but significantly reduces their magnitude. This shrinkage leads to more stable and generalizable models, especially in cases where the features are highly correlated or noisy.

![prajwal_data](https://github.com/user-attachments/assets/ce16b4c7-5526-4fbf-9cb6-6ec1bd39b9ba)

