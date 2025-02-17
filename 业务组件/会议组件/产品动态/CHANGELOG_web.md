# 变更记录

|    日期    |  版本  | 变更内容                                                     |
| :--------: | :----: | :----------------------------------------------------------- |
| 2020-09-15 | 1.0.0  | 首次正式发布，支持基础会议功能                               |
| 2020-09-29 | 1.2.6  | 支持预约会议加入，修复已知bug                                |
| 2020-10-29 | 1.3.0  | 支持预约会议密码加入，修复已知bug                            |
| 2020-10-22 | 1.2.8  | 支持多端互踢，增加*NEMeetingInfo*字段                        |
| 2020-11-12 | 1.3.1  | 增加*shortId*字段  <br>  增加两种登陆方式 *loginWithNEMeeting* *loginWithSSOToken* <br> 增加初始化配置，兼容已有方案 |
| 2020-11-20 | 1.3.2  | 增加创会入会额外可选配置： *meetingIdDisplayOptions* 会议号展示逻辑 |
| 2020-11-27 | 1.3.3  | 补充关闭预约会议密码回调监听 <br> 补充创建会议提示已存在会议取消操作监听 <br> 加入会议增加预约会议密码参数*password* <br> 调整会议画廊模式展示策略 |
| 2020-12-21 | 1.5.0  | 补充自定义按钮配置                                           |
| 2021-01-15 | 1.5.2  | 增加音频流订阅方法 <br> *subscribeRemoteAudioStream*订阅用户音频流 <br> *subscribeAllRemoteAudioStreams*订阅所有用户音频流 <br> *subscribeRemoteAudioStreams*订阅用户音频流Bylist |
| 2021-02-05 | 1.6.0  | 修复部分已知bug                                              |
| 2021-03-17 | 1.7.0  | 增加会中改名入口 <br> 创建，加入会议增加 *noRename* 字段（是否使用会中改名）<br> 新增*defaultWindowMode*选项配置“会议视图模式”，支持普通和白板模式 |
| 2021-03-30 | 1.7.2  | 增加成员进出事件监听*peerJoin* *peerLeave* <br> 网络事件监听*networkQuality*<br> 国际化配置*setLocale* *useLocale* |
| 2021-04-29 | 1.8.1  | 共享时支持视频显示 <br> 增加额外会议信息 <br> 增加会议创建配置 |
| 2021-06-02 | 1.9.1  | 修复已知bug                                                  |
| 2021-07-08 | 1.10.0 | 增加创建会议额外配置*scene* <br> 增加创会入会时自定义*memberTag* <br> 增加日志方法*uploadLog* *downLog* |
| 2021-07-20 | 1.12.0 | 升级音视频SDK                                                |
| 2021-08-12 | 1.12.2 | 调整主讲人切换间隔 <br> 修复已知bug                          |
| 2021-09-09 | 2.0.4  | 订阅接口支持promise <br> 修复已知bug                         |

# CHANGELOG

# v2.0.4 (2021-09-09)

  * 订阅接口支持promise

  * 修复部分重连产经bug
#  v1.12.2 (2021-08-12)

  * 调整主讲人切换间隔

  * 修复部分已知bug
#  v1.12.0 (2021-07-20)

  * 升级音视频SDK

  * 修复部分已知bug
# v1.10.0 (2021-07-08)

  * 支持仅受邀人可参会功能

  * 支持已有会议成员粒度的Tag字段

  * 增加上报日志方法

  * 修复部分已知bug
# v1.9.1 (2021-06-02)

  * 修复会议锁定展示状态异常问题

  * 修正屏幕共享主持人操作异常问题

  * 修正屏幕共享声音异常问题

# v1.8.1 (2021-04-29)

  * 增加共享时支持显示视频

  * 创建加入会议增加字段

    * *cloudRecordOn* 是否开启服务端录制配置项

  * 增加额外会议信息 *sipId*

  * 优化白板性能消耗问题

  * 修复已知bug
# v1.7.2 (2021-03-30)

  * 增加会中成员进出通知

  * 修复若干bug

    * 全体静音状态异常

    * 会中改名无提示

    * 断网优化

    * 订阅无声音问题修复
# v 1.7.0 (2021-03-17)

* 增加会中改名功能

  * *noRename* 创建，加入会议，会中改名配置

* 修复部分bug

* 新增会中白板功能

  * 新增白板菜单项，控制开启白板共享和结束白板共享

* 新增*defaultWindowMode*选项配置“会议视图模式”，支持普通和白板模式

* 修复部分已知bug
# v1.5.2 (2021-01-15)

* 增加音频订阅方法

  * *subscribeRemoteAudioStream* 订阅用户音频流
  * *subscribeAllRemoteAudioStreams* 订阅所有用户音频流
  * *subscribeRemoteAudioStreams* 订阅用户音频流Bylist

* 修复部分情况下加入会议失败的问题

# v1.5.0 (2020-12-21)

* 增加自定义按钮配置

# v1.3.3 (2020-11-27)

* 补充关闭预约会议密码回调监听

* 补充创建会议提示已存在会议取消操作监听

* 加入会议增加预约会议密码参数*password*

* 调整会议画廊模式展示策略

# v1.3.2 (2020-11-20)


* 新增会议初始化信息配置

  - 额外增加创会，入会时配置项 `meetingIdDisplayOptions` 短号显示规则（可选）

* 增加底部展示参会人数

* 优化了弹窗效果

# v1.3.1 (2020-11-13)

## Added

* 新增会议初始化信息配置
  
  - 额外增加config配置项 `neWebMeeting.actions.init(width, height, config)`

* 新增获取会议短号信息

  - `neWebMeeting.actions.NEMeetingInfo.shortMeetingId`

* 新增两种登陆方式

  - 账密登陆：`neWebMeeting.actions.loginWithNEMeeting`

  - SSO登陆：`neWebMeeting.actions.loginWithSSOToken`