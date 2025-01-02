# final homework
**课程期末作业复现，仅用于期末作业导师查看，请勿用于其他目的，如有侵权会及时删除**<br>
源代码在压缩包中<br>
数据集为国家科研保密文件<br>
如需复现，数据集制作请参考以下简要流程<br>
具体详细数据集制作请参考结课报告

**数据集制作**<br>
*1、预处理*<br>
获取高分一号影像（GF-1影像），对高分一号的原始全色和多光谱图像进行辐射定标、大气校正、正射校正、图像融合等步骤<br>
选取B4、B3、B2波段合成假彩色图像<br>
*2、样本制作*<br>
将收集到的所有影像进行划分，将研究区一部分区域作为样本采集区。其次将融合后的影像导入Geolabel标注软件，在ENVI5.6中导入野外通过GPS定位的样点，根据影像和点位在Geolabel中选取样点，进行标注<br>
将标注的样点裁剪为512×512大小，形成数据集<br>
训练集和验证集占比可自行决定<br>
*3、数据增强*<br>
研究基于Numpy与OpenCV库实现遥感影像和标签图的数据扩充，主要包括对图像的随机翻转、随机旋转、随机裁剪等处理。<br>

**权重文件获取**
通过网盘分享的文件：swin_tiny_patch4_window7_224.pth
链接: https://pan.baidu.com/s/145TuLdxSLXsB_DAdw1eJ0w?pwd=swin 提取码: swin<br>
下载后放入主文件夹下pretrained_ckpt文件夹中

其他操作详见主文件夹中Readme.md
