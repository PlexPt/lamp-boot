# 《灯灯》中后台快速开发平台

[![AUR](https://img.shields.io/badge/license-Apache%20License%202.0-blue.svg)](https://github.com/zuihou/lamp-cloud/blob/master/LICENSE)
[![](https://img.shields.io/badge/作者-zuihou-orange.svg)](https://github.com/zuihou)
[![](https://img.shields.io/badge/版本-3.1.2-brightgreen.svg)](https://github.com/zuihou/lamp-cloud)
[![GitHub stars](https://img.shields.io/github/stars/zuihou/lamp-cloud.svg?style=social&label=Stars)](https://github.com/zuihou/lamp-cloud/stargazers)
[![star](https://gitee.com/zuihou111/lamp-cloud/badge/star.svg?theme=white)](https://gitee.com/zuihou111/lamp-cloud/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/zuihou/lamp-cloud.svg?style=social&label=Fork)](https://github.com/zuihou/lamp-cloud/network/members)
[![fork](https://gitee.com/zuihou111/lamp-cloud/badge/fork.svg?theme=white)](https://gitee.com/zuihou111/lamp-cloud/members)

# lamp 项目名字由来
## 叙事版：

在一个夜黑风高的晚上，小孩吵着要出去玩，于是和`程序员老婆`一起带小孩出去放风，路上顺便讨论起项目要换个什么名字，在各自想出的名字都被对方一一否决后，大家陷入了沉思。 走着走着，在一盏路灯下，孩砸盯着路灯打破宁静，喊出：灯灯～
我和媳妇愣了一下，然后对视着一起说：哈哈，这个名字好～

## 解释版：

`灯灯`： 是我小孩学说话时会说的第一个词，也是我在想了很多项目名后，小孩一语点破的一个名字，`lamp`象征着光明，给困境的我们带来希望，给加班夜归的程序员们指引前方～

`灯灯`(简称灯， 英文名：lamp)，他是一个项目的统称，包含以下几个子项目

## lamp 项目组成
注意： 请先下载lamp-util 代码并编译（mvn install） 到本地仓库，然后在编译（mvn install）lamp-cloud或lamp-boot项目， 最后编译（mvn install）lamp-job项目！！！

### 工具集 （lamp-util 项目必备，其他2个可选）

| 项目 | gitee | github | 备注 | 
| --- | --- | --- | --- |
| 工具集 | [lamp-util](https://gitee.com/zuihou111/lamp-util) | [lamp-util](https://github.com/zuihou/lamp-util) | 业务无关的工具集，cloud 和 boot 项目都依赖它 |
| 代码生成器 | [lamp-generator](https://gitee.com/zuihou111/lamp-generator) | [lamp-generator](https://github.com/zuihou/lamp-generator) | 给开发人员使用 |
| 定时调度器 | [lamp-job](https://gitee.com/zuihou111/lamp-job) | [lamp-job](https://github.com/zuihou/lamp-job) | 尚未开发 |

### 后端 （下面2个项目功能一致，任选其一即可）

| 项目 | gitee | github | 备注 |
| --- | --- | --- | --- |
| 微服务版(后端) | [lamp-cloud](https://gitee.com/zuihou111/lamp-cloud) | [lamp-cloud](https://github.com/zuihou/lamp-cloud) | SpringCloud 版 |
| 单体版(后端) | [lamp-boot](https://gitee.com/zuihou111/lamp-boot) | [lamp-boot](https://github.com/zuihou/lamp-boot) | SpringBoot 版(和 lamp-cloud 功能基本一致) |

### 前端 （下面3个项目功能一致，任选其一即可）

| 项目 | gitee | github | 备注 | 演示地址 |
| --- | --- | --- | --- | --- |
| 中后台管理系统 | [lamp-web](https://gitee.com/zuihou111/lamp-web) | [lamp-web](https://github.com/zuihou/lamp-web) | （全部功能已完成）基于 vue-admin-element | http://tangyh.top:10000 |
| 中后台管理系统 | [lamp-web-beautiful](https://gitee.com/zuihou111/lamp-web-beautiful) | [lamp-web-beautiful](https://github.com/zuihou/lamp-web-beautiful) | （正在开发...）基于 vue-admin-beautiful | http://tangyh.top:180 |
| 中后台管理系统 (强烈推荐！👏👏👏) | [lamp-web-beautiful](https://gitee.com/zuihou111/lamp-web-plus) | [lamp-web-beautiful](https://github.com/zuihou/lamp-web-plus) | （正在开发...）基于 vue-vben-admin （vue 3 + vite 2） | http://tangyh.top:3100 |

# lamp-boot 简介

`lamp-boot`的前身是`zuihou-admin-boot`，从3.0.0版本开始，改名为lamp-boot，它是`lamp`项目的其中一员。

`lamp-boot` 基于`SpringBoot(2.3.9.RELEASE)` 的前后分离的快速开发平台，其中的可配置的SaaS功能尤其闪耀，
具备RBAC功能、网关统一鉴权、Xss防跨站攻击、自动代码生成、多种存储系统、分布式事务、分布式定时任务等多个模块，支持多业务系统并行开发，
支持多服务并行开发，可以作为后端服务的开发脚手架。代码简洁，注释齐全，架构清晰，非常适合学习和企业作为基础框架使用。

核心技术采用SpringBoot、Mybatis、Redis、RabbitMQ、FastDFS/MinIO、SkyWalking等主要框架和中间件。 希望能努力打造一套从 `JavaWeb基础框架` - `单体架构` - `持续集成`
- `系统监测` 的解决方案。`本项目旨在实现基础能力，不涉及具体业务。`

**切记:使用本项目之前，先下载并编译 [lamp-util](https://github.com/zuihou/lamp-util)**

**切记:使用本项目之前，先下载并编译 [lamp-util](https://github.com/zuihou/lamp-util)**

**切记:使用本项目之前，先下载并编译 [lamp-util](https://github.com/zuihou/lamp-util)**

## 分支介绍
1. master 分支为最新的稳定版本，每次提交都会升级一个版本号
2. dev 分支为作者的开发分支，作者开发的最新功能会实时提交上来，喜欢尝鲜的可以切换为dev。 但可能有报错、漏提等，对项目不是很熟的朋友千万别尝试。
3. tag 每个固定的版本都会打一个tag方便后续切换任意版本。

## lamp 租户模式介绍
本项目可以通过配置，轻松切换项目的 **租户模式**。

| 租户模式 | 描述 | 优点 | 缺点  | 
|---|---|---|---|
| NONE(非租户模式) | 没有租户 | 简单、适合独立系统 | 缺少租户系统的优点 | 
| COLUMN(字段模式) | 租户共用一个数据库，在业务表中增加字段来区分 | 简单、不复杂、开发无感知 | 数据隔离性差、安全性差、数据备份和恢复困难、 | 
| SCHEMA(独立schema) | 每个租户独立一个 数据库(schema)，执行sql时，动态在表名前增加schema | 简单、开发无感知、数据隔离性好 | 配置文件中必须配置数据库的root账号、不支持复杂sql和 sql嵌套自定义函数 | 
| DATASOURCE(独立数据源) | 每个租户独立一个 数据库(数据源)，执行代码时，动态切换数据源 | 可独立部署数据库，数据隔离性好、扩展性高、故障影响小 | 相对复杂、开发需要注意切换数据源时的事务问题、需要较多的数据库 |

## lamp 会员版项目演示地址

- (已完成) 基于 [FEBS-Cloud-Web](https://gitee.com/mrbirdd/FEBS-Cloud-Web) 改造的前端项目演示地址： http://tangyh.top:10000/lamp-web/
- (正在开发中...)基于 [vue-admin-beautiful](https://github.com/chuzhixin/vue-admin-beautiful)
  改造的前端项目 演示地址： http://tangyh.top:180
- (正在开发中...)基于 ant-design [vue-vben-admin](https://github.com/anncwb/vue-vben-admin) 开发的前端项目 演示地址：http://tangyh.top:3100
- 以下内置账号仅限于内置的0000租户
- 平台管理员： lamp_pt/lamp (内置给公司内部运营人员使用)
- 超级管理员： lamp/lamp
- 普通管理员： general/lamp
- 普通账号： normal/lamp

> ps: 演示环境中内置租户没有写入权限，若要在演示环境测试增删改，请使用lamp_pt账号查询租户管理员账号后,登录新租户测试

## lamp-cloud/lamp-boot + lamp-web 功能介绍：
1. 租户管理：运营人员管理所有的租户创建
2. 工作台：普通用户常用功能
3. 组织管理：组织、岗位、用户数据维护、重置用户密码等
4. 资源中心：消息、短信、附件管理
5. 流程管理：流程部署、模型管理、流程示例
6. 系统设置：菜单、资源配置、角色管理、给角色绑定用户、给角色授权菜单和资源、字典、地区、系统参数、操作日志、登录日志、应用管理等
7. 网关设置：限流和阻止访问
8. 开发者管理：定时任务、接口文档、注册&配置中心、服务监控、数据库监控、zipkin监控、SkyWalking监控

## lamp-boot 项目亮点功能介绍:
1. **服务鉴权:**

    通过JWT的方式来加强服务之间调度的权限验证，保证内部服务的安全性。

2. **数据权限**

    利用基于Mybatis的DataScopeInnerInterceptor拦截器实现了数据权限功能

3. **SaaS(多租户)的无感解决方案**

    本项目支持3种常见的租户解决方案和无租户方案，同一套代码，修改一个配置即可实现租户模式只有切换。

4. **缓存抽象**

    采用CacheOps操作缓存，内置2种实现：Caffeine、 Redis，可以让项目应急时在无Redis环境正常运行

5. **优雅的Bean转换**

    采用Dozer、BeanUtil等组件来对 DTO、DO、PO等对象的优化转换

6. **前后端统一表单验证**

    严谨的表单验证通常需要 前端+后端同时验证， 但传统的项目，均只能前后端各做一次检验， 后期规则变更，又得前后端同时修改。
    故在`hibernate-validator`的基础上封装了`lamp-validator-starter`起步依赖，提供一个通用接口，可以获取需要校验表单的规则，然后前端使用后端返回的规则，
    以后若规则改变，只需要后端修改即可。

7. **防跨站脚本攻击(XSS)**
    
    - 通过过滤器对所有请求中的 表单参数 进行过滤
    - 通过Json反序列化器实现对所有 application/json 类型的参数 进行过滤
    
8. **当前登录用户信息注入器**
    
    - 通过注解实现用户身份注入
    
9. **在线API**

    由于原生swagger-ui某些功能支持不够友好，故采用了国内开源的`knife4j`，并制作了stater，方便springboot用户使用。

10. **代码生成器**

    基于Mybatis-plus-generator自定义了一套代码生成器， 通过配置数据库字段的注释，自动生成枚举类、数据字典注解、SaveDTO、UpdateDTO、表单验证规则注解、Swagger注解等。

11. **定时任务调度器**：

    基于xxl-jobs进行了功能增强。(如：指定时间发送任务、执行器和调度器合并项目、多数据源)

12. **大文件/断点/分片续传**

    前端采用webupload.js、后端采用NIO实现了大文件断点分片续传，启动Eureka、Zuul、File服务后，直接打开docs/chunkUploadDemo/demo.html即可进行测试。
    经测试，本地限制堆栈最大内存128M启动File服务,5分钟内能成功上传4.6G+的大文件，正式服耗时则会受到用户带宽和服务器带宽的影响，时间比较长。

13. **分布式事务**

    集成了阿里的分布式事务中间件：seata，以 **高效** 并且对业务 **0侵入** 的方式，解决 微服务 场景下面临的分布式事务问题。

14. **跨表、跨库、跨服务的关联数据自动注入器**

    用于解决跨表、跨库、跨服务分页数据的属性或单个对象的属性 回显关联数据之痛, 支持对静态数据属性(数据字典)、动态主键数据进行自动注入。

15. **灰度发布**
    
    为了解决频繁的服务更新上线，版本回退，快速迭代，公司内部协同开发，本项目采用修改ribbon的负载均衡策略来实现来灰度发布。
     
## lamp-boot 技术栈/版本介绍：
- 所涉及的相关的技术有：
    - JSON序列化:Jackson
    - 消息队列：RabbitMQ
    - 缓存：Redis
    - 数据库： MySQL 5.7.9 或者 MySQL 8.0.19
    - 定时器：采用xxl-jobs项目进行二次改造
    - 前端：vue + element-ui
    - 持久层框架： Mybatis-plus
    - 代码生成器：基于Mybatis-plus-generator自定义 
    - API网关：Gateway/zuul
    - 项目构建：Maven 
    - 监控： spring-boot-admin  
    - 文件服务器：FastDFS 5.0.5/阿里云OSS/本地存储/MinIO
    - Nginx
- 部署方面：
    - 服务器：CentOS
    - Jenkins
    - Docker  
    - Kubernetes 

# 项目截图：

| 预览 | 预览 |
|---|---|
| ![预览.png](01-docs/image/架构图/lamp-cloud架构图.png) | ![预览.png](01-docs/image/业务/swagger.png) |
| ![预览.png](01-docs/image/业务/nacos.jpg) | ![预览.png](01-docs/image/业务/工作流.png) |
| ![预览.png](01-docs/image/业务/项目预览1.png) | ![预览.png](01-docs/image/业务/项目预览2.png) |
| ![预览.png](01-docs/image/监控/sba1.png) | ![预览.png](01-docs/image/监控/sba2.png) |
| ![预览.png](01-docs/image/监控/zipkin1_2_19_2.png) | ![预览.png](01-docs/image/监控/zipkin3_2_19_2.png) |
| ![预览.png](01-docs/image/监控/sw拓扑图.png) | ![预览.png](01-docs/image/监控/sw追踪列表.png)  |
| ![预览.png](01-docs/image/1000star.png) | ![预览.png](01-docs/image/软著V2.5.0.jpg) |


# 交流群，加群前请先给项目点个 "Star"，谢谢！😘

- 63202894(主群 满员请加群2)
- 1011148503(群2)    

# 如果觉得本项目对您有任何一点帮助，请点右上角 "Star" 支持一下， 并向您的基友、同事们宣传一下吧，谢谢！

# [点我查看详细文档](https://www.kancloud.cn/zuihou/zuihou-admin-cloud)
    ps: gitee捐献 或者 二维码打赏(本页最下方)： 45元及以上 并 备注邮箱，可得开发文档一份(支持后续更新) 
        打赏或者捐献后直接加群：1039545140 并备注打赏时填写的邮箱，可以持续的获取最新的文档。 

# 遇到问题请先查看历史issue，未找到解决方案，在提交issue(问题描述详细一些，报错截图大一些，复现步骤全一些)
    https://github.com/zuihou/lamp-cloud/issues    

# 会员版
本项目分为开源版和会员版，github和gitee上能搜索到的为开源版本，遵循Apache协议。 会员版源码在私有gitlab托管，购买后开通账号。

会员版和开源版区别请看：[会员版](会员版.md)

# 项目不错，支持一下吧
![扫码支持.png](01-docs/image/捐赠.png)

# 感谢 JetBrains 提供的免费开源 License：
[![JetBrains](01-docs/image/jetbrains.png)](https://www.jetbrains.com/?from=lamp-cloud)
    
# 友情链接 & 特别鸣谢
* 微服务快速开发平台：[https://github.com/zuihou/lamp-cloud](https://github.com/zuihou/lamp-cloud)
* 单体快速开发平台：[https://github.com/zuihou/lamp-boot](https://github.com/zuihou/lamp-boot)
* MyBatis-Plus：[https://mybatis.plus/](https://mybatis.plus/)
* knife4j：[http://doc.xiaominfo.com/](http://doc.xiaominfo.com/)
* hutool：[https://hutool.cn/](https://hutool.cn/)
* xxl-job：[http://www.xuxueli.com/xxl-job/](http://www.xuxueli.com/xxl-job/)
* kkfileview：[https://kkfileview.keking.cn](https://kkfileview.keking.cn)
* vue-vben-admin(vue3.x + vite2.x)： [https://github.com/anncwb/vue-vben-admin](https://github.com/anncwb/vue-vben-admin)
  lamp-web-plus 基于本项目改造
* FEBS Cloud Web： [https://gitee.com/mrbirdd/FEBS-Cloud-Web](https://gitee.com/mrbirdd/FEBS-Cloud-Web)
  lamp-web 基于本项目改造， 感谢 [wuyouzhuguli](https://github.com/wuyouzhuguli)
* Cloud-Platform： [https://gitee.com/geek_qi/cloud-platform](https://gitee.com/geek_qi/cloud-platform)
  作者学习时接触到的第一个微服务项目
* [vue-admin-beautiful](https://github.com/chuzhixin/vue-admin-beautiful)
  lamp-web-beautiful 基于本项目改造
