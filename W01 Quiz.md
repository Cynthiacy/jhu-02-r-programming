R Programming ��һ�� Quiz
===

[@������������ټ�](http://www.weibo.com/biobyelogy)


### Question 1
R was developed by statisticians working at

> �ع� PPT 01 Overview and History of R��PPT ��ֻ����ص�����������

===

### Question 2
The definition of free software consists of four freedoms (freedoms 0 through 3). Which of the following is NOT one of the freedoms that are part of the definition?

> �ع� PPT 01 Overview and History of R��

===

### Question 3
In R the following are all atomic data types EXCEPT

> �ع� PPT 03 Data Types�����ֻ����������͡�

===

### Question 4
If I execute the expression `x <- 4` in R, what is the class of the object `x` as determined by the `class()` function?

> �ع� PPT 03 Data Types��numeric �� integer ������

===

### Question 5
What is the class of the object defined by `x <- c(4, TRUE)`?

> �ع� PPT 03 Data Types��vector ��Ԫ������һ�¡���һ��ʱ����ǿ��ת����

===

### Question 6
If I have two vectors `x <- c(1, 3, 5)` and `y <- c(3, 2, 10)`, what is produced by the expression `cbind(x, y)`?

> �ع� PPT 03 Data Types������ `cbind` �� `rbind`��

===

### Question 7
A key property of vectors in R is that

> �ع� PPT 03 Data Types�������Ѿ��ἰ��

===

### Question 8
Suppose I have a list defined as `x <- list(2, "a", "b", TRUE)`. What does `x[[2]]` give me?

> �ع� PPT 04 Subsetting�������� subsetting operator �ǳ���Ҫ��
> - `[<expression>]` ���ط��� `<expression>` ���Ӽ���������ȫ����ͬ��
> - `[[<expression>]]` ���ط��� `<expression>` �ĵ���Ԫ�أ�����Ϊ����Ԫ�����ͣ�
> - `$<name>` ���� `<name>` ָ��ĵ���Ԫ�أ�����Ϊ����Ԫ�����͡������ܱ��ʽ��

===

### Question 9
Suppose I have a vector `x <- 1:4` and `y <- 2:3`. What is produced by the expression `x + y`?

> �� RStudio console ����һ�¼��ɣ�����Ҫ��ס��

===

### Question 10
Suppose I have a vector `x <- c(17, 14, 4, 5, 13, 12, 10)` and I want to set all elements of this vector that are greater than 10 to be equal to `4`. What R code achieves this?

> - `[<expression>]` ���ط��� `<expression>` ���Ӽ���
> - `==` ���߼��жϷ��ţ�`<-` ���� `=` ���Ǹ�ֵ��

===

### Question 11
In the dataset provided for this Quiz, what are the column names of the dataset?

> - д����֮ǰע�⵱ǰ `working directory`�����ú��� `setwd ���ã�
> - ���� `read.csv`��
> - ���� `colnames`��
> - ����ʵ�����������С���

===

### Question 12
Extract the first 2 rows of the data frame and print them to the console. What does the output look like?

> ���� `head`��

===

### Question 13
How many observations (i.e. rows) are in this data frame?

> - ���� `nrow`��
> - ����ʵ��һ��ѡ����Ҳ�С���

===

### Question 14
Extract the last 2 rows of the data frame and print them to the console. What does the output look like?

> ���� `tail`��

===

### Question 15
What is the value of `Ozone` in the 47th row?

> ��ѡ�� `Ozone`����ѡ���� 47 �����ݡ�

===

### Question 16
How many missing values are in the `Ozone` column of this data frame?

> ���ⷽ���ܶ࣬�����������
> ����һ��
> - �ú��� `na.omit` �õ�ȥ�� `NA` ��� `data$Ozone` ������
> - �ú��� `length` �õ�������Ԫ�ظ������Ͱ��� `NA` �� `Ozone` ����������Ƚϡ�
>
> ��������
> - ��ѡ�� `Ozone`��
> - �ú��� `is.na` �õ�һ�� `Ozone` ���Ƿ��� `NA` �� `logical` ������
> - �����У�`TRUE` �൱�� `1`��`FALSE` �൱�� `0`���� `sum` ��͵õ� `TRUE` ������

===

### Question 17
What is the mean of the `Ozone` column in this dataset? Exclude missing values (coded as `NA`) from this calculation.

> ���� `mean` ��һ��ѡ�� `na.rm = T`�����ڼ���ʱȥ�� `NA` Ԫ�ء�

===

### Question 18
Extract the subset of rows of the data frame where `Ozone` values are above `31` and `Temp` values are above `90`. What is the mean of `Solar.R` in this subset?

> �����кܶ෽����
> ����һ��
> - ������ `data$Ozone > 31 & data$Temp > 90` ѡ������� `data$Solar`��
> - ע�� `&` �� `&&` ������ǰ�߷���һ�����������߷��ص�һ `logical` ֵ��������������� `&`��
> - ���ú��� `mean`��
>
> ��������
> - �ú��� `subset` ѡ������� `Solar` ���ݣ�
> - ���ú��� `mean`��

===

### Question 19
What is the mean of `Temp` when `Month` is equal to `6`?

> �������⡣ע�� `==` ���߼��жϷ���`=` �Ǹ�ֵ���ţ����������ǰ�ߡ�

===

### Question 20
What was the maximum `ozone` value in the month of May (i.e. `Month = 5`)?

> �������⡣

