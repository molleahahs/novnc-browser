server:
下载vncserver安装
电脑A远程电脑B，查看和操作电脑B里面的东西
电脑B:
1.下载vncserver并注册一个enterprise类型的账号，注意，一定要是enterprise类型的
2. download or git clone
3. npm install
4. 将websockify-js目录复制到noVNC目录,此项目中已经复制好
5. 将noVNC目录复制到node_modules目录
6. cmd到noVNC\websockify-js\websockify目录，也就是带有websockify.js的文件夹下面
7. 执行下方命令，命令中的路径为你下载或者克隆项目的路径，6080为 novnc/utils/launch.sh中默认的
node websockify.js --web D:\\phpStudy\PHPTutorial\WWW\vnc\node_modules\noVNC 6080 你自己的serverIp:你自己的serverPort
8. security的encryption配置为prefer on(这个视情况来)

电脑A：
1.浏览器打开网址即可
电脑B第七步的serverIp:6080/vnc.html
如果控制台出现no supported type就配置电脑B的第八步

