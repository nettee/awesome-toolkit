# IntelliJ IDEA keymap 设计

## 26 个字母常用快捷键

Mac 通用-窗口：

+ ⌘M 最小化窗口
+ ⌘H 隐藏窗口
+ ⌘W 关闭标签页/窗口
+ ⌘Q 退出程序

Mac 通用-编辑：

+ ⌘A 全选
+ ⌘X 剪切
+ ⌘C 复制
+ ⌘V 粘贴
+ ⌘S 保存
+ ⌘Z 撤销

查找类：

+ ⌘F 查找 
+ ⌘R 替换

编辑类：

+ ⌘D Delete line（自定义）
+ ⌘P Parameter info
+ ⌘G Generate code（自定义）
+ ⌘N Generate code（待修改）
+ ⌘J Join lines（自定义）

导航类：

+ ⌘E Open Recent Files
+ ⌘L Go to line
+ ⌘O Go to class
+ ⌘B Go to definition
+ ⌘U Show Usages（自定义）
+ ⌘Y Quick Documentation

未定义：

+ ⌘K 
+ ⌘T 
+ ⌘I


## 最常用功能，以及目前的快捷键

| 类别 | 功能 | 目前快捷键 | 修改方案 |
| :-: | :-: | :-: | :-: |
| Edit | Complete Current Statement | ⇧⌘↩︎ | 保持 |
| Edit | Join lines | ⌃⇧J | ⌘J |
| Edit | Delete line | 忘了 | ⌘D |
| Edit | Show Usages | ?F7 | ⌘U |
| Edit | Find Usages | ?F7 | ⌥⌘U |
| View | Quick documentation | F1 | ⌘Y |
| View | Quick definition | ⌘Y | ⌥⌘Y |
| Navigate | Go to Class | ⌘O | ⌘N |
| Navigate | Go to File | ⇧⌘O | ⇧⌘N |
| Navigate | File Structure | ⌘F12 | ⌘O |
| Code | Generate | ⌘N | ⌘G |
| Code | Completion | ⌃Space | 保持 |
| Code | Cyclic Expand Word | ⌥/ | 保持 |
| Code | Optimize imports | ⌃⌥O | ⌥⌘O |
| Refactor | Refactor this | ⌃T | ⌘T |
| Refactor | Rename | ⇧F6 | ⌥⌘R |
| Refactor | Extract Variable | ⌥⌘V | 保持 |
| Refactor | Extract Method | ⌥⌘M | 保持 |
| Git | Show Diff | 无 | ⇧⌘D |


## F1~F12 键设计

F7~F10 基本上都是 build/run/debug 相关，不适合大改。

F1 在 mac 上目前就是 Quick documentation，等于 Windows 上的 Ctrl+Q。

F11 是 mac 内置快捷键（显示桌面）。