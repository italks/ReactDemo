# ReactDemo
##测试react框架
1、Hello-world

##测试React Native
1、[AwesomeProject](https://github.com/italks/ReactDemo/tree/master/AwesomeProject)

##常见问题
1：创建新项目，react-native init AwesomeProject命令长时间无响应，或报错shasum check failed

A：由于众所周知的网络原因，react-native命令行从npm官方源拖代码时会遇上麻烦。请将npm仓库源替换为国内镜像：

npm config set registry https://registry.npm.taobao.org --global
npm config set disturl https://npm.taobao.org/dist --global
另，执行init时切记不要在前面加上sudo（否则新项目的目录所有者会变为root而不是当前用户，导致一系列权限问题，请使用chown修复）。

2：运行react-native run-android时报错，报错信息中含有Unable to upload some APKs!字样

A：参照下图降级gradle版本

[降级gradle版本](5.png)

[常见问题解决方法](http://bbs.reactnative.cn/topic/130/%E6%96%B0%E6%89%8B%E6%8F%90%E9%97%AE%E5%89%8D%E5%85%88%E6%9D%A5%E8%BF%99%E9%87%8C%E7%9C%8B%E7%9C%8B-react-native%E7%9A%84%E5%B8%B8%E8%A7%81%E9%97%AE%E9%A2%98)
