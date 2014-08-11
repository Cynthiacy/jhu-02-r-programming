R Programming ������ Quiz
---

[@������������ټ�](http://www.weibo.com/biobyelogy)

---

### Question 1
What is produced at the end of this snippet of R code?
```R
set.seed(1)
rpois(5, 2)
```
> ����һ�¼��ɣ�˳��ع�һ�� `set.seed()` �����ã�PPT 01 Simulation����

---

### Question 2
What R function can be used to generate standard Normal random variables?

> �ع� PPT 01 Simulation���Ĵ����ͣ�`r`��`d`��`p`��`q`��

---

### Question 3
When simulating data, why is using the `set.seed()` function important?

> �ع� PPT 01 Simulation��

---

### Question 4
Which function can be used to evaluate the inverse cumulative distribution function for the Poisson distribution?

> �ع� PPT 01 Simulation �Ĵ����ͣ�ע���� ��inverse cumulative����

---

### Question 5
What does the following code do?
```R
set.seed(10)
x <- rbinom(10, 10, 0.5)
e <- rnorm(10, 0, 20)
y <- 0.5 + 2 * x + e
```

> �ع� PPT 01 Simulation��

---

### Question 6
What R function can be used to generate Binomial random variables?

> �ع� PPT 01 Simulation��

---

### Question 7
What aspect of the R runtime does the profiler keep track of when an R expression is evaluated?

> �ع� PPT 02 Profiler��

---

### Question 8
Consider the following R code
```R
library(datasets)
Rprof()
fit <- lm(y ~ x1 + x2)
Rprof(NULL)
```
(Assume that `y`, `x1`, and `x2` are present in the workspace.) Without running the code, what percentage of the run time is spent in the `lm` function, based on the `by.total` method of normalization shown in `summaryRprof()`?

> �ع� PPT 02 Profiler������ʹ�û��۶���Ľ��⼼�ɡ�

---

### Question 9
When using 'system.time()', what is the user time?

> PPT �Ͻ��ò��Ǻ���������� R �����ĵ���`system.time()` �ڳ������е�ͷ��β�������� `proc.time()` ����������õ�ʱ��`proc.time()` �������������
>
- ϵͳʱ�䣺the CPU time charged for the execution by the system on behalf of the calling process����ִ�еײ�ϵͳָ�������ѵ� CPU ʱ�䡣
- �û�ʱ�䣺the CPU time charged for the execution of user instructions of the calling process����ִ���û�ָ�������ѵ� CPU ʱ�䡣PPT �����Ϊ������ʽ�����ѵ�ʱ�䡣
- ����ʱ�䣺ʵ�����ĵ�ʱ��ʱ�䡣

---

### Question 10
If a computer has more than one available processor and R is able to take advantage of that, then which of the following is true when using `system.time()`?

> �ع� PPT 02 Profiler��