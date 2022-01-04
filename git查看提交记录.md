查看历史提交记录:git log
查看前二行：git log -2
使用短格式查看：git log -2 --pretty=oneline
使用自定义格式查看：
%ar 是日期
%s 是提交文本
%h 是哈希
%an 是用户名
实例：git log -2 --pretty="%ar | %an | %s"