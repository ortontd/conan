## 柯南流量回放平台
<p align="left">
    <a href="https://github.com/1042970366/">
        <img src="https://img.shields.io/badge/license-MIT-green" alt="MIT License" />
    </a>
    <a href="https://java.org/">
        <img src="https://img.shields.io/badge/java-1.8.1-green" alt="Vue2.0">
    </a>
    <a href="https://vuejs.org/">
        <img src="https://img.shields.io/badge/vue.js-2.0-green" alt="Vue2.0">
    </a>
    <a href="https://github.com/1042970366/">
        <img src="https://img.shields.io/badge/author-TALconan-blueviolet" alt="Author">
    </a>
    <a href="https://github.com/1042970366/">
        <img src="https://img.shields.io/badge/🚀-open--in--browser-blueviolet" alt="Live Demo">
    </a>
</p>

经过在线教育业务中的持续打磨与迭代，柯南平台终于开源，旨在为行业内更多的的质效保障团队提供更专业更稳定的质效保障方案。随着业务与技术架构的不断变化，服务端的质量保障工作变得越来越复杂。近几年流量回放的方案在行业内落地生根，但大部分以工具为主并且使用成本与二次开发生成本较高，柯南平台应运而生。



## 目标
基于线上真实用户流量的录制回放能力与结果校验能力，为冒烟测试，集成回归测试，线上验证与线上巡检提供解决方案。


## 核心功能
**流量采集**

基于ES日志源的流量录制采集，平台化配置接入，降低使用成本，并且提供详细的流量采集数据。


**流量回放**

分布式的后端架构，为流量回放提升执行效率，支持服务鉴权配置，基于http协议的回放符合真实业务场景。

**结果校验**

流量回放的常规校验方式基本上是以流量结果的DIFF为主，但大量的流量噪声（时间戳，自增数据...）一直影响结果的准确性，柯南平台在回放中基于配置的jsonSchema做第一层校验，再结合自研的降噪比对服务进行流量DIFF的第二层校验，从而保障了结果校验的准确性，大大提升了流量回放结果的可信度。


## 平台优势与应用场景
**优势**   
  - 解决传统自动化覆盖率低，维护成本高的问题
  - 多规则的流量结果断言校验
  - 多规则的流量结果比对支持
  - 流量数据可用于自动化测试与性能测试
  - 交互简单，配置化接入
  - 开源共建，持续优化

**应用场景**   
  - 提测质量卡点
  - CI/CD流水线质量卡点
  - 服务线上监控巡检


**平台业务架构**    
![后端业务架构.png](http://ttc-tal.oss-cn-beijing.aliyuncs.com/1605259627/%E5%90%8E%E7%AB%AF%E4%B8%9A%E5%8A%A1%E6%9E%B6%E6%9E%84.png)
<center>
业务架构
</center>

**平台技术架构**  
![后端技术架构.png](http://ttc-tal.oss-cn-beijing.aliyuncs.com/1605255935/%E5%90%8E%E7%AB%AF%E6%8A%80%E6%9C%AF%E6%9E%B6%E6%9E%84.png)
<center>
服务端架构
</center>

<br>

**平台能力及功能** 
![柯南能力图.png](http://ttc-tal.oss-cn-beijing.aliyuncs.com/1605261800/%E6%9F%AF%E5%8D%97%E8%83%BD%E5%8A%9B%E5%9B%BE.png)

**使用须知**
- 流量采集: ES日志；
- 回放协议: http协议；
- 具体环境可参考开源详细技术文档

## 写在最后
质效的提升也许不能单单通过一个平台，技术与人的结合才能带来更大的突破。善于利用技术创新才能从容的面对越来越频繁的需求，越来越复杂的业务，柯南平台的技术方案产出于学而思网校的大班业务并且逐步通用化，平台现已开源，希望更多优秀的人或团队参与进来，为质效保障工作提供更多的解决方案。

**详细使用文档**
https://dengkunnanmayun.gitee.io/conan-docs/#/use/README

**更多介绍**
https://mp.weixin.qq.com/s/1Cvi5kkqfF9y1rBi97qLwg

</br>
</br>
柯南 - 流量回放平台
基于SpringBoot、Spring Security、Jwt、RuoYi、Vue的前后端分离的流量回放平台管理系统
介绍
业务的线上质量与研发全流程的效率一直是工程师们关注的重点，近几年CI/CD的成熟度更是衡量研发团队效能体系的重要指标，质量与效率的博弈不断考验每一位工程师， 通过学而思网校质量团队基于线上真实流量，来赋能于网校业务的质效保障工作，通过网校实践总结的经验，本着技术开放，赋能更多人的愿望，在原有系统基础上改良后形成了现在的平台，并将其开源。

Conan 是一个 Java EE 企业级流量回放平台，基于经典技术组合（Spring Boot、Spring Security、MyBatis、Jwt、Vue），内置模块如：流量录制、流量回放、流量比对、ES数据源管理、接口管理、域名管理、菜单用户权限控制等。在线定时任务配置，支持定时线上轮询回放，任务Agent 机器水平扩展，高效流量回放，及回放结果检测方案。

在线体验

项目GitHub地址：https://github.com/tal-tech/conan (opens new window)

项目官网地址：https://tal-tech.github.io/conan (opens new window)


项目首页
账号密码：admin/admin123

系统需求

JDK >= 1.8 MySQL >= 5.7 Maven >= 3.0

联系我们

柯南技术交流群： 276567821（1群）




快速了解
主要特征
流量回放特有特征

支持流量多数据源录制
支持回放结果Schema校验
支持流量将智能化比对
支持动态ES数据源配置
灵活化任务管理，一次配置多次使用
系统代码特征

完全响应式布局（支持电脑、平板、手机等所有主流设备）
强大的一键生成功能（包括控制器、模型、视图、菜单等）
支持多数据源，简单配置即可实现切换。
支持按钮及数据权限，可自定义部门数据权限。
对常用js插件进行二次封装，使js代码变得简洁，更加易维护
完善的XSS防范及脚本过滤，彻底杜绝XSS攻击
Maven多项目依赖，模块及插件分项目，尽量松耦合，方便模块升级、增减模块。
国际化支持，服务端及客户端支持
完善的日志记录体系简单注解即可实现
支持服务监控，数据监控，缓存监控功能。
主要功能配置模块化，二次开发容易
技术选型
1、系统环境

Java EE 8
Servlet 3.0
Apache Maven 3
2、主框架

Spring Boot 2.3.x
Spring Framework 5.2.x
Spring Security 5.2.x
Shiro 1.7.0
RuoYi-vue 3.4.0
3、持久层

Apache MyBatis 3.5.x
Hibernate Validation 6.0.x
Alibaba Druid 1.2.x
Spring data jpa 2.2.6
4、视图层

Vue 2.6.x
Axios 0.21.0
Element 2.14.x
5、主要工具

json-schema-validato 2.2.12
hutool-all 5.3.10
json-compare-tool 1.1.x
内置功能
接口管理：该功能分主要完成需要录制/回放对接口提前配置。
域名管理：是流量所属的域名，该功能对域名数据源，域名权限校验配置。
测试用户：对回放需要替换对用户Cookie进行配置，为流量支持回放做准备。
任务管理：对需要回放接口进行管理，创建可重复使用对任务列表。
Schema：对接口response进行校验配置，灵活的对回放结果进行验证。
流量比对：对回放后对多个任务之间可以进行比对，得处比对结果。
用户管理：用户是系统操作者，该功能主要完成系统用户配置。
部门管理：配置系统组织机构（公司、部门、小组），树结构展现支持数据权限。
岗位管理：配置系统用户所属担任职务。
菜单管理：配置系统菜单，操作权限，按钮权限标识等。
角色管理：角色菜单权限分配、设置角色按机构进行数据范围权限划分。
字典管理：对系统中经常使用的一些较为固定的数据进行维护。
参数管理：对系统动态配置常用参数。
操作日志：系统正常操作日志记录和查询；系统异常信息日志记录和查询。
登录日志：系统登录日志记录查询包含登录异常。
在线用户：当前系统中活跃用户状态监控。
定时任务：在线（添加、修改、删除)任务调度包含执行结果日志。
代码生成：前后端代码的生成（java、html、xml、sql)支持CRUD下载 。
系统接口：根据业务代码自动生成相关的api接口文档。
服务监控：监视当前系统CPU、内存、磁盘、堆栈等相关信息。
缓存监控：对系统的缓存信息查询，命令统计等。
在线构建器：拖动表单元素生成相应的HTML代码。
连接池监视：监视当期系统数据库连接池状态，可进行分析SQL找出系统性能瓶颈。
环境部署
准备工作
JDK >= 1.8 (推荐1.8版本)
Mysql >= 5.7.0 (推荐5.7版本)
Maven >= 3.0
redis (推荐6.0以上版本)
Kafka 
必要配置
修改Mysql数据库连接，编辑admin和agent下resources目录下的application-local.yml

#数据库配置
spring:
resources:
  add-mappings: true
datasource:
  druid:
    # 主库数据源
    master:
      url: jdbc:mysql://127.0.0.1:8080/conan_test?useUnicode=true&characterEncoding=utf8&zeroDateTimeBehavior=convertToNull&useSSL=true&serverTimezone=GMT%2B8（数据库地址）
      username: conan（数据库名称）
      password: 'conan'（密码）
    # 从库数据源
    slave:
      # 从数据源开关/默认关闭
      enabled: false
      url:
      username:
      password:
    #JPA 连接的数据源
    url: jdbc:mysql://127.0.0.1:8080/conan_test?useUnicode=true&characterEncoding=UTF-8&autoReconnect=true&failOverReadOnly=false&serverTimezone=Asia/Shanghai
    password: La5Hha/wdY2u8iYSHN2JdPrUunJnu+bDoFr+fQhaNoyRXi6hxdAWJw7oatJn5LecK8N+Ls+mxLPbOwvtM8gD3Q==
    public-key: MFwwDQYJKoZIhvcNAQEBBQADSwAwSAJBAJgbbw4r01SO4o82/rXilIFLQGujU8xggtr+wTYgO2x0sdo1arGpQCXYsfQCXrGcvaIijUYmv+h/P9yoEvswciECAwEAAQ==
修改Redis数据库连接，编辑admin和agent下resources目录下的application-local.yml

 redis:
    # 地址
    host: 127.0.0.1
    # 端口，默认为6379
    port: 6379
    # 密码
    password: test@123
修改Kafka配置，编辑admin和agent下resources目录下的application.yml
kafka:
  bootstrap-servers: 10.90.72.126:9092
  consumer:
    group-id: conan-admin-local
修改服务器配置，编辑admin和agent下resources目录下的application.yml
server:
port: 8081 # 监听端口
运行系统
前往GitHub下载页面(https://github.xxx/xxx/Conan (opens new window))下载解压到工作目录

编译器后端运行
1、（1）导入到Eclipse，菜单 File -> Import，然后选择 Maven -> Existing Maven Projects，点击 Next> 按钮，选择工作目录，然后点击 Finish 按钮，即可成功导入。 （2）导入IntelliJ IDEA，菜单 File -> Open 打开文件目录。
Eclipse/IntelliJ IDEA会自动加载Maven依赖包，初次加载会比较慢（根据自身网络情况而定）
2、创建数据库Conan并导入数据脚本Conan_2021xxxx.sql，quartz.sql
3、 (1)ConanAdmin启动： 打开项目运行com.tal.wangxiao.conan.admin.AdminApplication.java，出现如下conan-admin服务启动图表示启动成功。
(2)ConanAgent启动： 打开项目运行com.tal.wangxiao.conan.admin.AgentApplication.java,出现如下conan-agent服务启动图表示启动成功


conan-admin服务启动

conan-agent服务启动

编译器前端运行
# 进入项目目录
cd conan-ui

# 安装依赖
npm install

# 强烈建议不要用直接使用 cnpm 安装，会有各种诡异的 bug，可以通过重新指定 registry 来解决 npm 安装速度慢的问题。
npm install --registry=https://registry.npm.taobao.org

# 本地开发 启动项目
npm run dev
打开浏览器，输入：(http://localhost:80 (opens new window)) 默认账户/密码 admin/admin123） 若能正确展示登录页面，并能成功登录，菜单及页面展示正常，则表明环境搭建成功

部署系统
提示：

因为本项目是前后端完全分离的，所以需要前后端都单独部署好，才能进行访问。后端需要部署redis、mysql、kafaka、服务conan-admin、conan-agent。

后端部署
1、在conan项目的bin目录下执行package.bat打包Web工程，生成war/jar包文件。 然后会在项目下生成target文件夹包含war或jar

2、可以通过编译器Intellij IDEA ->Maven ->Conan ->Install 如下图conan-打包


conan-打包

提示：

各个模块生成Jar在conan/../模块下target文件夹下。

部署工程文件 1、jar部署方式 使用命令行执行： java -jar conan-admin.jar >/dev/null 2>&1& 和 java -jar conan-agent.jar >/dev/null 2>&1& 或者执行脚本：conan/bin/run.bat 或单独执行脚本：conan/conanadmin/shell/run.bat 和 conan/conanagent/shell/run.bat

2、war部署方式 conan/pom.xml、conan/conan-admin/pom.xml、conan/conan-agent/pom.xml中的packaging修改为war，放入tomcat服务器webapps。


提示：

需要优先启动conanAdmin，conanAgent后启动，conanAgent可以修改端口部署多套，Agent会通过kafka主动向admin上报自己。 由于流量录制和回放可能流量较大时间较长，一台Agent可能无法支撑业务发展。所以agent支持水平扩展。admin在收到执行任务请求的时候会根据当前空闲的agent 去分配任务 。

前端部署
将开发完成的前端项目进行打包，注意修改配置文件服务器地址

# 打包正式环境
npm run build:prod

# 打包预发布环境
npm run build:stage
构建打包成功之后，会在根目录生成 dist 文件夹，里面就是构建打包好的文件，通常是 .js 、.css、index.html 等静态文件。

通常情况下 dist 文件夹的静态文件发布到你的 nginx 或者静态服务器即可，其中的 index.html 是后台服务的入口页面。


outputDir 提示：

如果需要自定义构建，比如指定 dist 目录等，则需要通过 config (opens new window)的 outputDir 进行配置。


publicPath 提示：

部署时改变页面js 和 css 静态引入路径 ,只需修改 vue.config.js 文件资源路径即可。

    publicPath: './' //请根据自己路径来配置更改
export default new Router({
  mode: 'hash', // hash模式
})
常见问题
如果使用Mac需要修改application.yml文件路径profile
如果使用Linux 提示表不存在，设置大小写敏感配置在/etc/my.cnf添加lower_case_table_names=1，重启MYSQL服务
如果提示当前权限不足，无法写入文件请检查application.yml中的profile路径或logback.xml中的log.path路径是否有可读可写操作权限
项目介绍
文件结构
后端结构
后端结构
com.tal.wangxiao.conan     
├── conan-ui              // 前端框架 [80]
├── coann-admin         // api业务管理服务 [8081]
├── coann-agent           // 数据任务执行服务（通常部署多个） [8082]
├── coann-common          // 通用模块
├── coann-utils          // conan工具集合
├── coann-config          // conan工具集合
│       └── coann-config-core                         // 配置核心模块
│       └── coann-config-datasource                   // 数据源
│       └── coann-config-redis                        // 缓存服务
│       └── coann-config-swagger                      // 系统接口
├── conan-system-fwk         // 二开ruoyi 的通用数据管理模块
│       └── conan-auth-demo                              // 演示
│       └── conan-sys-api                                 // ruoyi 通用api
│       └── conan-sys-auth                                 // 鉴权管理模块
│       └── conan-sys-common                                // 通用模块
│       └── conan-sys-framework                                // ruoyi框架核心业务
│       └── conan-sys-generator                                // 代码生成
│       └── conan-sys-quartz                               // 定时任务
│       └── conan-sys-system                                // 系统配置模块
├──pom.xml                // 公共依赖
前端结构
├── build                      // 构建相关  
├── bin                        // 执行脚本
├── public                     // 公共文件
│   ├── favicon.ico            // favicon图标
│   └── index.html             // html模板
│   └── robots.txt             // 反爬虫
├── src                        // 源代码
│   ├── api                    // 所有请求
│   ├── assets                 // 主题 字体等静态资源
│   ├── components             // 全局公用组件
│   ├── directive              // 全局指令
│   ├── layout                 // 布局
│   ├── router                 // 路由
│   ├── store                  // 全局 store管理
│   ├── utils                  // 全局公用方法
│   ├── views                  // view
│   ├── App.vue                // 入口页面
│   ├── main.js                // 入口 加载组件 初始化等
│   ├── permission.js          // 权限管理
│   └── settings.js            // 系统配置
├── .editorconfig              // 编码格式
├── .env.development           // 开发环境配置
├── .env.production            // 生产环境配置
├── .env.staging               // 测试环境配置
├── .eslintignore              // 忽略语法检查
├── .eslintrc.js               // eslint 配置项
├── .gitignore                 // git 忽略项
├── babel.config.js            // babel.config.js
├── package.json               // package.json
└── vue.config.js              // vue.config.js
