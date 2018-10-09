# 图像像素值的修改

## 任务一：把图像指定区域的红色通道置为255

**1.任务描述：把输入图像中起始点（100，100），宽度为200像素，高度为150像素的区域红色通道置为255.**

2.源图像如下：

![Homework02](https://github.com/SoftwareAutumn/Homework02)/[img02](https://github.com/SoftwareAutumn/Homework02/tree/master/img02)/**second.jpg**

3.任务一代码如下：

![Homework02](https://github.com/SoftwareAutumn/Homework02)/[img02](https://github.com/SoftwareAutumn/Homework02/tree/master/img02)/**01.PNG**

![Homework02](https://github.com/SoftwareAutumn/Homework02)/[img02](https://github.com/SoftwareAutumn/Homework02/tree/master/img02)/**02.PNG**

![Homework02](https://github.com/SoftwareAutumn/Homework02)/[img02](https://github.com/SoftwareAutumn/Homework02/tree/master/img02)/**03.PNG**

4.结果图像如下：

![Homework02](https://github.com/SoftwareAutumn/Homework02)/[img02](https://github.com/SoftwareAutumn/Homework02/tree/master/img02)/**second0.PNG**



## 任务2：把图像指定区域置为白色与黑色

**1.任务描述：把输入图像中起始点（300，300），宽度为100像素，高度为50像素的区域置为白色，同时，把输入图像中起始点为（500，500），宽度为50像素，高度为100像素的区域置为黑色。**

2.任务二代码如下：

![Homework02](https://github.com/SoftwareAutumn/Homework02)/[img02](https://github.com/SoftwareAutumn/Homework02/tree/master/img02)/**04.PNG**

![Homework02](https://github.com/SoftwareAutumn/Homework02)/[img02](https://github.com/SoftwareAutumn/Homework02/tree/master/img02)/**05.PNG**

![Homework02](https://github.com/SoftwareAutumn/Homework02)/[img02](https://github.com/SoftwareAutumn/Homework02/tree/master/img02)/**06.PNG**

3.结果图像如下：

![Homework02](https://github.com/SoftwareAutumn/Homework02)/[img02](https://github.com/SoftwareAutumn/Homework02/tree/master/img02)/**second1.PNG**

## 经验总结

1.在修改指定区域的像素值之前，需要将源图像打开，并创建输出图像poDstDS（任务一），poDstDS1（任务二）.

2.若要修改指定区域的像素值，需要分配源图像的内存(buffTmp0)，及指定区域的内存（白色与黑色区域大小相同，所以共用内存buffTmp1；红色区域用内存buffTmp).否则会造成访问内存失败。

3.若要生成白色与黑色区域，需要对指定区域的==所有通道==的像素值作出修改，生成白色置<u>0</u>，生成黑色置<u>255</u>.

