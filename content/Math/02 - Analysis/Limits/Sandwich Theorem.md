The "sandwich theorem," also known as the "squeeze theorem" or the "pinching theorem," is a fundamental concept in calculus limits. It provides a method for evaluating limits of a function by "squeezing" them between two other functions whose limits are known.
```desmos-graph
y=0.01e^{(-x)}*\cos(5x)
y=0.01e^{-x}
y=-0.01e^{-x}
```

The sandwich theorem is particularly useful when direct evaluation of a [[Limit]] is challenging. By finding simpler functions that "squeeze" the original function, you can often determine the limit of the original function indirectly. It's a powerful tool for proving the convergence or divergence of complicated sequences or series and for establishing the existence of limits in various contexts within calculus.
To do this, we create two other functions to "squeeze" the original function with. We can do this by evaluating the trigonometrical function as the smaller value it could be, then the largest. We then replace the trigonometry in the original function with these two values, then we can see that they "squeeze" together at a single point. 

