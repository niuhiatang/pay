微信个人收款免签系主要用来解决没有营业执照，想使用微信和支付宝收款，收款的逻辑

通过极速框架开发，实现收款通知订单管理，收款通知回调等功能;

特点：支付回调通知，0手续费实时到账，全部服务端源代码，随意接入其他系统；

实现原理： 监听支付宝客户端推送信息，最安全的一种

安装方式
宝塔面板安装集成环境，再安装极速框架即可

1.上传收款二维码

2.收款二维码和商品价格的关系：
用户付款后 -> 客户端通知后台 微信 或者 支付宝，收到多少金额，后台做相应的处理;
3.商品的地址统一是
\addons\pay\library\Service::submitOrder(金额, 唯一订单号);

4.客户端配置说明
api 地址填写：
填写密钥：在后台自由设置

5.请把支付宝/微信/收款客户端加入手机清理白名单，并保持网络畅通；
全部代码开源，暂不提供app监控端代码
程序适合中小站长使用
———————————————
