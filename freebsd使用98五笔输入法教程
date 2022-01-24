freebsd 使用fcitx5及98五笔（注：本输入法是在gnome3下的sh配制）

-、安装fcitx5 
pkg install fcitx5 fcitx5-qt fcitx5-gtk fcitx5-configtool zh-fcitx5-chinese-addons

二、配制fcitx5
创建.xprofile文件，直接复制freebsd下的.profile重命名并输入下面三年行代码
export GTK_IM_MODULE=fcitx
export QT_IM_MODULE=fcitx
export XMODIFIERS=@im=fcitx

三、添加gnome3托盘扩展插件
pkg install -y firefox chrome-gnome-shell
找topiconsfix添加这个是输入法托盘必备（千万别安装AppIndicator and KStatusNotifierItem Support这个托盘插件，这个会使freebsd卡死崩溃）

四、挂载98五笔
把98wbx.conf文件复制到"/usr/local/share/fcitx5/inputmethod/"（inputmethod目录）下面
把fcitx-98wubi.png和org.fcitx.Fcitx5.fcitx-98wubi.png图标复制到"/usr/local/share/icons/hicolor/48x48/apps/"（apps目录）下面
把98wbx.main.dict词库放到/usr/local/share/libime/（libime目录）下面
重起fcitx5，在fcitx5-configtool起用98五笔即可

王码98五笔生成.dict库方法，直接用下面命令生成
libime_tabledict 98wbx.txt 98wbx.main.dict


