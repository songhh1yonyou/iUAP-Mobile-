>来自：用友技术学院

>作者：SH

>链接：http://udn.yyuap.com/doc/train/iUAP-Mobile-/iuap-mobile平台介绍.html

>编辑：肖婷

#iuap Mobile平台介绍

##平台理念
iuap Mobile平台发展至今，本着定位于企业移动全生命周期的移动综合能力平台，形成独有的核心设计理念，主要体现在：
	快速开发、模型驱动 
	跨平台实现：一次开发，多个实现 
	基于模式开发：上百种应用、页面模板、组合控件、ICON
	多入口应用支撑：Web App、微信应用、Hybrid、Native-Hybrid、Native
	体验优先：既拥有Native的用户体验、又保留Web的开发效率 
	可视化设计、组件化组装 
	开放、融合开源 
	一体化移动解决方案：开放、管理、安全、整合… 

##平台产品祖成
基于平台定位以及iuap Mobile核心设计理念，形成目前mobile 5大产品。
![](/assets/100.png)

##产品定位
每个产品定位企业移动化不同阶段，解决用户痛点问题。企业可根据自身移动化阶段，选择不同产品。5大产品定位如下：
	开发平台：
目标：简化移动应用的开发复杂度，实现跨平台、可视化快速开发。
	移动中间件：
目标：为移动应用提供运行支持，集成多种异构后台系统，实现与后台各类业务系统的有效集成，降低开发和实施成本
	移动管理EMM：
目标：简化企业IT管理，提供用户、移动设备、移动应用等全面的监控和管理服务，提供全面的移动管控
	EMM移动工作台
目标：集成、保护数据安全，为移动业务数据提供安全保障
	应用商店
目标：快速下发应用到客户

##产品功能概况
5大产品功能概览如下：
![](/assets/101.png)

1)	开发平台
开发平台支持 HTML5、混合式和原生应用开发，由mobile studio和构造服务器Build Server组成。移动应用的设计、开发、模拟调试等工作在 mobile studio上完成。构建服务器 Build Server用于构造移动应用、管理模板等工作，完成移动应用的打包和发布。
![](/assets/102.png)

开发平台提供的功能主要包括：
•集成开发环境：提供向导、设计器、模拟器、模板等，帮助开发者快速上手，提高开发效率
•设备服务：将电话、通讯录、设备机型信息等设备服务封装，供开发者直接调用
•工具服务：将消息推送、地图、二维码、文件传输等服务封装，供开发者直接调用
•UI控件：UI设计器提供常用控件，如文本类、输入类、图片类、时间日期类等，开发者可使用设计器以拖拉拽的形式，设计应用UI界面
![](/assets/103.png)

•BuilderServer：移动应用构建服务器，负责移动应用的构建工作，提供：构建证书管理、构建模板管理、设备类型管理、移动OS类型管理、用户管理功能。
•扩展功能：基于平台标准，可以自定义UI控件扩展、服务器扩展。
2)	移动中间件MA Server
MA Server为移动应用提供运行支持，集成多种异构后台系统。
![](/assets/104.png)

提供以下功能：
•应用控制器：同时管理多个应用的多个版本
•服务网关：集成多种异构后台系统，实现与后台各类业务系统的有效集成
•管理工具：MA Server自带管理系统，提供应用部署工具、日志管理等功能。
•公共服务：提供登陆、身份认证、文件服务、持久化等服务。
3)	移动管理
提供全面的移动管控，简化企业IT管理，提供用户、移动设备、移动应用等全面的监控和管理服务。
![](/assets/105.png)

•移动设管理：监控设备运行、设备锁定/解锁、数据擦除、设备定位等
•移动应用管理：应用分发、升级、授权、信息管理等
•移动内容管理：内容信息库管理、内容授权
•用户自助管理：通过为用户提供基本的设备管理权来减轻IT部门的工作负担 
•移动策略管理：针对密码、功能、应用黑白名单、应用版本控制等，自定义相关策略
•仪表板、日志、统计分析等
4)	EMM移动工作台
集成、保护数据安全，为移动业务数据提供安全保障。
![](/assets/106.png)

•安全认证中心：支持点到登陆、身份验证功能
•应用中心：内置APP商店，可实现应用分发、应用集成，并采用沙箱隔离，保证数据安全。
•自定义设计：可根据公司需要，利用summer开发工具对移动工作台实现个性化设计。
5)	应用商店
快速下发应用到客户，实现应用分发、用户管理功能。

##技术架构图
了解完iuap Mobile平台的功能，从平台技术架构角度，更能对平台有深入的了解。

![](/assets/107.png)

①	开发工具：使用开发工具提供的各种设计器、设置工具、实时预览、调试工具、日志工具等功能，快速开发，生成Android、iOS工程
②	Build Server：将使用开发工具开发的工程打包成APP
③	使用mobile平台开发的APP，运行态是运行在iuapMobile APP Framework，包括原生UI加载、原生浏览器、私有浏览器、UI组件、原生框架、设备服务调用、JS引擎等，保证APP的正常运行。
④	MA Server：为平台开发的移动应用提供运行支持， 提供APP服务、过滤器filter、安全、消息推送push、提供者provide、数据源data source、协议转换的通用适配器Protocol Adapter 、Base Dao数据持久化，配置、日志等
⑤	EMM：提供用户MUM、移动设备MDM、移动应用MAM、内容MCM等全面的监控和管理服务，另外有统计分析，提供全面的移动管控
⑥	Mobile Portal：内置APP商店，实现应用集成；以sso实现单点登录，具有沙箱隔离，保护数据安全，为移动业务数据提供安全保障

对iuap Mobile 更多了解，请参考移动官网(http://mobile.yyuap.com/)

