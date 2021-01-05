
<p align="center">
  <a href="https://www.steedos.org">
    <img alt="Steedos OKR Management System
" src="https://steedos.github.io/assets/logo.png" width="120" />
  </a>
</p>
<h1 align="center">
  Steedos OKR Management System
</h1>

<p align="center">
<a href="https://github.com/steedos/okr-management-app/blob/master/README_cn.md">中文</a>
<a href="https://github.com/steedos/okr-management-app/issues/"> · Report a bug</a>
<a href="https://github.com/steedos/okr-management-app/discussions"> · Discussions</a>
</p>

<p align="center" style="border-top: solid 1px #cccccc">
Goal Setting and Employee Performance Management. Openly share your business strategy and main company goals with the rest of your organization and encourage the alignment and focus of everyone in your company behind a common objective.
</p>

<h3 align="center">
 🤖 🎨 🚀
</h3>

With Steedos OKR, each department, team, and individual aligns their own Objectives and Key Results toward your company goals, focusing on what really matters. Steedos OKR automatically records your OKRs, keeping track of their progress in a transparent way to ensure collaboration and commitment.

Follow a process of planning and alignment by creating periods for each quarter. Track and push best practices to ensure that each individual has the right OKRs. Complete wrap-up phases to perform self-assessments, score objectives, and receive manager feedback, and to determine how to improve for the next cycle. Steedos OKR supports both TOP-DOWN and BOTTOM-UP OKRs.

Steedos OKR is developed entirely within Steedos, allowing you to track your OKRs automatically and in real time by binding any Steedos report to the key result you need to measure.

Features: 

- OKR Alignment 
- Automatic and Continuous Tracking 
- OKR Achievement Forecast 
- Dashboards and Reporting 
- One on Ones Module 
- My Focus

## About  Steedos Platform

Steedos Platform is a visual modeling and descriptive programming development tool. The design goal is to lower the threshold of application construction so that everyone can participate in the development. The system has built-in data modeling and a series of automatic tools, including validation rules, public computing, workflow rules, automatic operation, approval process, report engine and so on.

- [Steedos Platform](https://www.steedos.org/)

## Requirements

- [MongoDB](https://www.mongodb.com/try/download/) version >= 3.4. MongoDB is a general purpose, document-based, distributed database built for modern application developers and for the cloud era.
- [Node.js](https://nodejs.org/en/download/) version >= 10.15.1 or above (which can be checked by running `node -v`). You can use [nvm](https://github.com/nvm-sh/nvm) for managing multiple Node versions on a single machine installed.
- [Yarn](https://yarnpkg.com/en/) version >= 1.5 (which can be checked by running `yarn version`). Yarn is a performant package manager for JavaScript and replaces the `npm` client. It is not strictly necessary but highly encouraged.


## okr Structure

```sh
okr-management-app
├── steedos-app/main/default
│   ├── applications
│   │   └── okr.app.yml
│   └── objects
│       └──okr__c
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
│           │   └── okr_manager.permission.yml
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

##  Quick Start

The source code of the project depends on nodejs environment. To use mongodb database, the corresponding running environment should be deployed first.

  1. Start the database  
  2. Install dependent packages
  3. Running project
  4. Using browser access `http://127.0.0.1:5000/`    For the first time, the database is empty. You need to register an account and choose to create an enterprise.

## Keep in Contact

If you have any questions or want to talk to other users of Steedos Platform , please jump to GitHub for discussion [Click to Discuss](https://github.com/steedos/steedos-platform/discussions) or [Join me on Slack-it's a faster,simpler way to work](https://join.slack.com/t/steedos/shared_invite/zt-jq7eupr9-cgKrUOyWb1zymniRzhH4jg).
