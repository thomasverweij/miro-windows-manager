This is a fork of [MiroWindowsManager](https://github.com/miromannino/miro-windows-manager)

Added `middle`, `fullscreenAll` and `middleAll` functions.

Example init.lua:
```
local hyper = {"ctrl", "alt", "cmd"}

hs.loadSpoon("MiroWindowsManager")

hs.window.animationDuration = 0.3
spoon.MiroWindowsManager:bindHotkeys({
  up = {hyper, "up"},
  right = {hyper, "right"},
  down = {hyper, "down"},
  left = {hyper, "left"},
  fullscreen = {hyper, "f"},
  middle = {hyper, "g"},
  fullscreenAll = {hyper,"r"},
  middleAll = {hyper,"t"}
})
```