
# Lab: probability via outcomes

Key point of this lab: if we have a sample space where each outcome is equally likely:

$P(\text{each outcome}) = \dfrac{1}{\mid S \mid}$

where $\mid S \mid$ is the cardinality of $S$, in other words, the number of possible outcomes in the sample space.
then

$P(E) = \dfrac{ \text{number of outcomes in E} }{\text{number of outcomes in S}}= \dfrac{\mid E \mid}{\mid S \mid}$

## Exercise 1

In this exercise, we'll look at possible outcomes when throwing a dice twice.

Next, we'll compute a couple or probabilities associated with doing this.
First, let's create the sample set as a numpy array below.


```python
import numpy as np
sample_dice = None
```

Look at the shape of the array to reassure we haven't made any mistakes.


```python
None # should be equal to (36,2)
```

Use Python to obtain the following probabilities:

#### a. What is the probability of throwing a 5 at least once?

First, use sample_dice to get "True" values for each time a 5 occurs.


```python
set_5 = None
```

Next, make sure that you get a value `True` for each pair where at least one 5 was thrown.


```python
true_5 = None
print(true_5)
```

Applying the `sum()` function you can get to the total number of items in the event space. Divide this by the total number in the sample space.


```python
prob_5 = None
print(prob_5)
```

#### b. What is the probability of throwing a 5 or 6 at least once?


```python
set_5 = None
set_6 = None
```


```python
set_5_6 = None
```


```python
set_any_5_6 = None
print(set_any_5_6) 
```


```python
prob_5_6 = None
print(prob_5_6)
```

#### c. What is the probability of the outcome having a sum of exactly 8?


```python
sum_dice = None
sum_8 = None
```


```python
prob_sum_8 = None
print(prob_sum_8)
```

# Exercise 2

At a supermarket, we randomly select customers, and make notes of whether a certain customer owns a Visa card (event A) or an Amex credit card (event B). Some customers own both cards.
You can assume that:

- P(A) = 0.5
- P(B) = 0.4
- both A and B = 0.25.

1) compute the probability that a selected customer has at least one credit card.

2) compute the probability that a selected customer doesn't own any of the mentioned credit cards.

3) compute the probability that a customer *only* owns VISA card.

(You can use python here, but you don't have to)

# Exercise 3

A teaching assistant is holding office hours so students can make appointments. She has 6 appointments scheduled today, 3 by male students, and 2 by female students. 


```python
import numpy as np
```

NOTE: pretty brutal having them type it by hand, but will prove the point of what they'll see later


```python
sample_mf= None
```


```python
None # get the shape of sample_mf
```


```python
sample_length= None
print(sample_length)
```

#### 1. Calculate the probability that at least 2 out of the first 3 appointments are with female students

First, select the first 3 appointment slots and check for "F".


```python
first_3_F = None
None
```


```python
num_F = None
print(num_F)
```


```python
F_2plus = None
print(F_2plus)
```


```python
prob_F_2plus = None
print(prob_F_2plus)
```

#### 2. Calculate the probability that after 4 appointment slots, all the female students have had an appointment


```python
None
```

You noticed that coming up with the sample space was probably the most time-consuming part of the exercise, and it would really become unfeasible to write this down for say, 10 or, even worse, 20 appointments in a row. You'll learn about methods that make this easy in the next lecture!

## Sources

https://www.datacamp.com/community/tutorials/statistics-python-tutorial-probability-1

https://www.youtube.com/watch?v=oYXYLljkC48&index=2&list=PLcmJYc2muOR9H96hGlUBV2DkviVZFmHAh
