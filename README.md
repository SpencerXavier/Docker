# Docker tutorial
https://github.com/twtrubiks/docker-tutorial

# Docker tutorial - basic command
https://blog.csdn.net/dongdong9223/article/details/52998375
http://seanlook.com/2014/10/31/docker-command-best-use-1/
http://seanlook.com/2014/11/05/docker-command-best-use-2/


# Docker put the files inside the comtainer
docker run -it -v /Users/spencer/Desktop/OpenCV/:/OpenCV yoanlin/opencv-python3 bash
ps. -v :volume (storage)
ps. source directory : des directory













# wildfire
-how to use DIGITS and run on jeston nano(you can test your own data )
https://github.com/dusty-nv/jetson-inference
ps. download and extract the trained model snapshot to Jetson (snapshot is in job)
NET = snapshot folder , png = your own data
segnet-console north_firecam_720.png output_firetower.png --prototxt=$NET/deploy.prototxt --model=$NET/snapshot_iter_4522.caffemodel --labels=$NET/fpv-labels.txt --colors=$NET/fpv-deploy-colors.txt --input_blob=data --output_blob=score_fr



use custom dataset to train models in digits (you can also test inference on digits)



# linux
http://www.polish.url.tw/ach4/ach4.html#sed_adv
