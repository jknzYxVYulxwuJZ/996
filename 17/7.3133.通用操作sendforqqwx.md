### 拉起微信和qq等功能

`sendforqqwx`

| 参数   | 类型      | 空   | 默认 | 注释                                     |
| :----- | :-------- | :--- | :--- | :--------------------------------------- |
| play   | `object`  | 否   |      | 玩家对象                                 |
| model  | `integer` | 否   |      | 1=拉起QQ<br />2=QQ好友<br />3=QQ群<br />4=微信 |
| param1 | `integer` | 否   |      | 参数2=2,填入QQ号<br />参数2=3,填入QQ群号   |
| param2 | `string`  | 否   |      | 参数2=3,填入QQ群key                      |
```lua
--拉起QQ
sendforqqwx(actor,1)

--拉起QQ好友
sendforqqwx(actor,2,2881xxxx84)

--拉起QQ群,参数3为qq群号,参数4位qq群key(KEY获取地址： https://qun.qq.com/join.html)
sendforqqwx(actor,3,2881xxxx84,"https://qm.qq.com/cgi-bin/qm/qr?k=W_xxxx&amp;jump_from=webapi&amp;authKey=xxxx")

--拉起微信
sendforqqwx(actor,4)
```

