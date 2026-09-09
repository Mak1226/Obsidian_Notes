
## Probability Distribution

```python
import math
import statistics

ans = math.comb(25,20) * math.pow(0.9,20) * math.pow(0.1,5)
print(ans)
```


```python
import math
import statistics
s = 0
for i in range(20,26):
	s = s + math.comb(25,i) * (0.9 ** i) * (0.1 ** (25-i))
print(s)
```


### Poisson Distribution

discrete distribution and refers to the number of events within a specific time provided or region of space
### Poisson Distribution
The probability of observing $k$ events in a fixed interval:
$$P(X = k) = \frac{\lambda^k e^{-\lambda}}{k!}$$

**Where:**
- $\lambda$: Average rate of occurrence
- $k$: Number of occurrences
- $e$: $\approx 2.71828$

> A stats instructor has observed that the no. of typographical errors in new editions of textbook varies considerably from book to book. After some analysis he concludes that the number of errors is poisson distribution with a mean of 1.5 per 100 pages. The instructor randomly selects 100 pages of a new book. What is the probability that there are no typos

```python
import math
import statistics
# P(X = 0)

ans = (1.5 ** 0) * (math.e ** -1.5) / 1 # 0!
print(ans)
```

> What is the probability that there are 5 or less typos?

```python
import math
import statistics
# P (X = 0)
s = 0
for i in range(0,6):
	s = s + (math.e ** -6) * (6**i) / math.factorial(i)
	
print(s)
```

> After conducting a survey of golfers, a stats conclude that the no. of lost balls in a round is PD with a mean of 2. Find the probability of the following event

- A golfer loses no golf balls

```python
# P (X = 0)
ans = math.e ** -2 * 2 ** 0 / math.factorial(0)
print(ans)
```
## Continuous Probability Distribution

unlike a discrete random variable which we studies in last chapter, a continuous random variable is one that can assume an uncountable number of values.

**Thus, we can determine the probability of a range of values only**

### Uniform distribution

Its given by the formula

### Uniform Distribution
The probability density function is:
$$f(x) = \frac{1}{b - a} \quad \text{for } a \le x \le b$$

**Key Measures:**
- **Mean:** $\mu = \frac{a + b}{2}$
- **Variance:** $\sigma^2 = \frac{(b - a)^2}{12}$

> The amt of gasoline sold daily at service station is uniformaly distributed with a min of 2000 gallons and a max of 5000 gallons. Find the prob. that daily sales will fall b/w 2500 & 3000 gallons?

$$\frac{1}{5000 - 2000} \cdot (3000 - 2500) = 0.1667$$

> What is prob. that the service station will sell atleast 4K gallons?

$$\frac{1}{5000 - 2000} \cdot (5000 - 4000) = 0.3333$$
> What is the prob. that station will sell exactly 2500 gallons?

$$\text{0}$$
### Normal Distribution

most imp prob distribution. The prob density function of normal random variable is given by:

### Normal Distribution Formula
The probability density function for a normal distribution:
$$f(x) = \frac{1}{\sigma\sqrt{2\pi}} e^{-\frac{1}{2}\left(\frac{x-\mu}{\sigma}\right)^2}$$

**Key Parameters:**
- $\mu$: Mean (average)
- $\sigma$: Standard deviation (spread)
- $\sigma^2$: Variance

### Standard Normal Distribution

A normal distribution whose mean is zero and standard deviation is one is called the standard normal distribution.

### Standard Normal Distribution
$\mu = 0$
$\sigma = 1$

### Convert Normal Distribution into Standard Normal Distribution

### Z-Score Formula
Used to standardize data to a standard normal distribution:
$$z = \frac{x - \mu}{\sigma}$$


> The daily demand of a  gas station for regular gasoline is normally distributed with a mean of 1000 gallons and a std dev of 100 gallons. the station manager has just opened the station for business and notes that there is exactly 1100 gallons of regular gasoline in storage. The next delivery is scheduled later today at close of business. The manger would like to know the probability that he will have enough regular gasoline to satisfy today's demands.


### Standardizing Probability
To find the probability $P(X < 1100)$ given $\mu = 1000$ and $\sigma = 100$:

$$z = \frac{1100 - 1000}{100} = 1.00$$

Therefore:
$$P(X < 1100) = P(Z < 1.00)$$

