
# Probability

### Relative frequency approach


$$\text{Relative Frequency} = \frac{\text{Frequency of Outcome}}{\text{Total Number of Observations}}$$ 

| Die Face | Freq |
| :------: | :--: |
|    1     |  6   |
|    2     |  8   |
|    3     |  10  |
|    4     |  7   |
|    5     |  8   |
|    6     |  10  |

$$\text{P(A) + P(A') = 1}$$ 
```python
x = [38.4, 3, 1.6, 1.4, 1.3, 1.1, 15.2]
total = 0
for i in x:
	total += i
print(total)

spanish = 38.4/total
print(spanish)
```

|                              | MF outperforms the market(B1) | MF doesn't outperforms the market(B2) | P(A) |
| :--------------------------: | :---------------------------: | :-----------------------------------: | :--: |
|   **T20 MBA Program (A1)**   |              .11              |                  .29                  | .40  |
| **Not T20 MBA Program (A2)** |              .06              |                  .54                  | .60  |
|           **P(B)**           |              .17              |                  .83                  | 1.00 |

### Conditional Probability

$$\text{P(A|B)} = \frac{\text{P(A and B)}}{\text{P(B)}}$$

> What is the probability that fund will outperform the market given that the manager graduated from the top 20 MBA program?

P(A|B) = 11/40

> What is the probability that a fund will not outperform the market given that the manger graduated from a top 20 program?

P(A|B) = 29/40

> Determine the probability that a fund outperforms or the manager graduated from a top 20 MBA program?

### Multiplication Rule

$$\text{P(A and B) = P(A|B) * P(B)}$$

> 7M & 3F. 2 stud: Prob that 2 stud are female

3/10 * 2/9 = 6/90

> Prob that choosing 2 stud will be female

3/10 * 3/10 = 9/100

### Addition Rule

### Addition Rule of Probability
For any two events A and B:
$$P(A \cup B) = P(A) + P(B) - P(A \cap B)$$

If A and B are mutually exclusive:
$$P(A \cup B) = P(A) + P(B)$$
### Bayes' Law

