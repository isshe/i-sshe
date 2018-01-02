# i-sshe

## 1. 初心
* 把自己学习到的知识，写成一个程序
* 实现一个代表自身能力的项目，不断把学习到的东西加到这个项目中，最终成为一个可用的系统。
* 每年写几个功能

## 2. 架构
### 2.1 微服务架构
> http://dockone.io/article/394  
> https://www.nginx.com/blog/introduction-to-microservices/  
### 2.2 实际做法
* 每种服务都有自己的数据库
* 冗余的代码抽出来放到公共库

### 2.3 模式拓扑
最常见和流行的拓扑结构有3种：
* 基于REST API的拓扑结构
    * 适用于网站，通过某些API对外提供小心的、自包含的服务。
* 基于REST的应用拓扑结构
    * 常见于中小型企业等复杂程序相对较低的应用程序。
* 集中式消息拓扑结构
    * 通常应用在较大的业务应用程序中。

### 2.4 避免依赖和编排
* 主要挑战：
    * 决定服务组件的粒度级别

* 粒度判断技巧
    * 如果发现需要从应用内部的用户接口或API层编排服务组件，那么可能服务组件的粒度太细了。
    * 如果发现需要在服务组件之间执行服务间通信来处理单个请求，那么可能服务组件的粒度太细了。





### 2.9 可能要继续了解的内容
* 远程访问协议：JMS, AMQP, REST, SOAP, RMI等
    * REST: https://www.zhihu.com/question/28557115
* 集中式消息代理：ActiveMQ，HornetQ等
* 服务间通信：可能导致组件之间产生耦合，可以通过共享数据库进行处理。

## 3.模块/功能
> 思路：一个功能一个模块，一个服务一个模块

* mqtt
* rpc
* 内网穿透
* 单元测试
* 调试模块：log
* 测试模块：性能测试
* 导入/导出模块：配置、数据
* 通知模块（notification）：

## 4.要求/想法
* 详尽的文档
* 不妥协
* 对实现得不好的地方进行重构
* 为了充分理解计算机语言，可以不同的模块/服务采用不同的语言实现。

## 5.涉及知识点
* rpc
* mqtt
* tcp
* udp
* 线程池
* 内存池


## 6.附录A:表现
* 移植性
* 稳定性
* 拓展性





