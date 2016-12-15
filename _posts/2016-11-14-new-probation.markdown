---
layout: post
title: "New Probation"
type: SHADOW
uri: 2016/11/14/new-probation.html
members: [金晶, 孙菁, 周奕星]
image: [12_23_Interview __.png,12_23_New Hire Landing Page.png,12_23_View New Hire.png]
description: 公司正在使用的Probation系统（TA Probation)主要用于新员工试用期期间的管理和考核，涉及Interview ++, probation,orientation等一系列的管理活动。
---
<h2>作品描述：</h2>

***Idea来源***
公司正在使用的Probation系统（TA Probation) 主要用于新员工试用期期间的管理和考核，涉及Interview ++, probation, orientation等一系列的管理活动。但是现有的TA Probation系统存在稳定性和可扩展性严重不足的问题，导致很多新需求无法满足。从而诞生了New Probation项目。

***项目意义***
这个项目具有重要的意义，此项目的第一阶段的目标是取代现有TA Probation，解决稳定性和扩展性的问题。未来我们期望将这个New Probation系统从新员工管理扩张到全公司员工的考核上，覆盖从新员工到转正之后的全生命周期的考核和培养。 它将会成为公司人员考核的一项重要工具。

***技术栈选型和架构设计***
New Probation系统采用了前后端分离的设计思想。这样便于团队协作和提高前端响应速度。
后端架构 - 采用Nginx + Rails API + Mysql数据库来提供API支持， 全部采用docker容器部署，便于迁移。
前端架构 - React + Redux 前端也部署在docker容器中

使用Go CD作为CI工具，实现了全自动部署，代码托管在Gitlab里
项目选用Rails API可以提高后端API开发效率并利用rails框架自身安全机制保证后端API的安全性
Docker容器的采用方便项目日后平滑迁移和简化了项目部署

***技术***
前后端分离
前端采用react渲染页面，轻量级动态刷新局部组件
使用redux进行数据流程的管理
代码运行在docker环境中，便于快速部署

***项目协作***
黑工项目，历来存在协作困难，难以坚持，效率低等问题。New Probation通过以下创新性方式进行协作：
项目人员采用常驻人员 + Beach人员的组合方式：常驻人员主要处理难度大的任务，beach人员处理相对简单的任务。
由于beach人员的流动性，为了充分利用beach资源，我们通过集中knowledge transfer的方式保证beach人员一天之内就可以快速接入项目; 通过拆分独立性的故事卡保证beach人员即使只能待一周，也能够有所产出并且不影响其他人进度。

***需求管理***
区别于传统黑工项目缺乏对需求的挖掘和管理，New Probation项目有以下特点：
通过正规Inception，识别真正需求，去除了老TA probation无用的功能
识别MVP，保证团队持续工作在高优先级的任务上

***设计***
在用户界面和交互上进行了全新改版：New Probation虽然是内部项目，但依然按照对外的billable项目标准来做，通过专业UX的帮助，制定了用户界面和交互的规范，以求带给用户更好的体验。

[作品主页][MainPage]

[MainPage]: http://10.202.5.15/
