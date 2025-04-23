### 返回前端面板消息[合成系统]

`sendactionofjson`

&gt; **&lt;font color="#808080" style="font-size: 13px;"&gt;引擎64_24.05.23新增接口&lt;/font&gt;**

| 参数  | 类型     | 空   | 默认 | 注释      |
| :---- | :------- | :--- | :--- | :-------- |
| actor | `object` | 否   |      | 玩家对象  |
| idx   | `string` | 否   |      | 合成表idx |
| json  | `string` | 否   |      | json信息  |
```lua
function g_compounditem10000(actor,idx)
    local data_json = string.format('{"action":"event","data":{"recog":%s,"param1":%s}}',"-2",idx)
    sendactionofjson(actor,idx,data_json)
end
```
