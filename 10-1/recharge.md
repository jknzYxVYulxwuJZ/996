### 充值触发

`recharge`

&gt; 充值时玩家不在线,则会在下次登陆时触发

| 参数           | 类型      | 空   | 默认                | 注释                             |
| :------------- | :-------- | :--- | :------------------ | :------------------------------- |
| self           | `object`  | 否   |                     | 玩家对象                         |
| Gold           | `integer` | 否   |                     | 充值金额                         |
| ProductId      | `integer` | 否   |                     | 产品ID（来源客户端充值面板调用） |
| MoneyId        | `integer` | 否   |                     | 货币ID                           |
| isReal         | `integer` | 否   |                     | =1真实充值<br />=0扶持充值         |
| orderTime      | `integer` | 否   | 引擎64_24.03.14新增 | 订单时间(时间戳)                 |
| rechargeAmount | `integer` | 否   | 引擎64_24.03.14新增 | 实际到账货币金额                 |
| giftAmount     | `integer` | 否   | 引擎64_24.03.14新增 | 额外赠送金额<br />运营后台配置     |
| refundAmount   | `integer` | 否   | 引擎64_24.03.14新增 | 开启积分金额<br />运营后台配置     |

------------

