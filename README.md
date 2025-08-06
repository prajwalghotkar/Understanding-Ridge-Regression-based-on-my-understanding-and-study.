# Understanding Ridge Regression.

-Ridge Regression is one of the foundational regularization techniques in machine learning and statistics. It’s especially useful when dealing with multicollinearity or overfitting in linear models. I’ve broken it down into 5 key points based on my understanding and study.
---
##### 1) How the Coefficients Get Affected?
- In Ridge Regression, we introduce a penalty on the size of the coefficients, which forces them to shrink. Unlike Lasso, Ridge doesn’t reduce them to exact zero, but significantly reduces their magnitude. This shrinkage leads to more stable and generalizable models, especially in cases where the features are highly correlated or noisy.

![prajwal_data](https://github.com/user-attachments/assets/ce16b4c7-5526-4fbf-9cb6-6ec1bd39b9ba)
---
##### 2) Higher Values Are Impacted More
- Since Ridge adds the square of the coefficients to the loss function, it affects larger values more aggressively. That means:
Penalty=λ∑β𝑗2 So, the bigger a coefficient is, the more it gets penalized. This ensures that no one feature dominates the model unless absolutely necessary.
---
##### 3) Bias-Variance Tradeoff
- One of the most insightful aspects of Ridge Regression is how it handles the bias-variance tradeoff.
  - By shrinking the coefficients, Ridge increases bias slightly.
  - But it also reduces variance significantly, which often leads to better performance on unseen data.
- In real-world data science tasks, this tradeoff helps build models that are robust and less sensitive to noise.
![WhatsApp Image 2025-08-06 at 20 55 08_d1fea426](https://github.com/user-attachments/assets/d993c265-1844-42e5-8cbb-7daee45cced4)
---
##### 4) Impact on the Loss Function
- The loss function for Ridge becomes:
​![WhatsApp Image 2025-08-06 at 21 02 30_45fd28cb](https://github.com/user-attachments/assets/931b8d2c-f11c-44d4-ae87-b5a83539aa72)
- This is a combination of the traditional Residual Sum of Squares (RSS) and a penalty term.
- he goal is no longer just to minimize prediction error, but also to keep the model as simple as possible by penalizing large coefficients.
---
##### 5) Why It’s Called "Ridge"? 
This is where things get visually intuitive.
- In the image below (which I drew to understand the geometry of Ridge Regression), the elliptical contours represent the OLS loss function. The circle around the origin is the constraint region defined by Ridge (i.e., the region where the sum of squared coefficients is limited).
![WhatsApp Image 2025-08-06 at 21 06 37_93cb4f75](https://github.com/user-attachments/assets/0e9c2b10-95a3-4c7f-965d-4e5061958a5b)
- Where the smallest loss contour just touches the constraint circle, that’s where Ridge gives us the best estimate. This edge — or "ridge" — created by the constraint is how the algorithm gets its name.

