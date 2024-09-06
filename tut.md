## Extracting out recurrence relation from recursive function.

Each element is defined by recurrence relation.
Representation of Time taken by recursive algo

```Python
def test(n):
    if(n>0):
        print(n)
        test(n-1)
```

If this algo take time T(n)

T(n-1) is 1
when n = 0

there is always atleast one comparison
comparisons | n
T(n) | 1 0

T(n) = T(n-1) + 1

_for n-1_

T(n-1) = T(n-1-1) + 1
T(n-1) = T(n-2) + 1

# Types of recurrence relation

## 1. Linear Recurrence Relation-> Substitution method

## 2. Divide and Conquer

T(n) = 2T(n/2) +Cn

## 3. Substitution Recurrence/ Master Theorem

```
T(n) = T(sq(n) + 1)
```

## 4. Homogenous Recurrence Relation

_Master Method_ is most common.
