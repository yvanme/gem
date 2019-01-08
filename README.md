# GemFrame
**架构简介**

- GemFrame基于SpringCloud、SpringBoot、MyBatis及周边的生态技术开发。是一款稳定，高效的企业级微服务架构，更是致力面向中小型企业提供的一套全面微服务架构的解决方案。并且其具有代码规范，学习成本极低，开箱即用等特点，方便开发者快速上手。官方网址： http://www.gemframe.cn

- 服务治理监控：Gem架构封装了SpringCloud提供的负载，降级，监控和统一配置等服务，可实现对应用、服务、链路、性能、响应率、成功率、可用率等基础监控与预警，并且集成了一些优秀的开源监控组件，对系统进行多维度监控，为企业系统保驾护航，让监控都变得如此简单。

- 基础能力建设：精细化权限管理，安全身份认证，即时通讯，文件服务，消息队列，工作流等。官方提供完善的API文档、部署文档、架构介绍文档以及视频教程帮助您快速学习入门，快速上手使用。

- GemFrame是为企业提供微服务基础架构最全面的解决方案，也是您学习Java微服务平台的最佳学习案例。

**软件需求**

- JDK1.8
- MySQL5.5+
- Maven3.0+


**技术选型**

前端
- Vue2.x
- Layui 单页版
- Bootstrap v3.3.6
- jQuery v2.1.4
- bootstrap-table v1.9.0
- layer v2.1
- zTree core v3.5.28
- WebUploader 0.1.5

后端
- SpringCloud Edgware.SR4
- SpringBoot 1.5.3.RELEASE
- MyBatis-Plus 2.0.8
- MyBatis 3.4.4
- Spring 4.3.8.RELEASE
- ActiveMQ 5.15.8.RELEASE
- Kafka 2.1.0
- Redis 3.3.1
- Kaptcha 2.3.2
- FastFs 1.2.31
- Shiro 1.4.0
- Druid 1.1
- SLF4J Log4j

**本地部署**

- 通过git下载源码
- 创建数据库gem_admin，数据库编码为UTF-8
- 运行gem-utlis-jpa即可生成数据库表结构
- 执行db/gem.sql文件，初始化表数据
- 修改application.properties文件，更新MySQL账号和密码
- 在gemframe目录下，执行mvn clean install

- Eclipse、IDEA运行gem-item-xxx中的XxxServerApplication.java，则可启动项目相关业务服务
- WebStrom运行gem-admin-layui前端代码运行start下的index.html
- gem-admin访问路径：http://localhost:8080/gem-admin/index.html
- 账号密码：admin/123456
- swagger文档路径：http://localhost:8080/xxx服务名/swagger/index.html

**内置功能**

- 资源管理：系统中的菜单，按钮，列表字段，查询条件等元素统称为资源。

- 角色管理：角色进行精细化资源授权，实现菜单，按钮，列表以及数据控制。

- 账户管理：登录系统的帐号称作“账户”，账户可以选择一个或多个角色。

- 人员管理：公司人员，通常指使用账户登录系统的人，人员可以与账户绑定。

- 部门管理：部门也可以称为“组织”，是将人员进行组织划分的模块。

- 字典管理：系统字典管理，常量管理。

- 日志管理：系统业务操作日志，API调用日志，用户登录日志等。

- 监控管理：系统链路监控，服务TPS，QPS监控，SQL监控等。

- 代码生成：使用GemFrame的专属代码生成器，减少80%重复工作量。