server:
下载vncserver安装
两个电脑关系：电脑A远程电脑B，查看和操作电脑B里面的东西
电脑B:
1.下载vncserver并注册一个enterprise类型的账号，注意，一定要是enterprise类型的，见博客[](https://blog.csdn.net/mollerlala/article/details/105750465)
2. download or git clone此项目
3. npm install
4. 将websockify-js目录复制到noVNC目录,此项目中已经复制好
5. 将noVNC目录复制到npm install之后出现的node_modules目录
6. 命令行切换到nodel_modules\noVNC\websockify-js\websockify目录，也就是带有websockify.js的文件夹下面，因为我们是js版的，不是python版的。
7. 执行下方命令
node websockify.js --web D:\phpStudy\PHPTutorial\WWW\git\novnc-browser\node_modules\noVNC 6080 你自己的serverIp:你自己的serverPort
命令中的路径D:\phpStudy\PHPTutorial\WWW\git\novnc-browser\这部分请改为你自己下载或者克隆项目的存放路径；
6080为 novnc/utils/launch.sh中默认的，你可以随便设置一个端口，比如1111，2222等
你自己的serverIp是vnc server这个软件启动后带的
你自己的serverPort是vnc server这个软件设置的，默认是5900
8. vnc server的security的encryption配置为prefer on(这个视情况来哦)

电脑A：
1.浏览器打开网址即可
电脑B第七步的serverIp:6080/vnc.html
如果控制台出现no supported type就配置电脑B的第八步

