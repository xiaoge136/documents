# 跑通互动直播
互动直播示例代码提供普通的单主播直播已经PK直播和连麦直播

## 前提条件
在开始运行示例项目之前，请确保您已完成以下操作：  
联系云信商务获取开通以下权限，并联系技术支持配置产品服务和功能
* 在云信控制台创建应用，并获取对应的 AppKey。[云信控制平台](../../云信控制平台/应用创建和服务开通.md)
* 为此应用开通以下相关服务与抄送：
* 产品服务：  
音视频通话 2.0、IM 专业版、聊天室、透传协议
* 产品功能：   
音视频通话 2.0 的抄送功能。

* 如需使用美颜功能请联系相芯获取美颜证书 [相芯](https://www.faceunity.com/)

## 开发环境 
在开始运行示例项目之前，请确保开发环境满足以下要求：
* Android SDK API 等级 19 或以上。
* Android Studio 4.0 或以上版本。  
  如果低于此版本，需要调整 `build.gradle` 和 `gradle\wrapper\gradle-wrapper.properties` 中匹配的版本。
* Android 系统 4.3 或以上版本的移动设备。

## 示例项目结构
|  目录   | 说明  |
|  ----  | ----  |
| app  | 应用主入口包含外部页面框架。 |
| biz-user | 用户相关实现 |
| lib-user  | 用户lib |
| lib-modularity  | app模块化 |
| lib-basic  | 基础lib |
| lib-beauty-faceunity  | 美颜lib，基于相芯 |
| lib-network-kt | kotlin 使用的网络库 |
| biz-live | 直播业务实现，主要是UI方面 |
| lib-live-room-service | 直播房间服务 |
| lib-live-pk-service | Pk相关功能服务 |

## 运行示例源码
1. GitHub下载源代码 [源码](https://github.com/netease-kit/OnlinePK/tree/dev_2.0.0/OnlinePK-Android)
2. 导入Android Studio
3. 找到 `config/test.properties` 文件替换自己的 appkey   
    *  `test.properties` 是debug包的配置环境，`online.properties` 是 release 包的配置环境   
    *  此处的appkey请联系技术支持获取配置互动直播服务器使用权限
4. 如果需要使用美颜功能请使用自己的相芯证书替换 `lib-beauty-faceunity/src/main/java/com/beautyFaceunity/authpack.java` 证书文件
5. 运行在自己的Android设备上
