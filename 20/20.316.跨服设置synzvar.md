### 跨服变量传递

`synzvar`

| 参数    | 类型      | 空   | 默认 | 注释                                                                     |
| :------ | :-------- | :--- | :--- | :----------------------------------------------------------------------- |
| itype   | `integer` | 否   |      | 变量类型<br />1=全局G变量<br />2=全局A变量<br />3=全局自定义变量<br />4=行会变量 |
| astr    | `string`  | 否   |      | 变量名<br />itype=4的时传入:`行会名称/变量名`                              |
| bstr    | `string`  | 否   |      | 存入本服全局变量名                                                       |
| func_id | `integer` | 否   |      | 同步成功后触发函数id<br />如传入1则同步成功后触发`kfsynvar1`函数           |

```lua
    -- 同步全局G/A/自定义变量
    local varName_1 = "G15"
    local varName_2 = "G16"
    if checkkuafuserver() then
        setsysvar(varName_1, getsysvar(varName_1) + 1)
        release_print("跨服",varName_1, "valValue" .. getsysvar(varName_1))
    else
        if not kfsynvar1 then
            function kfsynvar1()
                release_print("同步成功",getsysvar(varName_2))
            end
        end
        synzvar(1,varName_1,varName_2,1)
    end

    -- 同步行会变量
    local varName_1 = "行会自定义变量"
    local varName_2 = "A10"
    if checkkuafuserver() then
        local guild = getmyguild(actor)
        if guild ~= "0" then
            iniguildvar(guild, "integer", varName_1)
            local value = getguildvar(guild, varName_1) + 1
            setguildvar(guild, varName_1, value)
        end
    else
        local guild = getmyguild(actor)
        if guild ~= "0" then
            local guild_name = getguildinfo(guild,1)
            if not kfsynvar996 then
                function kfsynvar996()
                    LOGPrint("同步成功,行会变量",getsysvar(varName_2))
                end
            end
            synzvar(4,guild_name.."/"..varName_1,varName_2,996)
        end
    end
```

