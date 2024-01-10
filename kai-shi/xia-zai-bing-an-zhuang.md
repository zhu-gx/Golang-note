# 下载并安装

## Windows安装

msi文件下载：

* [https://go.dev/dl/](https://go.dev/dl/)

例如选择[go1.21.5.windows-amd64.msi](https://go.dev/dl/go1.21.5.windows-amd64.msi)

1. 打开下载的MSI文件，然后按照提示安装Go。
2. 验证是否安装成功：
   1. 在Windows中，单击Start菜单。
   2. 在菜单的搜索框中，键入cmd，然后按Enter键。
   3. 在出现的命令提示符窗口中，键入go version
   4. 确认命令打印已安装的Go版本。

```powershell
PS C:\Users\guanxin> go version
go version go1.21.5 windows/amd64
```

## Linux安装

1. 从[官网](https://go.dev/dl/)下载Linux版本的压缩包
2. 移动到Linux系统下的文件夹内，（如果此前安装过go）通过删除/usr/local/go文件夹来删除此前的go安装，然后将下载的安装包解压缩到/usr/local 中（注意前面需要加sudo，使用管理员权限）：`$ rm -rf /usr/local/go && tar -C /usr/local -xzf go1.21.6.linux-amd64.tar.gz`
3. 将/usr/local/go/bin 添加到环境变量中：`export PATH=$PATH:/usr/local/go/bin`
4. 键入以下命令来验证是否已安装 Go：`$ go version`
