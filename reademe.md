server:
下载vncserver安装
browser:
1. download or git clone
2. npm install
3. 将websockify-js目录复制到noVNC目录,此项目中已经复制好
4. 将noVNC目录复制到node_modules目录
5. cmd到noVNC\websockify-js\websockify目录，也就是带有websockify.js的文件夹下面
6. 执行下方命令
node websockify.js --web D:\\phpStudy\PHPTutorial\WWW\vnc\node_modules\noVNC 6080 你自己的serverIp:你自己的serverPort



