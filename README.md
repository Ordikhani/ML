Overfitting and Underfitting with Ridge Regularization (L2)
This Python script demonstrates how regularization helps prevent overfitting in machine learning models.
1.	The Goal: We want to learn a sine wave function y=sin(2πx) using only 10 noisy data points (blue dots).
2.	The Model: We use a high-degree (9th-degree) Polynomial Regression model. Since a 9th-degree polynomial is very flexible, it can easily overfit if not controlled.
3.	The Solution (Ridge Regularization): We apply Ridge Regression (L2 regularization) with different penalty strengths (lambda or alpha): 
  I.	λ=0 (Overfitting): There is no penalty. The model tries too hard to touch every noisy training point. The curve oscillates wildly and fails to represent the true green sine wave.
  II.	λ=10−e6: The penalty is too weak, and the model is still slightly overfitting.
  III.	λ=10−e3 (Good Fit): The penalty is balanced. The red prediction line smoothly follows the true green sine wave, ignoring the random noise.
  IV.	λ=1 (Underfitting): The penalty is too strong. It restricts the model weights too much, forcing the prediction to become almost a flat line that fails to capture the pattern.
<img width="1189" height="790" alt="RidgeRegularization" src="https://github.com/user-attachments/assets/2da42b44-7b54-4479-9b30-843702aaf145" />
