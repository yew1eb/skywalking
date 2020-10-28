# 跑起来一个Demo


<https://skyapm.github.io/document-cn-translation-of-skywalking/zh/8.0.0/guides/How-to-build.html>


打包出一个完全的包放在dist/ 目录下面。

cd dist
tar -xvf apache-skywalking-apm-bin.tar.gz
cd apache-skywalking-apm-bin

工作目录： /Users/yew1eb/workspaces/skywalking/dist/apache-skywalking-apm-bin

## 0.快速入门 
https://skyapm.github.io/document-cn-translation-of-skywalking/zh/8.0.0/setup/backend/backend-ui-setup.html

## 1.启动前端UI 
https://skyapm.github.io/document-cn-translation-of-skywalking/zh/8.0.0/setup/backend/ui-setup.html

## 2.启动后端
https://skyapm.github.io/document-cn-translation-of-skywalking/zh/8.0.0/setup/backend/backend-ui-setup.html

## 默认快速DEMO启动
你可以通过bin/startup.sh(或cmd) 在默认设置下启动Backend和UI,，同时希望你能了解：

默认使用H2存储，这样就不需要部署别的了。
Backend的gRPC相关的API可访问0.0.0.0/11800，rest相关的API可访问0.0.0.0/12800

UI 监听8080 端口,同时请求127.0.0.1/12800来做GraphQL查询。

