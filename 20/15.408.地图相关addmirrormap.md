### 添加-addmirrormap
`addmirrormap`

| 参数      | 类型      | 空   | 默认               | 注释                                   |
| :-------- | :-------- | :--- | :----------------- | :------------------------------------- |
| oldMap    | `string`  | 否   |                    | 原地图ID                               |
| NewMap    | `string`  | 否   |                    | 新地图ID                               |
| NewName   | `string`  | 否   |                    | 新地图名                               |
| time      | `integer` | 否   |                    | 有效时间(秒)                           |
| BackMap   | `string`  | 否   |                    | 回城地图(有效时间结束后，传回去的地图) |
| miniMapID | `integer` | 否   | 引擎64_23.0628新增 | 小地图编号                             |
| posmX     | `integer` | 否   | 引擎64_23.0628新增 | 返回地图的X坐标                        |
| posmY     | `integer` | 否   | 引擎64_23.0628新增 | 返回地图的Y坐标                        |
| result    | `bool`    |      |                    | 是否成功创建                           |

```lua
[[
MapInfo.txt
[0 比奇]
[01|0 比奇-1]
[02|0 比奇-2]
[03|0 比奇-3]

这个配置的意思是 地图代码 01、02、03的地图都镜像地图代码为0的地图，
这样你就可以拥有3个比奇了，而玩家客户端上调用的都只是0.map文件

注意：被镜像的原地图必须先被服务器读取，因为MapInfo.txt读取方式是从上到下
所以被镜像的原地图应该在镜像地图的上面。

注意：用addmirrormap接口创建的镜像地图不能以01、02、03为原地图ID,需要以0为原地图ID。
]]
function main(actor)
    name_1 = name_1 and name_1 + 1 or 1
    --地图
    local oldMapId  = "0"
    local newMapId  = "0" .. getbaseinfo(actor, 2).. name_1  --新地图
    local mapName   = string.format("比奇[%d]",name_1)
    local mapTime   = 10   --地图持续时间
    --删除地图
    delmirrormap(newMapId)
    --创建镜像地图
    addmirrormap(oldMapId, newMapId, mapName, mapTime, 3,1,333,333)
    --刷怪
    genmon(newMapId,14,14,"练功稻草人",10,10)
    --进入地图
    map(actor, newMapId)
end
```

