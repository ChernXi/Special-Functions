# Special-Functions
This is a repository of the special functions that widely used in Physical Sciences. <br>
This only serve as a notes for anyone who want to study them. <br>
The most materials from this repository are getting from "Mathematical Methods in the Physical Sciences", written by Mary L.Boas. <br>

## The Factorial Function
The Factorial Function is given as:
$$\int_{0}^{\infty} x^n e^{-x} dx = n!$$
Boas using a heuristic method to describe how to get the factorial function.<br>
However, the Factorial Function is really a direct result of applying the integration by part, as shown below. <br>
From the definition of integration by part, we have: 
$$\int_a^b u \frac{dv}{dx} dx = \left.uv\right\vert_a^b - \int_a^b v \frac{du}{dx} dx $$
Take $u=x^n$ and $\frac{dv}{dx}=e^{-x}$, we have $\frac{du}{dx}=nx^{n-1}$ and $v=-e^{-x}$.<br>
Substitute them into the integration by part, give:
## $\int_0^{\infty} x^n e^{-x} dx = \underbrace{\left.x^n(-e^{-x})\right\vert_0^{\infty}}_\text{=0} - n\int_0^{\infty} (-e^{-x}) x^{n-1} dx $





