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
 

this recursive binary search helps identify which is the highest floor eggs can be dropped
without them breaking. it has a runtime complexity of O(log n)


binary search through the _n_ floors
    set variable middle to //2 _n_ floors
        drop egg:
            if egg breaks:
                if egg breaks:
                    go through bottom half and set middle to its middle most value:
                else:
                    go through top half and set middle to its middle most value:
s


