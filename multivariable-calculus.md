
A function maps every element in set X to an element in set Y. set X is called the domain of the function and the codomain of the function is set Y. The range of the function is a subset of the codomain of the function that is actually used. The codomain of the function and the range of the function can be the same. The graph of a function is the visual representation of it. f(x) represents the mapping value of each x. 

  $$
\begin{aligned}
1 &\rightarrow 4 \\
2 &\rightarrow 5 \\
3 &\rightarrow 6
\end{aligned}
$$

We have a function here. What kind of function is this? This function is an injective function.
Is this function also a surjective function? This function is also a surjective function. By definition, 
this function is a bijective function. Now, let's look at another function below.

$$
\begin{array}{ccc}
1 & \rightarrow & 4 \\
2 & \rightarrow & 5 \\
  & \nearrow & \\
3 & & 6
\end{array}
$$


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

This formal definition of finite limit is not easy to understand initially but now I definitely have a better understanding of it. 
The following link can be helpful for understanding the definition since it contains a visual representation. The key to understanding this definition was to think of the "if" condition abstractly. It is said that "understanding this definition is the key that opens the door to a better understanding of calculus". 


[Formal Definition of a Limit (LibreTexts)](https://math.libretexts.org/Courses/Mount_Royal_University/Calculus_for_Scientists_I/2%3A_Limit__and_Continuity_of_Functions/2.5%3A_Formal_Definition_of_a_Limit_%28optional%29)

## The definition of the derivative of f at a

$$
f'(a) = \lim_{h \to 0} \frac{f(a+h)-f(a)}{h}
$$
