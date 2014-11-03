R Programming ������ Assignment
===

��һ�ܷų��� Programming Assignment 2 �ǹ��� cache �ġ���ҵ��ʵ�ܼ򵥣�����ֻҪ�ճ����������Ӿ��У����ǳ�ѧ�߿��ܲ�̫������⣬�����������һ���������롣

```r
# ��������ڲ�һ��������������x �� m��
# x ����Ҫ����� numeric vector������������ʵҲ���ԣ���
# m �����洢����֮��Ľ����
makeVector <- function(x = numeric()) {
  # �����ڲ�����ı���
  m <- NULL
  
  # ������ֵ�ĺ�����"<<-" ��ȫ�ָ�ֵ���š�
  # һ��ĸ�ֵ��"��" ���� "<-"��ֻ���ڵ�ǰ�����ڲ����ֲ����Է��Ÿ�ֵ��
  # ������Ų����ڣ��򴴽��µķ��š�
  # �� "<<-" ������ȫ�ֵķ��Ž��и�ֵ��
  # ���Դ˺������ y ��ֵ���� makeVector ��������� x��
  # �������� set �����ڲ�����һ���µķ��� x���� m ��Ϊ NULL��
  set <- function(y) {
    x <<- y
    m <<- NULL
  }
  
  # ��ֵ���������� x������Ҫ��������ݡ�
  get <- function() x
  
  # �� mean ��ֵ���� m�������洦��֮��Ľ����
  setmean <- function(mean) m <<- mean
  
  # ��ֵ���������� m������������
  getmean <- function() m
  
  # ���� makeVector ���ص���һ�� list�����й����ĸ�Ԫ�أ�
  # ÿ��Ԫ�ض���֮ǰ�������һ��������
  list(set = set,
       get = get,
       setmean = setmean,
       getmean = getmean) 
}

# �˺������������ x ������һ�� makeVector��
cachemean <- function(x, ...) {
  # x ����һ�� makeVector��
  # x$getmean ���ǵ��� makeVector �е� getmean ������
  # Ҳ�����Ȳ�ѯһ��֮ǰ��û�м���� mean ֵ��
  m <- x$getmean()
  if(!is.null(m)) {
    # m ���� NULL��˵��֮ǰ�Ѿ������ mean ֵ�ˣ�
    # ֱ�ӷ��ؽ����
    message("getting cached data")
    return(m)
  }
  
  # �������ִ�е���һ����˵��֮ǰû�м���� mean��
  # ���� x �ڲ��� get �������� x �е�����Ҫ��������ݡ�
  data <- x$get()
  # ���� mean ֵ��
  m <- mean(data, ...)
  # ���� x �ڲ��� setmean ���������õ��Ľ�����浽 x ����ȥ��
  # �´ε��� cachemean ��ʱ��x �Ѿ������˽����
  # cachemean ��������֮ǰ�� if ��ѯ��ֱ�ӷ��أ�����Ҫ�ټ����ˡ�
  x$setmean(m)
  # ���ؽ����
  m
}
```

��������������õģ�
```r
numbers = seq(1, 10)
cachedNumbers = makeVector(numbers)
cachemean(cachedNumbers)
cachemean(cachedNumbers)
```

`cachemean` �������������Σ���һ��ֱ����ʾ��� `5.5`���ڶ����ȵõ�һ�� message��`getting cached data`��Ȼ������������Ҳ����˵��һ�ε���ʱ�Ľ���Ѿ����棬�Ժ����۵��ö��ٴΣ�������Ҫ�����ˡ�

Cache ˵���׷ǳ��򵥣�����ÿ����Ҫ�����ʱ���ȿ�����ǰ��û�м�������еĻ�ֱ�ӷ��أ������ټ��㲢�ѽ����������
