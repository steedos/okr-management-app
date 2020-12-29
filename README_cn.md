
<p align="center">
  <a href="https://www.steedos.com/cn">
    <img alt="华炎OKR管理系统" src="https://steedos.github.io/assets/logo.png" width="120" />
  </a>
</p>
<h1 align="center">
  华炎OKR管理系统
</h1>

<p align="center">
<a href="https://github.com/steedos/okr-management-app/blob/master/README.md">English</a>
<a href="https://github.com/steedos/okr-management-app/issues/"> · 报告错误</a>
<a href="https://github.com/steedos/okr-management-app/discussions"> · 讨论</a>
</p>

<p align="center" style="border-top: solid 1px #cccccc">
  帮助您管理组织范围内的目标(Objectives)与关键成果(Key Results)，实时跟踪、自动汇总、全面统计。系统使用华炎魔方平台可视化配置实现，基于元数据驱动，可以快速自定义。
</p>

<h3 align="center">
 🤖 🎨 🚀
</h3>

# OKR管理系统

OKR（Objectives and Key Results）即目标与关键成果法，聚焦于企业战略落地，通过目标分解、成果量化、跟踪复盘来推动资源整合、团队协同、目标达成。从Intel、Google、Facebook到百度、华为、字节跳动，OKR这套管理工具/方法正被越来越多的卓越企业应用、推崇。

华炎OKR管理系统，融合了OKR的理论和实践，着力于明确企业与团队的“目标”，将目标分解为可衡量的“关键成果”，通过有效行动推动进展，适时汇报进展，系统自动累计绩效数据，优化实施策略。

## ✨系统功能

- **目标(Objectives)**：可以在系统中管理组织、团队与个人目标。公开透明的信息，促使组织与个人目标一致，共同实现战略目标与长远价值。

![目标](https://steedos.github.io/assets/github/okr_management_app/cn/objective.png)

- **关键成果(Key Results)**：聚焦重点项，将目标分解为可量化考核的关键成果，设定目标值及权重，并分配给责任人落实。

- **进度跟踪**：责任人按要求定期汇报关键成果的最新进展，系统自动计算成果的完成度。数据公平透明，激励员工更好地学习和成长。

![关键成果](https://steedos.github.io/assets/github/okr_management_app/cn/keyresults.png)

- **绩效评估**：自动汇总目标的实时完成度百分比、信心指数，由此可以及时发现问题，提出优化措施，推动目标达成。

## 🚀功能开发

华炎OKR管理系统基于华炎魔方开发，采用业界领先的零代码/低代码开发方式，代码量减少90%，开发效率提升十倍。这么一来，原先只能提出需求的业务人员，也可以在需求开发的过程中，通过配置的方式来实现业务需求。

下面是几个简单的例子。

- 公式

例如，在本系统中，当增加1条进度跟踪记录时，试图用最新值、起始值、目标值结合对应关键成果的目标类型（增加/减少）来自动求得。通过华炎魔方来开发，就可以用公式引擎来快速实现。

![公式](https://steedos.github.io/assets/github/okr_management_app/cn/formula.png)

这样的公式配置，对于业务人员来说也不是很困难。通过查看华炎魔方的说明文档，其难度应与EXCEL的函数配置大体相当。

- 累计汇总

例如，基于公式，系统已经可以自动计算出目标下的每个关键成果的最新完成度百分比，以及加权后的完成度（贡献），将这些完成度（贡献）累加就是该目标的最新完成度的数值。这个字段，就可以采用“累计汇总”的字段类型。

![累计汇总](https://steedos.github.io/assets/github/okr_management_app/cn/cumulative.png)

这么配置后，系统会自动累计完成度（贡献）到目标的完成度上。如果采用传统的开发方式，这个需求可能需要由开发人员（程序员）编写触发器来实现；而在华炎魔方的开发环境下，熟悉一点的业务人员自己就可以在页面上配出这个字段、实现这样的业务逻辑。

- 工作流规则

例如，当输入1条最新的跟踪记录时，需要实时更新进度跟踪记录（本条记录对应的父对象记录）的最新跟踪日期、最新值、完成度、信心指数、完成度（贡献）。这一需求，通过华炎魔方的工作流规则即可快速实现。

![工作流规则](https://steedos.github.io/assets/github/okr_management_app/cn/flowrule.png)

上例中，还增加了规则条件，如果输入的不是最新数据，则系统不会自动运行工作流规则。

## 关于华炎魔方

华炎魔方是一套可视化建模、描述式编程的开发工具。设计目标是降低应用构建门槛，让每个人都能参与开发。系统内置了数据建模以及一系列自动化工具，包括验证规则、公式计算、工作流规则、自动化操作、批准过程、报表引擎等等。

- [华炎魔方概述](https://www-steedos-com.oss-accelerate.aliyuncs.com/videos/steedos/steedos-open-source.mp4)
- [华炎魔方文档](https://www.steedos.com/help/)

## 依赖包

- [MongoDB](https://www.mongodb.com/try/download/) version >= 3.4. MongoDB is a general purpose, document-based, distributed database built for modern application developers and for the cloud era.
- [Node.js](https://nodejs.org/en/download/) version >= 10.15.1 or above (which can be checked by running `node -v`). You can use [nvm](https://github.com/nvm-sh/nvm) for managing multiple Node versions on a single machine installed
- [Yarn](https://yarnpkg.com/en/) version >= 1.5 (which can be checked by running `yarn version`). Yarn is a performant package manager for JavaScript and replaces the `npm` client. It is not strictly necessary but highly encouraged.


## 项目目录

```sh
okr-management-app
├── steedos-app/main/default
│   ├── applications
│   │   └── okr.app.yml
│   └── objects
│       └── okr
│           ├── buttons
│           │   └── print.button.yml
│           │   └── print.button.js
│           ├── fields
│           │   └── name.field.yml
│           │   └── description.field.yml
│           │   └── isDone.field.yml
│           │   └── status__c.field
│           │   └── ...
│           ├── listviews
│           │   └── all.listview.yml
│           │   └── recent.listview.yml
│           │   └── my.listview.yml
│           ├── permissions
│           │   └── user.permission.yml
│           │   └── admin.permission.yml
│           │   └── okr.permission.yml
│           └── okr.object.yml
│           └──...
├── .env
├── .gitignore
├── package.json
├── README.md
├── server.js
├── steedos-config.yml
└── yarn.lock
```

## 项目运行

项目源码依赖 nodejs 环境，使用 mongodb 数据库，需先部署相应的运行环境。

1、 启动数据库

2、安装依赖软件包

```
yarn
```

3、运行项目

```
yarn start
```

4、使用浏览器访问 http://127.0.0.1:5000/

第一次使用时，数据库为空，需注册一个账户，并选择创建一个企业。

## 保持联系

如果您有任何疑问或想与其他华炎魔方用户交谈，请[点击进入讨论](https://github.com/steedos/steedos-platform/discussions)或扫码添加以下联系方式与我们联系！
##### 开发人员微信群
![开发者微信交流群](https://steedos.github.io/assets/github/project_management_app/cn/QR_wechat_developers.jpg)

##### 商务咨询
![商务咨询](https://steedos.github.io/assets/github/project_management_app/cn/business_consulting.jpg)

##### 微信公众号
![微信公众号](https://www.steedos.com/assets/github/platform/cn/public_number.jpg)
