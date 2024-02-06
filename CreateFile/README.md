# 在MAC上创建空白文件

这个快捷指令可以轻松的让你在MAC上的任意目录下创建任意类型的空白文件。

## 指令设置

先让快捷指令接收用户要创建的文件名，然后调用`applescript`创建文件。

```applescript
on run {input, parameters}
	tell application "Finder"
		set fileName to input
		set filePath to (the target of the front window) as text
		make new file at filePath with properties {name:fileName}
	end tell
	return input
end run
```

![shortcuts](https://babyno.top/imgs/posts/2024-01-23-create-files-anywhere-on-your-mac-with-apple-shortcuts/shortcuts.webp)

## 成果

创建空白文本文件：

![](https://babyno.top/imgs/posts/2024-01-23-create-files-anywhere-on-your-mac-with-apple-shortcuts/example1.gif)

创建空白任意文件：

![](https://babyno.top/imgs/posts/2024-01-23-create-files-anywhere-on-your-mac-with-apple-shortcuts/example2.gif)

如果你想了解更详细的细节，请查看：https://babyno.top/posts/2024/01/create-files-anywhere-on-your-mac-with-apple-shortcuts/

## 下载地址

https://www.icloud.com/shortcuts/951edcaf19bb45d8be6f9a90532e253d