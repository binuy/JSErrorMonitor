# JSErrorMonitor
页面javascript错误监控系统
## 安装
1. 通过`npm install`安装所有依赖 
2. 项目本地开发调试依赖于`webpack`和`yeoman`所以需要先全局安装二者
3. 项目是基于`generator-react-webpack`生成的，更多用法请参考[generator-react-webpack](https://github.com/newtriks/generator-react-webpack)
## 命令
**本地开发调试需要后台API支持，请安装并启动[JSErrorMonitor-server]()或者自己实现，API代理转发配置在[cfg/base.js](https://github.com/icefox0801/JSErrorMonitor/blob/master/cfg/base.js)中**
+ `npm start`：在本地[http://localhost:8000/webpack-dev-server/](http://localhost:8000/webpack-dev-server/)启动项目
## 开发
+ 项目底层是基于[react](https://facebook.github.io/react/)、[redux](https://github.com/reactjs/redux)和[react-redux](https://github.com/reactjs/react-redux)搭建
  + react-redux：通过`connect`和`<Provider>`将`react`和`redux`两者进行集成 
  + react的文档：[中文](http://reactjs.cn/react/docs/getting-started.html)、[English](http://reactjs.cn/react/docs/getting-started.html)
  + flux应用架构：[中文](https://facebook.github.io/flux/docs/overview.html)、[English](http://reactjs.cn/react/docs/flux-overview.html)
  + redux的文档：[中文](http://cn.redux.js.org/)、[English](http://redux.js.org/)
  + redux的教程：[redux核心概念](http://www.jianshu.com/p/3334467e4b32)、[React+Redux系列教程](https://github.com/lewis617/react-redux-tutorial)、[深入理解React、Redux](http://www.jianshu.com/p/0e42799be566)
+ 项目UI应用了[react-boostrap](https://github.com/react-bootstrap/react-bootstrap)
  + react-bootstrap文档：[English](http://react-bootstrap.github.io/)
+ 路由应用了[react-router](https://github.com/reactjs/react-router)、[react-router-redux](https://github.com/reactjs/react-router-redux)和[react-router-bootstrap](https://github.com/react-bootstrap/react-router-bootstrap)
  + react-router-bootstrap：通过`<LinkContainer>`将`react-router`与`react-bootstrap`两者进行集成
  + react-router-redux：通过`routeReducer`和`routeMiddleWare`将`react-router`与`react-redux`两者进行集成
  + react-router文档：[中文](http://react-guide.github.io/react-router-cn/)、[English](https://github.com/reactjs/react-router/tree/master/docs)
+ 图表应用了[Highcharts](http://www.highcharts.com/)
  + Highcharts文档：[中文](http://www.hcharts.cn/api/index.php)、[English](http://api.highcharts.com/highcharts)
+ 数组、对象操作应用了[lodash](https://github.com/lodash/lodash)
  + lodash的文档：[中文(**比较旧，不推荐**)](http://lodashjs.com/docs/)、[English](https://lodash.com/docs)
+ 日期对象操作应用了[momentjs](https://github.com/moment/moment)
  + momentjs的文档：[中文](http://momentjs.cn/docs/)、[English](http://momentjs.com/docs/)
+ 其他库：
  + [nprogress](https://github.com/rstacruz/nprogress)：页面顶部加载进度条
  + [react-highcharts](https://github.com/kirjs/react-highcharts)：将`react`和`Highcharts`两者进行集成
  
## src目录结构
src
├── actions：redux的actions目录
├── components：react的组件目录
├── config：开发配置目录
├── constants：常量目录
├── favicon.ico
├── images：图片目录
├── index.html：页面
├── index.js：页面的入口js
├── reducers：redux的reducers目录
├── stores：redux的store目录
├── styles：redux的样式目录
└── utils：js工具方法目录
## ES6与JSX harmony语法
项目默认开启ES6与JSX harmony语法支持
+ ES6教程：[深入浅出ES6](http://www.infoq.com/cn/minibooks/ES6-in-Depth?utm_campaign=rightbar_v2&utm_source=infoq&utm_medium=minibooks_link&utm_content=link_text)
+ 模块化：支持import语法，项目的`node_modules`目录会作为模块根目录

## 系统示例：
+ 首页：

+ 列表页：
+ 详情页：
+ 图表页：
