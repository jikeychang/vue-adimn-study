> [金鑫的NPM包](https://www.npmjs.com/package/easy-create)
> [项目的备注地址](https://github.com/jikeyChang/vue-adimn-study/blob/master/build/webpack.base.conf.js)
## Webpack
webpack是一个打包工具

loader 和 plugin

https://github.com/niceMatthew/easy-create/blob/master/package.json


下载包的时候   
npm i vue -S/--save  这个命令就是下载包到dependencies里面文件夹下
npm i css-loader -D 这个命令到devDependencies


npm run <命令> 读取 package.json文件夹下scirpts命令,只是个快捷方式


webpack-dev-server --inline --progress --config build/webpack.dev.conf.js

用webpack-dev-server起一个本地服务，配置地址是--config build/webpack.dev.conf.js

webpack.config.js

跨域： 浏览器的在一下情况下有安全策略的限制： 在不同协议（http,https）, 不同端口号（80），不同域名

如何解决跨域问题？
配置 cors属性，制定域名，*
使用jsonp:  https://www.cnblogs.com/soyxiaobi/p/9616011.html
jsonp的原理： 内部实现就是script的src去请求资源不会收到跨域策略限制，使用这一点就在请求接口中和后端约定一个callback函数
window.postMessage

loader 和 plugin 的区别

loader是讲特定模块转化成js能识别的模块，用于模块化转化
plugin更高级一点，做最后的处理，包括压缩，删除