koa文件夹路由加载

## Installation

```sh
$ npm install koa-directory-router
```

## Use with koa

```js
var app = require('koa')();
var directoryRouter = require('koa-directory-router');
var admin = directoryRouter({
    root: path.resolve(__dirname, path.normalize('./../app/controller/admin')),
    suffix: '.js',
    prefix: '/v1'
});
app.use(admin.routes());

提示：文件夹名可定义为router中可变参数
```
作者官网:
http://www.wemallshop.com