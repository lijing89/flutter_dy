# 斗鱼APP

Flutter 1.12.13+hotfix9

原项目地址：https://github.com/yukilzw/dy_flutter


flutter重构的斗鱼直播APP<br/>
首页、娱乐为Material组件开发；直播间、鱼吧为纯自定义编写。<br/>
另外整合各类优质的第三方开源库，打造出原生APP丝滑的用户体验<br/>
尽可能接入更多功能，方法附带注释，帮助你在使用flutter进行开发新的应用提供实用的借鉴案例<br/>

#### 包含功能：

- 启动页广告位
- 开播列表上拉加载、下拉刷新、返回顶部
- 列表图片缓存加载优化
- 渐进式头部动画
- 底部导航切换保存页面状态
- HTTP缓存、IO缓存
- 直播间webSocket消息弹幕、礼物
- 页面路由传值
- RxDart全局消息通信封装
- Bloc流式状态管理(启动页预加载首页数据)
- 礼物横幅动画队列
- 礼物全屏svga特效
- 弹幕消息滚动
- 静态视频流
- 九宫格抽奖游戏
- 照片选择器
- 全屏、半屏webView
- 鱼吧头部手势动画
- 仿微信朋友圈图片控件
- 登录注册弹窗
- 国家区号列表(仿微信通讯录滑动首字母定位)
- 二维码扫码
- 本地通知推送
- ...
- 持续增加中

#### 调试：
服务端接口没有上云，如需本地启动该项目调试，可修改`lib/base.dart`中`DYBase.baseHost`为内网本机IP，并确保手机与电脑在同一局域网且能访问内网1236端口<br/>
然后clone[服务端仓库](https://github.com/yukilzw/factory)，本地启动服务器<br/>
Mock服务为python tornado，两种简单启动方式可选(1.安装py3.6与pip依赖，2.使用Docker镜像)，具体参考其README

PS：**因第三方插件版本兼容性不可控，请严格按照`pubspec.lock`的版本安装依赖启动**

#### 建议：
使用Material自带的widget进行搭配使用，已经能满足绝大部分场景的开发需求<br/>
但是在企业级APP高度UI交互定制化的场景下，仍需要根据业务场景重新实现诸如AppBar、TabView等widget，并编写手势交互<br/>

#### 入门推荐：
[Dart语法](https://www.dartcn.com/guides/get-started) - 语法中文教程<br/>
[Dart SDK（英）](https://api.dartlang.org/stable/2.4.0/index.html)<br/> - flutter只集成了部分SDK<br/>
[Flutter中文网](https://flutterchina.club/get-started/install/) - 简单易懂的入门教程<br/>
[Flutter实战](https://book.flutterchina.club/) - 较为全面的进阶教程<br/>
[Flutter官网（英）](https://flutter.dev/docs) - 可查阅全部的API与SDK相关<br/>
[Bloc（英）](https://felangel.github.io/bloc/#/gettingstarted) - 全局状态管理(除此之外也可选用`redux`或原生`InheritedWidget`)


#### dy_flutter为个人项目，仅用作学习交流
