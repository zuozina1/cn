# 修改弹性公网IP带宽

京东云支持全计费类型的弹性公网IP实时进行升配与降配操作，本文将详细介绍如何修改公网IP的带宽上限。

## 操作场景

- 根据业务需要实时调整公网IP带宽上限，如当前带宽上限不能满足业务需求，提升带宽上限，如当前业务量降低，可降低公网IP的带宽上限。

## 前提条件及限制

- 确保您已经[注册京东云账号](https://user.jdcloud.com/register?returnUrl=https%3A%2F%2Fwww.jdcloud.com%2F)，并实现[实名认证](https://docs.jdcloud.com/cn/real-name-verification/introduction)；
- 确保您已经创建一个弹性公网IP；
- 包年包月计费类型，升配需要补带宽差价，降低带宽上限根据带宽差价等值延长到期时间，不支持退差价；
- 按配置计费类型，升配与降配后均按照调整后带宽出账单；
- 按用量计费类型，带宽仅用来限制速率，不影响实际计费；
- 带宽范围为0~200Mbps，按用量计费的公网IP不支持调整超出范围的带宽上限（加入共享带宽中除外）；
- 按配置或按用量计费的公网IP加入共享带宽包后，公网IP的带宽上限不生效，IP的最大带宽上限为共享带宽包的带宽上限，不支持在公网IP侧修改带宽，如需修改带宽上限，请前往共享带宽包中修改，可参考[单IP限速](https://docs.jdcloud.com/cn/shared-bandwidth-package/manage-public-ip#user-content-3)。

## 操作步骤

步骤1：登录京东云控制台，进入控制台导航页面；

步骤2：在控制台左侧导航栏，选择网络-【私有网络】-【弹性公网IP】，进入弹性公网IP列表页；

步骤3：在弹性公网IP列表页，定位到需要调整带宽的弹性公网IP，在操作列点击【更多】选择【修改带宽】按键，进入修改带宽弹窗；

> 注：弹性公网IP详情页右上角快捷操作菜单同时提供绑定资源按键，功能与列表页按键保持一致。

步骤4：在修改带宽弹窗，调整滑块或输入带宽值，指定需要修改的带宽；

> 注：带宽上限值仅支持带宽范围内的正整数。


步骤5：在修改带宽弹窗，点击【确定】按键，进入订单确认页；


> 注：按用量计费的公网IP无订单确认页，点击【确定】后即完成带宽上限修改。


步骤6：在订单确认页，点击立即开通，完成支付并返回弹性公网IP列表页，查看带宽修改情况。

## 相关参考

- [使用限制](../../Introduction/Restrictions.md)
- [常见问题](https://docs.jdcloud.com/cn/elastic-ip/faq)
- [创建公网IP](Create-Elastic-IP.md)
- [单IP限速](https://docs.jdcloud.com/cn/shared-bandwidth-package/manage-public-ip#user-content-3)

