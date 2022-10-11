# Special-Functions
This is a repository of the special functions that widely used in Physical Sciences. <br>
This only serve as a notes for anyone who want to study them. <br>
Personally I highly recommend to use the books below as the textbook to study the Mathematical Physics:<br>
[Mathematical Methods for Physicists: A Comprehensive Guide 7th Edition](https://www.amazon.com/Mathematical-Methods-Physicists-Comprehensive-Guide/dp/0123846544) <br>
[Mathematical Methods in the Physical Sciences 3rd Edition](https://www.amazon.com/Mathematical-Methods-Physical-Sciences-Mary/dp/0471198269)
#### For those students who are really under poverty line, you may get the e-book from https://libgen.is/ to study the material and remember to buy the book once you have enough financial resources. 

## The Factorial Function
The Factorial Function is given as:
$$\int_{0}^{\infty} x^n e^{-x} dx = n!$$
Boas using a heuristic method to describe how to get the factorial function.<br>
However, the Factorial Function is really a direct result of applying the integration by part, as shown below. <br>
The formula of integration by part is:

$$ \int_a^b u \frac{dv}{dx} dx = \left.uv\right\vert_a^b - \int_a^b v \frac{du}{dx} dx $$

Take $u=x^n$ and $\frac{dv}{dx}=e^{-x}$, we have $\frac{du}{dx}=nx^{n-1}$ and $v=-e^{-x}$ and substitute them into the integration by part formula, we get:

$$ \int_0^{\infty} x^n e^{-x} dx = \underbrace{\left.x^n(-e^{-x})\right\vert_0^{\infty}}_\text{=0} - n\int_0^{\infty} (-e^{-x}) x^{n-1} dx $$

or 

$$\begin{aligned}
\int_0^{\infty} x^n e^{-x} dx &= n\int_0^{\infty}  x^{n-1} e^{-x} dx \\ 
&= n(n-1)\int_0^{\infty} x^{n-2} e^{-x} dx \\
&= n(n-1)(n-2) \int_0^{\infty} x^{n-3} e^{-x} dx \\
&= n(n-1)(n-2)...(n-(n-1)) \int_0^{\infty} x^{n-n} e^{-x} dx \\
&= n(n-1)(n-2)...(1) \int_0^{\infty} e^{-x} dx \\
&= n! \underbrace{\left(-e^{-x})\right\vert_0^{\infty}}_\text{=1} \\
&= n! \\
\end{aligned}$$






