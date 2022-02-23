## spring-cloud-docker-microservice-book-code

一本书里的源码，我觉得还不错。具体url在这里

git@github.com:itmuch/spring-cloud-docker-microservice-book-code.git

可以使用ssl拉取。如果觉得慢的话可以去gitee上面搜索同名项目，一般比较出门的项目都会用，而且网速不用担心。不过我这次拉的好像“缺斤短两”

我大致的笔记，我就觉得重点在后面的config和zuul

### Eureka

本地package发现，空间一下子上去了。上次问我的那个不维护我真吓了一跳，不敢说自己关注动态连这都不知道。
使用rest端点注册微服务

### Ribbon负载均衡

怎么起来两个实例呢
就是改端口。。。。。。我决定不去做
最后一节讲了个ribbon没有eureka情况下的使用

### Feign声明式REST调用

Feign还可以控制日志
自定义配置优先级更高

### Hystrix对微服务容错处理

Rabbitmq在这里出现
要不要安装rabbitmq我犹豫了，果然没装
Spring cloud 默认为feign整合了hystrix，也可以配置一下全局禁用
也可以监控，可视化监控
Turbine聚合监控数据

### Zuul构建微服务网关

文件上传、过滤器等等、Sidecar整合非jvm访问JVM
使用zuul聚合微服务，这也许才是我要的
路由器配置详解注意一下
cloud 默认为zuul整合了hystrix，也可以配置一下全局禁用
也有高可用，最后的最后居然有node.js，我又犹豫了
聚合微服务一定要会，并且懂

### Spring cloud config 统一管理微服务配置

启动类声明，然后配置url和账号密码
还有加解密
编写configserver是基础吧
还有仓库配置，配合着和eureka使用

### Spring cloud sleuth 实现微服务跟踪

为什么里面提到八大误区；还说到ELK，安装我记得也是一行命令，
先不安装了吧；zipkin；这一块儿gitee居然偷工减料
