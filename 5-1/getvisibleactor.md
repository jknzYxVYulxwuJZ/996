### 根据唯一id获取视野内的目标对象

`getvisibleactor`

&gt; **&lt;font color="#808080" style="font-size: 13px;"&gt;引擎64_24.08.07新增接口,替换引擎:[996M2.rar](http://engine-doc.996m2.com/server/index.php?s=/api/attachment/visitFile&amp;sign=6994fd675e9a3598850b552923623aff "[996M2(2024.08.07.0_64位)[20241106].rar")&lt;/font&gt;**

&lt;font color="#ff00ff" style="font-family: Fixedsys;font-size: 15px;"&gt;**特殊：该接口只能获取玩家[参数1]视野内的目标,用于解决TXT调用LUA时获取对象困难问题**&lt;/font&gt;

| 参数       | 类型     | 空   | 默认 | 注释           |
| :--------- | :------- | :--- | :--- | :------------- |
| player     | `object` | 否   |      | 玩家对象       |
| userID     | `string` | 否   |      | 目标唯一ID       |
| result     | `object`   | 否   |      | 返回值，目标对象 |

```lua
    -- userID 可以是玩家/英雄/怪物/宠物/人形怪的
    function main(actor,userID)
        local objcet = getvisibleactor(actor,userID)
        release_print("根据唯一id获取视野内的目标对象",userID,getbaseinfo(objcet,1))
    end
```
