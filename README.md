# examSystem

> 一款开源的在线考试系统

## 技术栈

Vue + Vuex + element-ui + webpack + nodejs + koa2 + mongodb

## 目录结构

- build - webpack配置文件

  - build.js - 执行webpack编译任务
  - check-versions.js
  - utils.js
  - vue-loader.conf.js - vue配置
  - webpack.base.conf.js - webpack基本通用配置
  - webpack.dev.conf.js - webpack开发环境配置
  - webpack.prod.conf.js - webpack生产环境配置

- config - 项目参数配置文件

- logs - 日志打印文件

- node_modules - 项目依赖模块

- public - 静态文件入口

- src - 代码模块

  - admin - 后台管理源码

    - src - 代码区域
      - assets - 资源加载
        - font - 字体
        - img - 图片
        - styles - 样式表
        - icon - 图标
      - components - 组件
      - filters - 过滤器
      - router - 路由
      - store - vuex状态管理
      - utils - 请求封装
      - views - 页面模块
      - app.vue - app组件
      - main.js - 入口js
    - index.html - webpack模板文件

  - client - 客户端源码

    同admin

  - server - 服务端源码

    - controller - 接口方法
      - admin - 后台管理接口
      - client - web端接口
    - middkeware - 中间件
      - auth - 权限
      - func - 方法
      - log - 日志
      - rule - 规则
      - send - 发送
      - index.js
    - models - 数据库model
    - router - 路由
    - app.js - 入口
    - config.js - 配置文件
    - index.js - babel编译
    - mongodb.js - MongoDB配置文件

- static - 静态资源文件

- test - 测试文件

- .babelrc - babel编译

- .eslintrc.js - eslint配置文件

- .postcssrc.js - CSS后处理器配置

- package.json - 包管理文件

## 开发依赖

- vue/vue-router/vuex - Vue全家桶
- axios - 一个现在主流并且很好用的请求库 支持Promise
- qs - 用于解决axios POST请求参数的问题
- element-ui - 饿了么出品的vue2.0 pc UI框架
- babel-polyfill - 用于实现浏览器不支持原生功能的代码
- highlight.js / marked- 两者搭配实现Markdown的常用语法
- js-md5 - 用于登陆时加密
- nprogress - 顶部加载条
- less
- less-loader
- koa

chromedriver被墙

```bash
npm install chromedriver --chromedriver_cdnurl=http://cdn.npm.taobao.org/dist/chromedriver
```

