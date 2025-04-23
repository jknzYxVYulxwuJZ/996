### 发送邮件
`sendmail`

|参数|类型|空|默认|注释|
|:----    |:-------    |:--- |---|------      |
|userid |`string`    |否   |    |   玩家UserId，如果是玩家名，需要在前面加#，如:#张三 |
|id |`integer`    |否   |    |自定义邮件ID |
|lable |`string`    |否   |    |邮件标题 |
|memo |`string`     |否   |     |邮件内容 |
|Rewards |`string`    |否   |    |附件内容：物品1#数量#绑定标记&amp;物品2#数量#绑定标记，&amp;分组，#分隔<br />绑定标记值参考物品帮助 |

```lua
function main(self)
    sendmail(getbaseinfo(self,2),1,"测试","物品发放","木剑#2")
end
```

## 商城相关

