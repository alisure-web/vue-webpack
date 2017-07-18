多页脚手架


For detailed explanation on how things work, checkout the [guide](http://vuejs-templates.github.io/webpack/)
 and [docs for vue-loader](http://vuejs.github.io/vue-loader).


0.脚手架说明：
    1.安装webpack：
        npm install -g webpack
    2.安装vue-cli:
        npm install -g vue-cli
    3.安装vuejs-templates(https://github.com/vuejs-templates):
        (从这里克隆，不需要本步骤，若从新开始，则需要)
        vue init webpack vue-webpack
        cd vue-webpack
    4.安装依赖：
        npm install
    5.启动项目（开发）：
        npm run dev
    6.构建项目（生产）：
        # build for production with minification
        npm run build
        # build for production and view the bundle analyzer report
        npm run build --report


1.修改为多页脚手架
    总共修改了6处，代码中有说明（alisure add x）：
    build/utils.js 添加两处
    build/webpack.base.conf.js 修改一处
    build/webpack.dev.conf.js (注释一处)添加一处
    build/webpack.prod.conf.js (注释一处)添加一处
    config/index.js 注释一处


2.运行
    1）启动项目（开发）：
        npm run dev
    2）构建项目（生产）：
        # build for production with minification
        npm run build
        # build for production and view the bundle analyzer report
        npm run build --report

3.示例
    等有时间了再写个复杂一点的。


