title: 什么是 egg
---

**egg 为企业级框架和应用而生**，我们希望通过 egg 能孕育更多上层框架帮助开发团队和开发人员。

## 设计原则

egg 是社区少见的一种框架，它并没有集成社区常见的一些功能（诸如数据库、模板引擎、前端框架等），只是提供了 web 开发的核心功能和一套插件机制。为了团队能够基于 egg 扩展自己的框架，我们不会做出技术选型，因为固定的技术选型会让框架过于片面，无法满足的定制需求，egg 可以帮助架构师基于技术选型搭建框架。

egg 的插件机制有很高的定制化，插件只做一件事，比如 nunjucks 模板封装成了 [egg-view-nunjucks](https://github.com/eggjs/egg-view-nunjucks)，MySQL 数据库封装成了 [egg-mysql](https://github.com/eggjs/egg-mysql)。egg 通过框架聚合这些插件，并根据自己的业务场景定制配置，这样应用的开发成本就变得很低。

egg 奉行『约定优于配置』，按照[一定的约定](https://github.com/eggjs/egg/blob/master/docs/source/zh-cn/advanced/loader.md)进行应用开发，团队内部采用这种方式可以减少开发人员的学习成本，开发人员不再是『钉子』，可以云动起来。没有约定的团队，沟通成本是非常高的，比如有人会按目录分栈而其他人按目录分功能，开发者认知不一致很容易犯错。但约定不等于扩展性差，相反 egg 有很高的扩展性，可以按照团队的约定定制框架。

## 与社区框架的差异

[expressjs] 是 node 社区广泛使用的框架，简单且扩展性强，非常适合做个人项目。但框架本身缺少约定，标准的 MVC 模型会有各种千奇百怪的写法。egg 按照约定进行开发，奉行『约定优于配置』，团队协作成本低。

[sailsjs] 是和 egg 一样奉行『约定优于配置』的框架，扩展性也非常好。但是相比 egg，[sailsjs] 

## 特性

- 深度[框架定制](../advanced/framework.md)
- 高度扩展的[插件机制](../advanced/plugin.md)
- 内置[多进程管理](../advanced/cluster.md)
- 基于 [koa] 开发，性能优异
- 框架稳定，测试覆盖率高

[sails]: http://sailsjs.com
[express]: http://expressjs.com
[koa]: http://koajs.com
