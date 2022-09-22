# Complexity
## complexity of code (Software metrics)
* Cyclomatic complexity and others

## Big O notation (for time / space)
### How to find out (simple example)
* (1) find the fastest growing term (in terms of different functions)
* (2) neglect the coefficient (constant it is multiplied by)
### Operations with "sub-algorithms" of certain time complexity
* O(1) + O(1) => 2 * O(1) => neglecting coefficient => O(1)
* O(1) + O(n) => neglecting smaller => O(n)
### More parameters
* it is probably ok to do this - O(n*m) => O(n^2)

## Complexity Classes
* property of problem -> how much computational power/space is required to solve the problem
### Examples
* P (P-complete problems) - polynomial time
* NC - Nick's Class
* NP -
