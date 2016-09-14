
备注: Maven版本 3.0.X
#清空环境:
mvn clean 

打包+装配+安装二进制：
测试环境(常规）
mvn clean install -Denv=test
测试环境(特殊)
mvn clean install -Denv=special
测试环境(紧急）
mvn clean install -Denv=eme

线上环境
mvn clean install -Denv=prod 
开发环境
mvn clean install -Denv=dev
镜像环境
mvn clean install -Denv=img

=================================================================================================
更新记录：
2016-03-16
    1、monitorLog
    2、数据库Queue
    3、Logback MDC
2016-03-21
    1、Jetty发送、接受消息
2016-03-22
    1、Redis Pool
2016-03-25
    1、RateLimiter实现SLA限流
2016-03-30
    1、curator操作zookeeper
    2、HttpUtil
2016-03-31
    1、TaskUtil排他锁（Future+Callable+ConcurrentHashMap）
2016-04-06
    1、netty4使用例子
2016-06-02
    1、Annotation+Spring AOP Aspect实现缓存命中和未命中
2016-08-24
    1、JSR303通用参数校验（ValidatorUtil）
    2、通过自定义注解ObjectCheck支持嵌套对象的校验