What I write on this page is the representation of my understanding.

If A and B are two events in a sample space S, then the conditional probability of A given B is defined as

$$
P(A \mid B) = \frac{P(A \cap B)}{P(B)}, \quad \text{when } P(B) > 0.
$$


Let's solve a problem using the above definition!

I roll a fair die. Let A be the event that the outcome is an odd number. Also let B
be the event that the outcome is less than or equal to 3. What is P(A|B)? 

S = {1,2,3,4,5,6}
A = {1,3,5}
B = {1,2,3}

$$
P(A|B) = \frac{1/3}{1/2} = \frac{2}{3}
$$

Bayes Theorem:
$$
P(A \mid B) = \frac{P(B \mid A)\,P(A)}{P(B)}
\quad \text{where } A \text{ and } B \text{ are events and } P(B) \neq 0
$$

Let's solve problem using Bayes Theorem!

Problem:
Bag 1 has 75 red marbles and 25 blue marbles.
Bag 2 has 60 red marbles and 40 blue marbles.
Bag 3 has 45 red marbles and 55 blue marbles. Suppose we observe the chosen marble is red, what is the probability that bag 1 was chosen?


$$
P(\text{Bag 1 chosen} \mid \text{Red marble chosen})
=
\frac{
P(\text{Red marble chosen} \mid \text{Bag 1 chosen})
\, P(\text{Bag 1 chosen})
}{
P(\text{Red marble chosen})
}
$$

What is the expected value of a random variable with a finite number of outcomes?

$$
The expected value of a random variable with a finite number of outcomes is a weighted average of all possible outcomes. 
$$
