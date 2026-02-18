## Basic Bitwise Operators
```
# AND (&) - both bits are 1
5 & 3   # 101 & 011 = 001 = 1

# OR (|) - at least one bit is 1
5 | 3   # 101 | 011 = 111 = 7

# XOR (^) - bits are different
5 ^ 3   # 101 ^ 011 = 110 = 6

# NOT (~) - flips all bits (two's complement)
~5      # -(5+1) = -6

# Left Shift (<<) - shift bits left
5 << 1  # 101 << 1 = 1010 = 10

# Right Shift (>>) - shift bits right
5 >> 1  # 101 >> 1 = 10 = 2
```
## Useful Bit Tricks for Your Problem

```
# Check if a number is a power of 2
n & (n - 1) == 0

# Get the rightmost set bit
n & -n

# Clear the rightmost set bit
n & (n - 1)

# Check if bits alternate (relevant to your problem!)
(n ^ (n >> 1)) & ((n ^ (n >> 1)) + 1) == 0
```