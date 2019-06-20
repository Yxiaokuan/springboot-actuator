# springboot-actuator
springboot:2.1.6 整合actuator
详解：

    GET	/conditions	提供了一份自动配置报告，记录哪些自动配置条件通过了，哪些没通过
    GET	/configprops	描述配置属性(包含默认值)如何注入Bean
    GET	/beans	描述应用程序上下文里全部的Bean，以及它们的关系
    GET	/dump	获取线程活动的快照
    GET	/env	获取全部环境属性
    GET	/env/{name}	根据名称获取特定的环境属性值
    GET	/health	报告应用程序的健康指标，这些值由HealthIndicator的实现类提供
    GET	/info	获取应用程序的定制信息，这些信息由info打头的属性提供
    GET	/mappings	描述全部的URI路径，以及它们和控制器(包含Actuator端点)的映射关系
    GET	/metrics	报告各种应用程序度量信息，比如内存用量和HTTP请求计数
    GET	/metrics/{name}	报告指定名称的应用程序度量值
    POST	/shutdown	关闭应用程序，要求设置management.endpoint.shutdown.enabled=true
    GET	/httptrace	提供基本的HTTP请求跟踪信息(时间戳、HTTP头等)
  
```
  #默认端点 前面多了一个根路径 /actuator
  访问：http://localhost:8181/actuator/health
```
基本配置请看 [application.yaml](./src/main/resources/application.yaml)