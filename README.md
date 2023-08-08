# 解决 Mac 中英文切换频繁出错（删除 ABC）

1、打开系统偏好设置 → 键盘 → 输入法 → 添加 `US 美国`（Big Sur 及之前版本是 `🇺🇸 美国`），再删除 `ABC`。

![](https://i.imgur.com/qhpNu0q.png)

2、访达前往文件夹（快捷键：Command-Shift-G）输入下面路径并用 [Xcode](https://apps.apple.com/cn/app/xcode/id497799835?mt=12) 软件打开 
（路径里 `XXX` 替换为 Mac 用户名）。
```
/Users/XXX/Library/Preferences/com.apple.HIToolbox.plist
```

3、删除所有包含 `U.S.` 的文件并保存。

![](https://i.imgur.com/q9xTLLL.png)

4、重启 Mac，此时只有一个输入法，切换中英文只需要按 Shift，再也不必担心出错。

![I](https://i.imgur.com/zoyqOsr.png)
> 发现的弊端：设置 - 网络 - 修改 DNS 时可能会无法输入数字，可以选择粘贴进去，不必担心。

## 还原

系统偏好设置 → 键盘 → 输入法 → 添加 `US 美国` 或 `ABC` 即可。
