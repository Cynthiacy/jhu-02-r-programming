R Programming ������ Quiz
===

[@������������ټ�](http://www.weibo.com/biobyelogy)


### Question 1
Take a look at the 'iris' dataset that comes with R. The data can be loaded with the code:
```R
library(datasets)
data(iris)
```
There will be an object called 'iris' in your workspace. In this dataset, what is the mean of 'Sepal.Length' for the species virginica? (Please only enter the numeric result and nothing else.)

> �� `split` ������ `iris` ���� `Sepal.Length` ���飬���Ϊһ�� `list`��ѡ�� `list` �� `virginica` ��һ�飬���� `mean` ������

===

### Question 2
Continuing with the 'iris' dataset from the previous Question, what R code returns a vector of the means of the variables 'Sepal.Length', 'Sepal.Width', 'Petal.Length', and 'Petal.Width'?

> �ع� PPT 02 apply��`apply(���ݼ�, ά��, ����, ...)`��

===

### Question 3
Load the 'mtcars' dataset in R with the following code
```R
library(datasets)
data(mtcars)
```
There will be an object names 'mtcars' in your workspace. How can one calculate the average miles per gallon (mpg) by number of cylinders in the car (cyl)?

> �ع� PPT 03 tapply��`tapply(���ݼ�, ����, ����, ...)`��

===

### Question 4
Continuing with the 'mtcars' dataset from the previous Question, what is the absolute difference between the average horsepower of 4-cylinder cars and the average horsepower of 8-cylinder cars?

> �������һ�����ơ��ó�ƽ��ֵ֮�����ȡ����ֵ��

===

### Question 5
If you run `debug(ls)`, what happens when you next call the 'ls' function?

> �ع� PPT 06 debugging��ע��ʹ�� `Q` �����˳� `browser`��



