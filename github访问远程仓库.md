github 访问远程仓库有两种方式：HTTPS 方式和 SSH 方式。

HTTPS是零配置，但是每次访问都要输入账号密码

SSH是需要配置，以后每次访问都是直接访问

### 配置 SSH 访问 github 远程仓库
在当前电脑生成公钥和私钥
输入命令：`ssh-keygen -t rsa -b 4096 -C "792939277@qq.com"`
连按3下回车即可
在 `C:/User/用户文件夹/.ssh` 目录中生成 `id_rsa` 和 `id_rsa.pub` 两个文件

### 配置 SSH key
1. 使用记事本打开 `id_rsa.pub`
2. 在浏览器中登录 Github，点击头像 -> Settings -> SSH and GPG Keys -> New SSH key
3. 将 `id_rsa.pub` 中的内容，粘贴到 Key 对应的文本框
4. 在 Title 文本框中任意填写一个名称，来标识这个 Key 从何而来

### 测试 SSH 是否配置成功
`ssh -T git@github.com`