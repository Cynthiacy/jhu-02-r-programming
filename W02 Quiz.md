R Programming �ڶ��� Quiz
===

[@������������ټ�](http://www.weibo.com/biobyelogy)


### Question 1
Suppose I define the following function in R
```R
cube <- function(x, n) {
    x^3
}
```
What is the result of running `cube(3)` in R after defining this function?

>  �ع� PPT 02 Functions��֪ʶ�� lazy evaluation��

===

### Question 2
The following code will produce a warning in R.
```R
x <- 1:10
if(x > 5) {
    x <- 0
}
```
Why?

> `if` ���ж��������Ψһ����������һ��������

===

### Question 
Consider the following function

```
f <- function(x) {
    g <- function(y) {
        y + z
    }
    z <- 4
    x + g(x)
}
```

If I then run in R
```
z <- 10
f(3)
```
What value is returned?

> �ع� PPT 04 Scoping Rules��֪ʶ�� lexical scoping��������ֵ�ͺ�������һ������һ�� closure�����ɱ�����ֵ����ȡ���ں���������ʱ���Ǳ������ֵ�������Ǻ���������ʱ��ֵ�������У�`z` �� `f` ������ʱ���и�ֵ `z <- 4` ������ `f` ������ʱ `z <- 10` ���������á�

===

### Question 4
Consider the following expression:
```R
x <- 5
y <- if(x < 3) {
    NA
} else {
    10
}
```
What is the value of 'y' after evaluating this expression?

> �ع� PPT 01 Control Structures��`if` �ṹ��ֱ�����ڸ�������ֵ��

===

### Question 5
Consider the following R function
```
h <- function(x, y = NULL, d = 3L) {
    z <- cbind(x, d)
    if(!is.null(y))
        z <- z + y
    else
        z <- z + f
    g <- x + y / z
    if(d == 3L)
        return(g)
    g <- g + 10
    g
}
```
Which symbol in the above function is a free variable?

> �ع� PPT 04 Scoping Rules���ں��������У��������⣬û����ȷֵ�ı����������ɱ�����

===

### Question 6
What is an environment in R?

> �ع� PPT 04 Scoping Rules��

===

### Question 7
The R language uses what type of scoping rule for resolving free variables?

> �ع� PPT 04 Scoping Rules��

===

### Question 8
How are free variables in R functions resolved?

> �ع� PPT 04 Scoping Rules��

===

### Question 9
What is one of the consequences of the scoping rules used in R?

> �ع� PPT 04 Scoping Rules��

===

### Question 10
In R, what is the parent frame?

> �ع� PPT 04 Scoping Rules��