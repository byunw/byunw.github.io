
A function maps every element in set X to an element in set Y. set X is called the domain of the function and the codomain of the function is set Y. The range of the function is a subset of the codomain of the function that is actually used. The codomain of the function and the range of the function can be the same. The graph of a function is the visual representation of it. f(x) represents the mapping value of each x. 

  $$
\begin{aligned}
1 &\rightarrow 4 \\
2 &\rightarrow 5 \\
3 &\rightarrow 6
\end{aligned}
$$

We have a function here. What kind of function is this? This function is an injective function since every element in the domain 
of the function is mapped to a distinct element. 
Is this function also a surjective function? This function is also a surjective function since every element in the codomain of the function
has at least 1 element in the domain that maps to it. By definition, 
this function is a bijective function. Now, let's look at another function below.

$$
\begin{array}{ccc}
1 & \rightarrow & 4 \\
2 & \rightarrow & 5 \\
  & \nearrow & \\
3 & & 6
\end{array}
$$

This function is not an injective function because two different elements in the domain of the function
point to the same element. Then, is this function a surjective function? This function is not a surjective function.
There is no element in the domain of the function that maps to 6. By definition, this function
is not a bijective function (A function has to be both injective and surjective to be a bijective function).

## Function Composition
Let's assume two functions f: X->Y and g: Y->Z.
we define g ∘ f: X -> Z as the following: g(f(x)).


## Inverse Function
Given a function $$f$$ with domain $$D$$ and range $$R$$, its inverse function $$f^{-1}$$ has domain $$R$$ and range $$D$$, such that $$f^{-1}(y) = x$$ if $$f(x) = y$$.


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


## What is the formal definition of continuity?
  
$$
\begin{aligned}
&\text{A function } f \text{ is continuous at } a \text{ if and only if:}\\
&\text{(i)}\quad f(a) \text{ is defined}\\
&\text{(ii)}\quad \lim_{x \to a} f(x) \text{ exists}\\
&\text{(iii)}\quad \lim_{x \to a} f(x)=f(a)
\end{aligned}
$$

Now we have the formal definition of continuity written down above, let's find out if a function is continuous at a point.
Let's look at the following function.  

$$
\begin{aligned}
1 &\rightarrow 4 \\
2 &\rightarrow 5 \\
3 &\rightarrow 6
\end{aligned}
$$

Is this function continuous at 4? The function is not defined at 4 and the function is not continuous at 4.
The function is defined at 1. The function is defined at 2. The function is defined at 3. Now, let's find out a point where the function is continuous!



## The definition of the derivative of f at a

$$
f'(a) = \lim_{h \to 0} \frac{f(a+h)-f(a)}{h}
$$
