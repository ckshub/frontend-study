## 一：区别

（1）post更安全（不会作为url的一部分，**不会被缓存**、保存在服务器日志、以及浏览器浏览记录中）

- 可以做个简短的测试，使用ajax采用get方式请求静态数据（比如html页面，图片）的时候，如果两次传输的数据相同，第二次以后消耗的时间将会在10ms以内（chrome测试），而post每次消耗的时间都差不多。

（2）post发送的数据更大（get有url长度限制）
（3）post能发送更多的数据类型（get只能发送ASCII字符）
（4）post比get慢
（5）post用于修改和写入数据，get一般用于搜索排序和筛选之类的操作（淘宝，支付宝的搜索查询都是get提交），目的是资源的获取，读取数据

（6）get的总耗是post的2/3左右



## 二：GET请求如何防止别人窃取信息

