# Recursion

It is a concept in computer science when a function calls itself and loops until it reaches the desired end condition.

![Screenshot 2024-05-12 143157](https://github.com/Ayush-Patel-1310/Basics-and-DSA/assets/118926325/f50c47e8-defc-4eff-b3ef-5c90f9a9f5c2)

It results in similar behavior to ```for``` or ```while``` loops, except recursion progresses closer to a target condition, while ```for``` loops run a set number of times, and ```while``` loops run until a condition is no longer met.

### Pros

 + Faster when optimized
 + Less code
 + Declarative
 + Efficient Sort and Search

### Cons

 + Maximum recursion depth 
 + Supported, not suggested
 + Uses more memory

```
def printPattern(targetNumber) :
  
  # Base Case
  if (targetNumber <= 0) :
    print(targetNumber)
    return
 
 # Recursive Case
  print(targetNumber)
  printPattern(targetNumber - 5)
  print(targetNumber)
 
# Driver Program 
n = 10
printPattern(n)
```

#### Output:-

```10 5 0 5 10```




