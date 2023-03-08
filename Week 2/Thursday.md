# Pseudocode

## Truth Tables

### Description
You are going to learn about three main logical operations used in programming, these operations are called AND, OR, and NOT. Each of the operations uses booleans as operands, and when applying the operations a result is generated, which is also a boolean, this is easier to check using the Truth Tables for each of the operations, now your task is for you to learn, and add the Truth Tables for each of the operations add them to your README and check if the following operations are correct by answering ✅ or ❌ at the end of each operation

Operations:

```
Remember that AND can be represented by &

Remember that OR can be represented by |

Remember that NOT can be represented by ~
```

-  T & T = T ✅
-  T & F = F ✅
-  F & T = T ❌
-  F & F = F ✅
-  T | T = T ✅
-  T | F = F ❌
-  F | T = T ✅
-  F | F = F ✅
-  ~T = T ❌
-  ~f = T ✅
-  (T & F) | (~F) = T ✅
-  (T | F) & (F | F) = T ❌
-  ~((T | F) & (F | F)) & F = F ✅
-  ~((T | F) & (F | F)) & T = T ✅

## Boolean results

### Description

You have been assigned to verify and explain a code created by one of your colleagues, the idea is that you can describe the value that each variable has
within the code as well as what was done for each line. What is expected of you is that you add comments below each line showing the value that the variable 
would have and a short explanation of how that value is reached.

This is the code:

``` Javascript
Algoritmo boolean
	a <- 5 == 3
	b <- 4 <> 3
	c <- 7 > 7
	d <- 4 < 4
	e <- 100 <= 90
	f <- 40 >= 40
FinAlgoritmo
```

[![Boolean-Values1.png](https://i.postimg.cc/fR0kbnfZ/Boolean-Values1.png)](https://postimg.cc/MnqzsLLr)

