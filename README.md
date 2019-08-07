# Docker tutorial - basic command

- container:
-------------
1. docker run -it -d(background) image:version bash  
2. go inside the container : docker exec -it container_name bash (so the container won't ends)
3. docker run -it -v /Users/spencer/Desktop/OpenCV/:/OpenCV yoanlin/opencv-python3 bash
4. share the file from container to host :  docker cp mycontainer:/Project/userfiles.txt userfiles.txt

-------------
- docker建立jupyter notebook: 
1. Host machine : docker run -it -d -p 8888:8888 tensorflow/tensorflow:nightly-py3-jupyter
2. Inside the Container : jupyter notebook --ip 0.0.0.0 --no-browser --allow-root (or use jupyter notebook --port 9999)
3. Host machine access this url : http://127.0.0.1:8888/?token=... (paste the token,use jupyter list)
4. jupyternotebook 常用指令:https://www.itread01.com/content/1548302963.html
 






ps. -d for background , so container won't die
ps. -v :volume (storage)
ps. source directory : des directory
ps. -p 8888(host machine port,可自訂):8888(jupyternotebook default)
ps. --no-browser 不要有網頁顯示出來
ps. IPV4中，0.0.0.0地址被用于表示一个无效的，未知的或者不可用的目标。 
* 在服务器中，0.0.0.0指的是本机上的所有IPV4地址，如果一个主机有两个IP地址，192.168.1.1 和 10.1.2.1，并且该主机上的一个服务监听的地址是0.0.0.0,那么通过两个ip地址都能够访问该服务


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























