# Docker tutorial - basic command

- container:
-------------
1. docker run -it -d(background) image:version bash  
2. go inside the container : docker exec -it container_name bash (so the container won't ends)
3. docker run -it -v /Users/spencer/Desktop/OpenCV/:/OpenCV yoanlin/opencv-python3 bash
4. share the file from container to host :  docker cp mycontainer:/Project/userfiles.txt userfiles.txt


1、宿主机文件到容器：docker cp 当前宿主机的文件 容器ID:容器目录：

docker cp /host/path/target  <containerId>:/file/path/within/container 
文件从容器到宿主机： docker cp 容器:容器目录 当前宿主机的文件
 
 
docker cp <containerId>:/file/path/within/container /host/path/target
-------------
- docker建立jupyter notebook: 
1. Host machine : docker run -it -d -p 8888:8888 tensorflow/tensorflow:latest-py3 (再去灌tensorflow2.0.0)
2. Inside the Container : jupyter notebook --ip 0.0.0.0 --no-browser --allow-root
3. Host machine access this url : http://127.0.0.1:8888/?token=... (paste the token,use jupyter list)(記得用完log out 不要quit)
4. jupyternotebook 常用指令:(use jupyter notebook list)
https://www.itread01.com/content/1548302963.html
https://ithelp.ithome.com.tw/articles/10192614
 
ps. -d for background , so container won't die
ps. -v :volume (storage)
ps. source directory : des directory
ps. -p 8888(host machine port,可自訂):8888(jupyternotebook default sever, web port)
ps. --no-browser 不要有網頁顯示出來 --allow-root 你在root 執行必須要用這個flag
ps. --ip=<Unicode>  預設是: 'localhost'，從前面的現實中也可以看出來，表示的是notebook伺服器會監聽的IP地址，我們也可以手動指定


ps. 在服务器中，0.0.0.0指的是本机上的所有IPV4地址(外面看裡面本機的ip)，127.0.0.1是(裡面看外面本機主機的ip)
ps. 0.0.0.0：指的是本机上的所有IPV4地址(外面看裡面時本機的ip)，这发生在主機启动时但又不知道自己的IP地址情况下。如果一个主机有两个IP地址，192.168.1.1 和 10.1.2.1，并且该主机上的一个服务监听的地址是0.0.0.0,那么通过两个ip地址都能够访问该服务
ps. 127.0.0.1：该地址指电脑本身(裡面傳給外面時本機的ip)，主要预留测试本机的TCP/IP协议是否正常。只要使用这个地址发送数据，则数据包不会出现在网络传输过程中。


# Docker tutorial
https://github.com/twtrubiks/docker-tutorial

# Docker tutorial - basic command
https://mileslin.github.io/2019/04/Docker-指令小抄/
https://blog.csdn.net/dongdong9223/article/details/52998375
http://seanlook.com/2014/10/31/docker-command-best-use-1/
http://seanlook.com/2014/11/05/docker-command-best-use-2/
https://www.jinnsblog.com/2018/10/docker-container-command.html





# linux
http://www.polish.url.tw/ach4/ach4.html#sed_adv

# use gitlab to run docker 
edit the dockerfile 
follow the registry
docker run -it -d gitlab-registry.nautilus.optiputer.net/ar-noc/keras-smoke-detection:tag










..上ㄧ業
./目前這頁的folder


1.git init to create .git folder
2.git clone
3.









