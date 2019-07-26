# Docker tutorial
https://github.com/twtrubiks/docker-tutorial

# Docker tutorial - simple version
https://blog.csdn.net/dongdong9223/article/details/52998375


# Docker put the files inside the comtainer
docker run -it -v /Users/spencer/Desktop/OpenCV/:/OpenCV yoanlin/opencv-python3 bash
ps. -v :volume (storage)
ps. source directory : des directory


# wildfire
-how to use DIGITS and run on jeston nano
https://github.com/dusty-nv/jetson-inference
ps. download and extract the trained model snapshot to Jetson (snapshot is in job)
NET = sanpshot folder
segnet-console north_firecam_720.png output_firetower.png --prototxt=$NET/deploy.prototxt --model=$NET/snapshot_iter_4522.caffemodel --labels=$NET/fpv-labels.txt --colors=$NET/fpv-deploy-colors.txt --input_blob=data --output_blob=score_fr



use custom dataset to train in digits



# linux
http://www.polish.url.tw/ach4/ach4.html#sed_adv
