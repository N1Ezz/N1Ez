### 登录成功后展示的欢迎信息 修改方法
1. 修改 /etc/motd 文件【vim /etc/motd】

### 修改命令行 shell命令前的提示词 修改方法
1. 修改.bash_profile 【vim ~/.bash_profile】
2. 修改 export PS1=" 这里写想要展示的内容 "
   \d – Current date
   \t – Current time
   \h – Host name
   
   – Command number
   
   \u – User name
   \W – Current working directory (ie: Desktop/)
   \w – Current working directory with full path (ie: /Users/Admin/Desktop/)
3. 激活修改的设置 执行【source ~/.bash_profile】

例: 当前 [root@iZ8vbipm4vunjxjsxirahiZ ~]# 这种样式是 export PS1="[\u@\h \W]"