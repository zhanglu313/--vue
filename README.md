# elements

> elements app

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```
##vue项目环境搭建

```bash
# 安装node环境
node官网下载安装，node -v 检测安装版本 npm -v 检测安装版本

# 脚手架创建项目
全局安装脚手架：npm i vue-cli -g

# webpack初始化项目
vue init webpack 项目名称

# 切换目录 
cd 目录

#运行项目
npm run dev

#打包项目
npm run  build
```
##目录结构分析

```bash 
#package
依赖包存放区域

#package.json
package的锁文件，帮助我们去确定安装的第三方包的版本信息，保持团队编程的统一

# index.html
项目默认的首页模板文件

#.postcssrc.js
是对postcss配置项

#.gitignore
对git提交时候，把特殊的文件放进去，在进行git提交的时候，不会提交到上面

#.eslintr.js
配置了一些代码规范，对代码规范的要求,做出错误提示

#.eslintignore
在根目录下的build，config，dist，*.js 文件夹，是不会受eslint检测工具检测，这些文件写的不标准，不会进行语法上的提示

#.editorconfig
配置了编辑器里面的语法

#.babelrc
我们的项目写的代码是vue单文件组件的写法，所以需要通过babelrc语法解析器做语法转换，最终转换成浏览器能够编译执行的代码，所以我们需要引入babelrc的内容，当我们需要做额外配置的时候，都需要放在babelrc文件下

# static文件
放静态资源，如图片，模拟json数据

#node-modules
依赖的包

#src文件下的main.js
是整个项目的入口文件

#src文件下的App.vue
是项目最原始的根组件

#src文件下的router文件
项目中所有的路由

#src文件下的components
项目里面用的组件

#src文件下的assets
项目中用到的图片资源

#config文件
放的是项目配置的文件，基础的配置信息放在index.js中，开发中的配置信息放在dev.env.js中，线上的配置文件放在prod.env.js中

#build
放的是webpack打包的一些配置
```

## 第三方插件的安装

```bash
#
```
##项目初始化

```bash
#引入公共样式
在static文件夹加入reset.css,然后在main.js里面引入reset.css   import './assets/style/reset.css'

#解决移动端边框一像素的问题
引入border.css文件,放在style文件夹下面，然后在main.js里面引入border.css   import './assets/style/border.css'

#解决移动端点击300毫秒延迟问题
引入fastclick库，打开终端，安装第三方模块 npm i fastclick -save ,在main.js中引入，import fastClick from 'fastclick',fastClick.attach(document.body)

#n
```


For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).
