# Hypothesis Testing

A criminal trial is an example of hypotheses testing without the statistics

In a trial a jury must decide between two hypothesis, the null hypothesis is:

```yaml
H_o = The defendant is innocent -> null hypothesis
H_1 = The defendent is guilty -> alternative or research hypothesis
```

> The manager of a dept store is thinking about est. a new billing system for the store's credit customers. Mean monthly acc is $170. She determines that the new system will be cost effective only if the mean monthly acc is more than $170. A random sample of 400 monthly acc is drawn for which the sample mean is $178. The manager knows that the acc are approx normally distributed with std. dev of $65. Can the manager conclude from this that the new system will be cost effective?

```python
import statistics
import math

s = (178 - 170) / (65 / math.sqrt(400))
print(s)
```

> FedEx sends invoices to customers requesting payment within 30 days. The bill lists an address and customers are expected to use their own envelopes to return their payments. Currently the mean and std dev. of amt of time taken to pay bills are 24 days and 6 days resp. The CFO believes that including a stamped self addressed envelope would decrease the amt of time.

> She calculates that the improved cash flow from a 2 day decrease in the payment period would pay for the costs of the envelopes and stamps. Any further decrease in the payment period would generate a profit. 

```python
import statistics
import math

x = [27, 24, 14, 39, 13, 31, 26, 33, 13, 23, 17, 24, 18, 34, 13, 23, 16, 32, 30, 29, 21, 19, 22, 14, 27, 20, 11, 20, 30, 24, 18, 21, 24, 18, 27, 27, 27, 21, 22, 23, 18, 17, 23, 26, 20, 20, 22, 21, 13, 36, 18, 25, 26, 19, 16, 28, 16, 20, 16, 14, 25, 14, 35, 17, 16, 19, 19, 17, 18, 22, 23, 22, 27, 23, 23, 21, 20, 18, 29, 32, 27, 15, 21, 26, 32, 20, 29, 25, 15, 21, 30, 24, 23, 14, 18, 22, 37, 24, 35, 29, 24, 17, 27, 15, 19, 12, 19, 21, 19, 21, 15, 17, 20, 21, 31, 19, 27, 19, 26, 26, 26, 23, 12, 20, 34, 21, 24, 20, 21, 16, 23, 13, 19, 18, 31, 29, 23, 28, 19, 19, 22, 24, 21, 23, 14, 25, 17, 22, 21, 18, 22, 15, 27, 14, 23, 25, 24, 24, 17, 16, 30, 24, 17, 27, 24, 17, 10, 25, 15, 13, 29, 21, 22, 11, 25, 30, 23, 18, 19, 18, 14, 21, 22, 17, 19, 23, 31, 26, 25, 15, 16, 28, 27, 22, 12, 25, 12, 21, 19, 26, 16, 21, 30, 16, 25, 13, 11, 13, 22, 28, 14, 21, 30, 19, 14, 31, 9, 14, 21, 28]

m = statistics.mean(x)
print(m)
print(len(x))
```


### Hypothesis

- **Null Hypothesis ($H_0$):** $\mu = 22$
- **Alternative Hypothesis ($H_1$):** $\mu < 22$ (Left-tailed test)

```python
import statistics
import math

s = (21.63 - 22) / (6 / math.sqrt(220))
print(s)
```



