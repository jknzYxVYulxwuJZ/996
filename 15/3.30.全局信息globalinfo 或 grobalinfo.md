### 获取全局信息
`globalinfo` 或 `grobalinfo`
* 说明 id 对应值
0: 全局玩家信息
1: 部署时间开始 开发天数 **开区天数建议获取常量`&lt;$KFDAY&gt;`**
2: 部署时间开始 开服时间 **开服时间建议获取常量`&lt;$showtime&gt;`**
3: 合服次数
4: 合服时间
5: 服务器IP
6: 玩家数量
7: 背包最大数量
8: 引擎版本号（以线上版本为准,测试版、本地版可能存在差异）
9：游戏id
~~10：服务器名称~~**获取异常,用常量`&lt;$SERVERNAME&gt;`**
11：服务器id

```lua
    function main(self)
        say(self,"当前开服天数"..globalinfo(1).."在线玩家数:"..globalinfo(6))
    end
```

