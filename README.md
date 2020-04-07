# klasa-member-gateway

[![Build Status](https://dev.azure.com/dirigeants/klasa/_apis/build/status/dirigeants.klasa-member-gateway?branchName=master)](https://dev.azure.com/dirigeants/klasa/_build/latest?definitionId=3&branchName=master)

Simple plugin to manage an efficient per-member settings gateway.

## Installation

```bash
# NPM
$ npm install --save dragondev/klasa-member-master-gateway/

# Yarn
$ yarn add https://github.com/dragondev/klasa-member-master-gateway.git
```

## Setup

```js
const { Client } = require('klasa');

Client.use(require('@klasa/member-gateway'));

// Modifying the Schema
Client.defaultMemberSchema
    .add('experience', 'integer', { default: 0 })
    .add('level', 'integer', { default: 0 });
```
