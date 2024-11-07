# Docker
# 实验要求：

启动一个nginx，并将他首页改为自己首页，发布



# 流程：

下载容器 -> 启动容器 -> 修改页面 -> 保存镜像 -> 分享社区



# 下载镜像：

检索：docker search

下载：docker pull

列表：docker images

删除：docker rmi

镜像名：标签(版本)



# 启动容器：

运行：run

查看：ps

停止：stop

状态：stats

日志：logs

进入：exec

删除：rm



# docker run细节

docker run -d --name name xxx

-d：后台运行，

name取的名字，

xxx运行的程序  ，

-p：端口映射    -p aa:bb  aa是容器的端口，bb是主机的端口



# 交互

docker exec -it  name  /bin/bash

-it 交互模式

/bin/bash  控制台





> 以修改nginx为例
>
> nginx的页面在 /usr/share/nginx/html/

```bash
cd  /usr/share/nginx/html/
//有index.html 50x.html
echo "<h1>Hello</h1>" > index.html
```





# 保存镜像

提交： docker commit

保存：docker save

加载：docker load



# 分享社区

登录：docker login

命名 ：docker tag

推送：docker push



# 挂载

目录挂载：-v 、app/nghtml:/xxx/html

挂载配置文件  卷映射： -v ngconf:/etc/nginx



