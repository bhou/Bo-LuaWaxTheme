Bo-LuaWaxTheme
==============

LuaWaxTheme is a lib to customize iOS application's look and feal. 
This project is used in Bo-AntibesBus project to support multiple themes.

LuaWaxTheme provides a series of util functions to help you easily create iOS components.
for example: a UITableView can be created in the following code:
`````lua
local tableView = TB.table("mytable") -- 'mytable' is the theme resource definition
`````

The 'mytable' resource can be defined as:
`````lua
return {
  -- other resources
  ...
  
  mytable={
    background={
      image="tablebackground.png",
      edgeInsects={10, 0, 10, 0},
      -- if image is defined color will no be applied
      color = {0.3, 0.5, 0.6, 1}
    },
  },
  -- other resources
  ...
}
`````
