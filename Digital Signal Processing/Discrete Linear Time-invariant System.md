# Discrete Linear System
The term *linear* defines a special class of systems where output is the superposition (sum) of the individual outputs had the individual inputs been applied separately to the system.
Ex: if $x_{1}(n) \xrightarrow{\text{results in}} y_{1}(n)$ and $x_{2}(n) \xrightarrow{\text{results in}} y_{2}(n)$, then $x_{1}(n) + x_{2}(n) \xrightarrow{\text{results in}} y_{1}(n) + y_{2}(n)$

Also, part of this description of linearity is a proportionality.
Ex: follow from the above example,
$c_{1}x_{1}(n)+c_{2}x_{2}(n) \xrightarrow{\text{results in}} c_{1}y_{1}(n)+c_{2}y_{2}(n)$

In literature, this property is called *homogeneity property*.

### An example of non-linear System
Given a system $y(n) = [x(n)]^2$.

Suppose we have an input signal
$$
x_{1}=\sin(2\pi n t_s)
$$
with frequency $f_0$ = 1 Hz to the system, we then have the output signal
$$
y_{1}=\frac 1 2 - \frac{\cos(4\pi n t_{s})}{2}
$$
Go through the same process with another signal $x_{2}=\sin(6\pi n t_s)$ then add this with $x_{1}(n)$ to create $x_{3}(n)$. Apply $x_{3}(n)$ to the system, we have the output signal
$$
(x_{1}+x_{2})^{2} = x_{1}^2+x_{2}^{2}+2x_{1}x_{2}
$$
We can already see from this example the non-linear behaviour of this system. The output signal have an addition sinusoidal componet $2x_{1}x_{2}$ which was not present in either of the outputs when the indiviual sinewaves alone were applied. EE recognizes this effect as *intermodulation distortion*.

## Properties
[[Commutative - Linear Time-invariant Systems]]