# 到期或欠费

RDS实例到期或欠费的7天内数据库实例保留但不可用，可在实例到期或欠费7天内进行续费或充值后恢复数据库实例使用。

## 包年包月实例

| 时间段                     | 处理机制                                                     |
| :------------------------- | :----------------------------------------------------------- |
| 到期前30天~到期前1天       | 1、到期前30、15、7、3、1天，系统给用户推送资源即将到期的提醒； <br>    2、通知以邮件、短信、站内信的方式推送； |
| 到期当天                   | 1、对已到期未续费的资源，到期后云资源将被立即停服，系统给用户推送到期停服通知；<br>2、通知以邮件、短信、站内信的方式推送； |
| 到期当天停服后~到期后第7天 | 1、如在此期间对资源做续费处理，则云资源会自动启动服务，用户可继续使用；<br>2、如在此期间对资源不做续费处理，则系统会在到期停服后的第4、6天，给用户推送资源即将释放的提醒； |
| 到期后第8天                | 1、若用户仍未进行续费，系统将销毁云资源，其数据将被清除且不可恢复；<br>2、资源因到期销毁后，以邮件、短信、站内信的方式通知用户； |

## 按配置付费实例



| 时间段             | 处理机制                                                     |
| :------------------ | :------------------------------------------------------------ |
| 后付费资源生成账单 | 1、根据计费周期，按资源生成账单，执行扣费； <br>    2、账户余额不足，无法完成扣费，则账户进入欠费状态。系统将为用户推送该云资源欠费通知。 |
| 欠费状态使用期     | 客户欠费后，进入欠费使用期（欠费使用期为1天），该期间客户可继续使用资源，资源会正常计费； |
| 欠费状态停服期     | 客户欠费后进入欠费停服期（欠费停服期为7天）<br>1、客户正在使用的欠费资源将强制停服关闭；<br>2、已经关闭的服务配置和资源将保留至停服期结束，期间如果正常充值补缴费用，对应资源将自动重新启动服务；<br>3、在停服期内，如未补缴费用，停服后第4、6天，系统将为用户推送该云资源欠费即将释放资源的通知。 |
| 欠费状态资源释放   | 客户欠费超过欠费停服期，启动欠费资源释放；<br>1、按配置计费的资源，资源将被释放；<br>2、系统推送客户资源释放通知。 |
