# FreeBSD-98wubi-tables

#### 介绍
FreeBSD 使用98 五笔输入法教程

pkg install zh-ibus-rime

环境变量配置：安装好运行初始化命令ibus-setup

将98 五笔码表（wubi86.dict.yaml、wubi86.schema.yaml）复制到/usr/local/share/rime-date 目录下

修改rime-date 目录下default.yaml 文件，打开default.yaml 找到schema_lis：下面第一行添加 - schema: wubi98 保存退出重新加载ibus 输入法即可。
