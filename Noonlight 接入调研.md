Noonlight 接入调研

### 接入类型

* Dispatch API

方法：推送纯文本告警信息到Noonlight并等待接收Noonlight的反馈结果

```mermaid
sequenceDiagram
meShare->>Noonlight: 推送告警消息
Noonlight->>User: 确认告警(通过电话)
User-->>Noonlight:确认是告警
Noonlight->>Police:报案
Noonlight-->>meShare:反馈结果
Police->>User:处理告警
```

   以下是官方流程图：
![avatar](https://raw.githubusercontent.com/xjr20042/public-img/master/Dispatch%20API.png)

* Video Monitoring

Dispatch API的升级版，在Dispatch API的基础上增加告警视频，Noonlight会判断告警视频
    ![avatar](https://raw.githubusercontent.com/xjr20042/public-img/master/Video%20Monitoring.png)

### 价格

![avatar](https://raw.githubusercontent.com/xjr20042/public-img/master/pricing.png)

### 信息收集

#### 用户信息

1. 真实姓名
2. 手机号码
3. 详细住址

#### 开发者账号

需要一个美国手机号码来注册开发者账号