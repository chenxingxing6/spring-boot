## Spring Boot

Spring Boot使创建具有Spring动力的生产级应用程序和服务变得非常容易，而引起的麻烦却很小。 它从Spring平台的角度出发，以便新老用户都能快速找到所需的信息。
您可以使用Spring Boot创建独立的Java应用程序，可以使用java -jar或更传统的WAR部署来启动它。 我们还提供了运行Spring脚本的命令行工具。

我们的主要目标是：
> 为所有Spring开发提供根本上更快且可广泛访问的入门经验  
> 开箱即用，但随着需求开始偏离默认值而迅速摆脱困境  
> 提供一系列大型项目通用的非功能性功能（例如，嵌入式服务器，安全性，指标，运行状况检查，外部化配置）  
> 完全没有代码生成，也不需要XML配置  

---
## Modules
There are a number of modules in Spring Boot, here is a quick overview:

#### spring-boot-autoconfigure
Spring Boot can configure large parts of common applications based on the content of their classpath. A single @EnableAutoConfiguration annotation triggers auto-configuration of the Spring context.

Auto-configuration attempts to deduce which beans a user might need. For example, if HSQLDB is on the classpath, and the user has not configured any database connections, then they probably want an in-memory database to be defined. Auto-configuration will always back away as the user starts to define their own beans.

#### spring-boot-starters
Starters are a set of convenient dependency descriptors that you can include in your application. You get a one-stop-shop for all the Spring and related technology that you need without having to hunt through sample code and copy paste loads of dependency descriptors. For example, if you want to get started using Spring and JPA for database access just include the spring-boot-starter-data-jpa dependency in your project, and you are good to go.

#### spring-boot-cli
The Spring command line application compiles and runs Groovy source, making it super easy to write the absolute minimum of code to get an application running. Spring CLI can also watch files, automatically recompiling and restarting when they change.

#### spring-boot-actuator
Actuator endpoints let you monitor and interact with your application. Spring Boot Actuator provides the infrastructure required for actuator endpoints. It contains annotation support for actuator endpoints. Out of the box, this module provides a number of endpoints including the HealthEndpoint, EnvironmentEndpoint, BeansEndpoint and many more.

#### spring-boot-actuator-autoconfigure
This provides auto-configuration for actuator endpoints based on the content of the classpath and a set of properties. For instance, if Micrometer is on the classpath, it will auto-configure the MetricsEndpoint. It contains configuration to expose endpoints over HTTP or JMX. Just like Spring Boot AutoConfigure, this will back away as the user starts to define their own beans.

#### spring-boot-test
This module contains core items and annotations that can be helpful when testing your application.

#### spring-boot-test-autoconfigure
Like other Spring Boot auto-configuration modules, spring-boot-test-autoconfigure, provides auto-configuration for tests based on the classpath. It includes a number of annotations that can be used to automatically configure a slice of your application that needs to be tested.

#### spring-boot-loader
Spring Boot Loader provides the secret sauce that allows you to build a single jar file that can be launched using java -jar. Generally you will not need to use spring-boot-loader directly, but instead work with the Gradle or Maven plugin.

#### spring-boot-devtools
The spring-boot-devtools module provides additional development-time features such as automatic restarts, for a smoother application development experience. Developer tools are automatically disabled when running a fully packaged application.
