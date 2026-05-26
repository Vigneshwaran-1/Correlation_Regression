# Correlation and regression for data analysis
# Aim : 

To analyse given data using coeffificient of correlation and regression line
![image](https://user-images.githubusercontent.com/104613195/168224136-d6b64e64-7d3d-4775-9337-c8f96fe41f2d.png)


# Software required :  

Python

# Theory:

Correlation describes the strength of an association between two variables, and is completely symmetrical, the correlation between A and B is the same as the correlation between B and A. However, if the two variables are related it means that when one changes by a certain amount the other changes on an average by a certain amount.  

If y represents the dependent variable and x the independent variable, this relationship is described as the regression of y on x. The relationship can be represented by a simple equation called the regression equation. The regression equation representing how much y changes with any given change of x can be used to construct a regression line on a scatter diagram, and in the simplest case this is assumed to be a straight line.

# Procedure :

![image](https://user-images.githubusercontent.com/104613195/168225866-ac8f6610-bdc3-4ac2-a24e-2b24ba08e189.png)

# Program :
~~~
import numpy as np

X = np.array([25, 28, 35, 32, 31, 36, 29, 38, 34, 32])
Y = np.array([43, 46, 49, 41, 36, 32, 31, 30, 33, 39])

r = np.corrcoef(X, Y)[0, 1]
print("Correlation coefficient (r):", round(r, 3))

b = np.sum((X - X.mean()) * (Y - Y.mean())) / np.sum((X - X.mean())**2)
a = Y.mean() - b * X.mean()

print(f"Regression line equation: Y = {a:.3f} + {b:.3f}X")
~~~


# Output 
<img width="356" height="92" alt="image" src="https://github.com/user-attachments/assets/26053bfa-676c-4af9-b443-25e27ce95f3d" />

# Result
Thus given experiment is done successfully.
