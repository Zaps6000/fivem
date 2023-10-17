---
ns: CFX
apiset: client
---
## SEND_NUI_MESSAGE

```c
BOOL SEND_NUI_MESSAGE(char* jsonString);
```


## Parameters
* **jsonString**: 

## Return value

## Examples
```
local data = {
    action = "displaySomething",
    text = "Hello, world!"
}

-- Convert the Lua table to a JSON string
local jsonStr = json.encode(data)

local result = send_nui_message(jsonStr)

if result then
    print("sent to NUI.")
else
    print("Failed  NUI.")
end
