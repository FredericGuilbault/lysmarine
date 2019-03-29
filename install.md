# Install LysMarine

### 1) Download the latest image file
 [https://archive.org/download/lysmarine-0.8.0.img/lysmarine-0.8.0.img.zip](https://archive.org/download/lysmarine-0.8.0.img/lysmarine-0.8.0.img.zip)

### 2) Extract the image file from the zip archive
Find the downloaded archive — by default, it should be in your Downloads folder.<br>
Double-click on it to extract the files, and keep the resulting Explorer/Finder window open.

Linux CLI:
 ```
 unzip lysmarine-0.8.0.img.zip
 ```

### 3) Copy the lysmarine.img file on the microSd card


Linux CLI (_be careful with this one_):
 ```
 sudo dd if=./lysmarine-0.8.0.img  of=/dev/mmcblk0
 ```

### 4) Enjoy

![](https://projects-static.raspberrypi.org/projects/raspberry-pi-setting-up/5bfb8f69592ea36d75df9d39b8abc186d7815cb6/en/images/pi-sd.png)

<br><br>

###   Next : &nbsp; &nbsp; [ First run, What to do ](doc/userdoc/firstboot.md)
