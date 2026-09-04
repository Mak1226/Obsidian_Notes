
```python
import math
import statistics as s

import statistics as s

a = [
    [17, 10, 13],
    [8, 4, 21],
    [6, 15, 8],
    [24, 12, 15]
]
print("mean")
r_mean = 0
for i in range(0,4):
	print(s.mean(a[i]))
	r_mean += s.mean(a[i])
	
r_mean /= 4
print(r_mean)
r_var = 0
print("variance^2")
for i in range(0,4):
	print(math.pow(s.variance(a[i]),2))
	r_var += 3 * math.pow(s.variance(a[i]),2)

print("SST")
r = 0
for i in range(0,4):
	r += 4 * math.pow(s.mean(a[i])-r_mean,2)
	
r /= 4
print(r)
print("SSE")
print(r_var)

F = (r/3)/(r_var/8)
print(F)
```


