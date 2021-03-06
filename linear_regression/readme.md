This linear regression was implemented with gradient descent algorithm. 

<img src="https://github.com/gogowenzhang/machine-learning-algorithms-python/blob/master/img/linear-regression.png" width='600' height='300'>

### Test with generated dataset
```
from sklearn.datasets import make_regression
X, y, coef = make_regression(n_features=10, coef=True)
```

### In a terminal, you should be able to run your function like this:
```
import linear_regression as f
from GradientDescent import GradientDescent
gd = GradientDescent(f.cost, f.gradient, f.predict)
gd.fit(X, y)
print "coeffs:", gd.coeffs
predictions = gd.predict(X)
```

Package Dependencies:
- numpy==1.13.1
- sklearn==0.18.1
