# windowbuilder
build em windows n stuff

**Usage**
```lua
local WindowBuilder = loadstring(game:HttpGet("https://raw.githubusercontent.com/sharpcystals-github342/windowbuilder/refs/heads/main/main.lua"))()

local window = WindowBuilder.createWindow(UDim2.new(0.5, -150, 0.5, -100), UDim2.new(0, 300, 0, 200), "something")

local closedConnection = window.windowClosed:Connect(function()
print("Window is closing")
end)

local minimizingConnection = window.windowMinimising:Connect(function()
print("Window is minimizing")
end)
--[[
  Window:
    self.windowPosition: UDim2
    self.windowSize: UDim2
    self.title: string
    self.processID: number
    self.UI: Instance
    self.MainFrame: Instance
    self.windowClosed: Event
    self.windowMinimising: Event
    self.minimized: boolean
    self.minimizedButton
    self.storedContents
]]
```
