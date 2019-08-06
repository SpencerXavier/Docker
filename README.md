# Docker tutorial - basic command

- container:
-------------
- docker run -it -d(background) -p  8888:8888 image:version bash  
- go inside the container : docker exec -it container_name bash (so the container won't ends)
- docker run -it -v /Users/spencer/Desktop/OpenCV/:/OpenCV yoanlin/opencv-python3 bash
- share the file from container to host :  docker cp mycontainer:/Project/userfiles.txt userfiles.txt


docker建立jupyter notebook: https://medium.com/@jihung.mycena/docker-建立-jupyter-container-8084748e2f33



ps. -d for background , so container won't die
ps. -v :volume (storage)
ps. source directory : des directory



# Docker tutorial
https://github.com/twtrubiks/docker-tutorial

# Docker tutorial - basic command
https://medium.com/@jihung.mycena/docker-建立-jupyter-container-8084748e2f33
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
