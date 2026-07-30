
On this page, I explain concepts using mathematical notation. 
What I write on this page is the representation of my understanding.

## What is function?

A function maps every in set X to an element in set Y. set X is called the domain of the function and the codomain of the function is set Y.

## What is the formal definition of finite limit?


Let $$f(x)$$ be defined for all $$x \neq a$$ over an open interval containing a. Let L be a real number. 

Then

$$
\lim_{x \to a} f(x) = L
$$

if, for every $$\varepsilon > 0$$, there exists a $$\delta > 0$$, such that if

$$
0 < |x-a| < \delta,
$$

then

$$
|f(x)-L| < \varepsilon.
$$  

This formal definition of finite limit is not easy to grasp initally but now I definitely have a better understanding of it. 
The following link can be helpful to understand the definition. 

[Formal Definition of a Limit (LibreTexts)](https://math.libretexts.org/Courses/Mount_Royal_University/Calculus_for_Scientists_I/2%3A_Limit__and_Continuity_of_Functions/2.5%3A_Formal_Definition_of_a_Limit_%28optional%29)

## What is partial derivative?

We have a function:

$$
f(x) = x^2
$$

The graph of the function is the following:

<p align="center">
  <img src="../images/Screen Shot 2026-05-27 at 9.28.47 AM.png" width="400">
</p>

The derivative (2x) gives the slope of the tangent line to the graph of the function.

Now, we have this function

$$
f(x,y) = (x^2+y^2) / 2 
$$

The graph of the function is the following:

<p align="center">
  <img src="../images/Screen Shot 2026-05-27 at 11.40.35 AM.png" width="400">
</p>
  
## partial derivatives 

$$
\frac{df}{dx} = x
$$

$$
\frac{df}{dy} = y
$$


## What is chain-rule?

Before defining the definition of chain-rule, let's first solve the following problems!

problem 1: 
$$
f(x) = (6x^2 + 7x)^4
$$

$$
\frac{df}{dx}
=
4(12x + 7)(6x^2 + 7x)^3
$$

problem 2: 
$$
g(t) = (4t^2 -3t + 2)^{-2}
$$

$$
\frac{dg}{dt}
=
-2(8t-3)(4t^2-3t+2)^{-3}
$$

problem 3: 
$$
y = (1-8z)^{(1/3)}
$$

$$
\frac{dy}{dz}
=
(-8/3)(1-8z)^{(-2/3)}
$$

problem 4: 
$$
R(w) = csc(7w)
$$

$$
\frac{dR}{dw}
= -7csc(7w)cot(7w)
$$

problem 5:
$$
G(x) = 2sin(3x+tan(x))
$$

$$
G'(x) = 2\left(3+\sec^2(x)\right)\cos\left(3x+\tan(x)\right)
$$

problem 6:
$$
h(u) = tan(4+10u) 
$$

$$
h'(u) = 10\sec^2(4+10u)
$$

problem 7:
$$
f(t) = 5 + e^{4t + t^7}
$$

$$
f'(t) = (4+7t^6)e^{4t+t^7}
$$

problem 8:
$$
g(x) = e^{1-cos(x)}
$$

$$
g'(x) = sin(x)e^{1-cos(x)}
$$

problem 9:
$$
u(t) = tan^{-1}(3t-1)
$$

$$
u'(t)=\frac{3}{(3t-1)^2+1}$$

problem 10: 
$$
F(y) = ln(1-5y^2+y^3)
$$

$$
F'(y) = \frac{-10y+3y^2}{1-5y^2+y^3}
$$

problem 11:
$$
q(t) = t^2ln(t^5)
$$

$$
q'(t) = 2tln(t^5) + 5t
$$

problem 12:
$$
S(w) = \sqrt{7w} + e^{-w}
$$

$$
S(w)'= \frac{7}{2\sqrt{7w}} - e^{-w}
$$

problem 13:
$$
f(x) = \cos\left(x^2 e^x\right)
$$

$$
f'(x) = -\left(2xe^x + x^2e^x\right)\sin\left(x^2e^x\right)
$$

problem 14:
$$
g(z) = 3z^7-sin(z^2+6)
$$

$$
g'(z) = 21z^6+2zcos(z^2+6)
$$

problem 15:
$$
f(x) = \ln(\sin(x)) - (x^4 - 3x)^{10}
$$

$$
f'(x) = cot(x)-10(4x^3-3)(x^4-3x)^9
$$

problem 16:
$$
g(w) = cos(3w)sec(1-w) 
$$

$$
g'(w) = -3sin(3w)sec(1-w)-cos(3w)sec(1-w)tan(1-w)
$$

problem 17:
$$
z = \sqrt{5x + \tan(4x)}$$

$$
z' = \frac{1}{2}\left(5x + \tan(4x)\right)^{-1/2}\left(5 + 4\sec^2(4x)\right)
$$

problem 18:
$$
f(t) = \left(e^{-6t} + \sin(2 - t)\right)^3
$$

$$
f'(t)=3\left(e^{-6t}+\sin(2-t)\right)^2\left(-6e^{-6t}-\cos(2-t)\right)
$$

problem 19:

$$
y=\frac{\sin(3t)}{1+t^2}
$$

$$
y' =
\frac{
(1+t^2)\left(3\cos(3t)\right)-\sin(3t)\left(2t\right)
}{
(1+t^2)^2
}
$$

