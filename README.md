# html5speed
docker
使用 Docker 一键安装 HTML5 Speedtest

首先安装 Docker

curl -sSL https://get.docker.com/ | sh
systemctl start docker
systemctl enable docker

安装HTML5 Speedtest

docker run -d -p 6608:80 ch6896/html5speedd

参数详解：

-t：启动后显示日志，可用Ctrl+C转入后台运行
-d：后台模式启动
-p 6608:80：镜像映射端口，修改6608为任意端口即可

如果打不开，需要宝塔面板或VPS控制后台放行6688端口

搭建完成，打开 http://你的IP:6608 即可
