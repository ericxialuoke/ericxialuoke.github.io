---
title: 时间片轮转问题的解决
cover: https://qiniu.sukoshi.xyz/src/images/68686407_p0.jpg
tag: 
   - 时间片
   - 调度算法
category: 
          - 操作系统
---

```java
**0  1  2  3  4  5  6  7  8  9  10  11  12  13  14 15  16  17  18  19  20**

---

1  2  1  3  4  1  5  3  1  5   1    5    1     5    1   5    1    1     1    **1**

​    1  3  4  1  5  3  1  5   1  5  1  5  1  5  1

​            1  5  3  1  5                                                 **5**

​         **2**     3              **3**

​                      **4**

​                        

1:19   1.9 

2:2    2

3:8     4

4:5     6

5:16    2.8

平均周转时间：
```

{%  image
    url="https://qiniu.sukoshi.xyz/src/images/68686407_p0.jpg"
    title="带描述带图片"
%}
