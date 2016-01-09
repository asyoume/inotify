## inotify是什么？
在做golang开发的时，总需要自己不断的重复去编译代码，这是一个很痛苦的事情，所以我们需要一个自动编译golang源代码的脚本，linux/mac上都支持shell所以有了这个通过监听文件变化，调用shell脚本的插件
## 使用方式
* 1.go get github.com/asyoume/inotify
* 2.在需要监控的目录创建一个配置文件 .inotify,内容为监控目录的子目录名,例如["xxx","xxxx"]，脚本会在主目录和定义的子目录下文件修改时候自动编译
* 3.inotify -h 查看的帮助命令参数