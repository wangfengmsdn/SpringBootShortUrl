# 短域名服务

### 实现API接口

* 短域名存储接口：接受长域名信息，返回短域名信息。
* 短域名读取接口：接受短域名信息，返回长域名信息。
* 限制：短域名长度最大为8个字符

### 技术要点

* 框架:Spring Boot；
* 文档:Swagger API； 
* 访问路径：
* swagger2接口说明:
     [http://地址:端口/应用名/swagger-ui.html](http://127.0.0.1:8080/swagger-ui.html)
   
* swagger2接口源信息:
     [http://地址:端口/应用名/v2/api-docs](http://127.0.0.1:8080/v2/api-docs)

* 单元测试:JUnit;
* 测试报告:Jacoco(提交截图)；
* 映射数据:存储在JVM内存，防止内存溢出；

### 递交作业内容

* 源代码：(按照生产级的要求编写整洁的代码，使用gitignore过滤掉非必要的提交文件，如class文件)
* Jacoco单元测试覆盖率截图(行覆盖率和分支覆盖率85%+)
* 文档：完整的设计思路、架构设计图以及所做的假设(Markdown格式)
*     设计思路：
*     1、长链接进行变短存入HASHMAP，然后跟据短链接查找长链接
*     （自己先后写了单向链表、双向链表进行存储）实现
*     2、目前链接的数据格式面没有进行严格意义上的格式校准
*              

### 加分项

* 系统性能测试方案以及测试结果
* 系统性能测试方案：
*     1、写脚本对数据进行压力测试
*     2、从返回状态，丢包率等维度进行测试。

