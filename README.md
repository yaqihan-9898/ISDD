# Infrared Ship Detection Dataset (ISDD)

Our paper **"Knowledge-Driven Deep Network for Infrared Ship Detection under Complex Ocean Environment"** is under review, and we decide to public our dataset in advance.

I. Introduction
--

**Infrared Ship Detection Dataset (ISDD)** is a public datasets with **1284** infrared remote sensing images and **3061** ship instances. The image size is 500*500. Our ISSD collects images taken by the Landsat8 satellite, which carries the Operational Land Imager (OLI) with nine imaging bands and Thermal Infrared Sensor (TIRS) with two Thermal Infrared imaging bands. We fuse three OLI bands of Band 7, Band 5, and Band 4 to obtain short-wave infrared images. All images in ISDD are preprocessed by radiometric calibration and FLAASH atmospheric correction.



In ISDD, there are 373 inshore scenes containing 924 instances and 911 offshore scenes containing 2137 instances. 

We split the dataset into training set, validation set, and test set according to the ratio of 6:1:3. The detailed statistics of the dataset division are listed in Table 1. 

<p align="center">Table I</p>

<div align=center>
  
|    -      | Train   |  Validation  |  Test  |  Total| 
| :--------:   | :-----:  | :-----:  | :----:  | :----:  |
| Image Number    | 765 |   134     |385|1284|
| Instance number        |   1799   |   303   |959|3061|

</div>
  
Fig.1 displays several typical scenes in ISDD such as ships with trail, inshore scenes, berthing scenes, sea wave scenes, thin clouds scenes, and thick clouds scenes.


<div align=center><img width="800" src="https://github.com/yaqihan-9898/ISDD/blob/main/typical%20scenes.png"/></div>
<p align="center">Fig. 1 Typical Scenes in ISDD</p>


II. Annotations
--
Limited by the resolution of infrared images, small ships, which are often densely packed, are largely invisible in the image. Therefore, we annotate the ship instances with horizontal bounding boxes (xmin,ymin,xmax,ymax), which are enough for dispersed medium and large ships.

The annotations follows the VOC format with .xml files.

III. How to obtain
--
You can get ISDD at (1) [Google Drive][1] or (2) [Baidu Netdisk][2] with access code **asdf**

[1]:https://drive.google.com/file/d/18PwPXoEpKhmq_qqXLHL-v9SB2lukmZPo/view?usp=sharing
[2]: https://pan.baidu.com/s/1VfCbiWnjPoXoI4MaH0VkXw 
