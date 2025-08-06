# Understanding Ridge Regression.

***Ridge Regression is one of the foundational regularization techniques in machine learning and statistics. It’s especially useful when dealing with multicollinearity or overfitting in linear models. I’ve broken it down into 5 key points based on my understanding and study.***
---
##### 1) How the Coefficients Get Affected?
- In Ridge Regression, we introduce a penalty on the size of the coefficients, which forces them to shrink. Unlike Lasso, Ridge doesn’t reduce them to exact zero, but significantly reduces their magnitude. This shrinkage leads to more stable and generalizable models, especially in cases where the features are highly correlated or noisy.
![WhatsApp Image 2025-08-06 at 19 50 06_808ac199](https://github.com/user-attachments/assets/24e1d8d8-e1df-498b-840f-863809e79cb1)
