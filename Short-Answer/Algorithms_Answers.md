## Exercise I

```
a)  a = 0
    while (a < n * n * n):
      a = a + n * n
```
Exercise I part a has a runtime of O(n)

```
b)  sum = 0
    for i in range(n):
      i += 1
      for j in range(i + 1, n):
        j += 1
        for k in range(j + 1, n):
          k += 1
          for l in range(k + 1, 10 + k):
            l += 1
            sum += 1
```
Exercise I part b has a runtime of O(n^3)

```
c)  def bunnyEars(bunnies):
      if bunnies == 0:
        return 0

      return 2 + bunnyEars(bunnies-1)

Exercise I part c has a runtime of O(n)



## Exercise II
  -  _n_ story building
  -  eggs break on floor _f_ or higher
  -  egg doesn't break below floor _f_
 

<!-- First Pass--time complexity O(n^2)  -->

egg_thrower_count(n_floors):
    count = 0
    for n_floor in n_floors:
        while count < n_floor:
            count + 1
    return count

<!-- Second Pass -->