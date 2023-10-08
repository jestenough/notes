# Python core

## **Strings**

In Python string of **str** type represents **single characters** each of which is an object of str type with length is **1**. This means that each character in string is an individual object of **str** type whether how much string contain characters

## Generators

You can omit the parentheses surrounding **generator-expression** if expression is used as **single** argument of function.

```python
>>> sum((x * 2 for x in range(10))) 
90 
## Compare with
>>> sum(x * 2 for x in range(10)) 
90
```