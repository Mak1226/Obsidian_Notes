
# Measure of relative standing

Comparing one with respect to the other: 
- percentile: 25%, 50%, 75% are called **quartiles**

```python
import statistics
x = [0,7,12,5,33,14,8,0,9,22]
x = sorted(x)
n = len(x)
L1 = (n+1)*(25/100)
L2 = (n+1)*(50/100)
L3 = (n+1)*(75/100)
print(f"1st Quartile {L1}")
print(f"2nd Quartile {L2}")
print(f"3rd Quartile {L3}")
```

3rd Quartile: 14 + 2(22-14=8\*0.25) = 16

Similarly for 1st and 2nd Quartile

## Box Plot

```latex
Interquartile Range = $Q_3$ - $Q_1$
```




```python
x = 201 * 0.25
y = 201 * 0.5
z = 201 * 0.75

print(x)
print(y)
print(z)
```

