# autoftp
ftp、sftp自动上传模块
###xm-autoftp v0.0.5
实现本地自动监听文件变动上传指定服务端路径
```js
//需要在package.json scripts 添加 "autoftp": "autoftp"
npm run autoftp    //默认sftp
npm run autoftp ftp //ftp
```
./cfg/autoftpconfig.js
```js
//autoftp模块config
module.exports = {
    "host": "118.190.74.124",
    "user": "xmiles",
    "password": "mJH8ZVV1uaf13uOR",
    "filePath": "./pages",//本地路径
    "target": '/data2/webserver/campaign_service_apache-tomcat-7.0.64_152/webapps/campaign_service/pages',//服务器路径
    "time": 10//连接超时时间10min，不要设置太长时间
};
```
