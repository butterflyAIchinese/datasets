
ORL是由剑桥大学计算机实验室公开的供科研与学习的人脸识别数据库，它含有400张112*92尺寸的人脸灰度图片，分为40类，每类由同一个人的10张照片组成。在本文中，每张人脸图片可以表示成一幅112*92的行列矩阵，然后将其按列拉直成一个10304*1的向量，然后在最后一位后面添加该图片的类别标签，组成一个10305*1的列向量；故此，人脸数据集可以编码成10305*400尺度的矩阵，每一列前10304位代表一幅灰度人脸图片，最后一位是该样本的标签。具体数据参看orl.mat文件：scale=（10305*400），pic_rows=112,pic_cols=92。

ORL is a public database for research and study usage provided by Cambridge University Computer Laboratory. The database contains 400 face images with 112*92 dimensions for each, which holds 40 classes, and there are 10 different face pictures of the same person in each class. In this context, each face could be represented to a 112*92 matrix, and further be reshaped to a 10304*1 vector; and then each vector would be converted into 10305*1 shape by putting its label on its bottom. Consquently, the whole face corpus equates to a matrix: 10305*400, and each column represents one face image. The concrete digital datasets are coded in orl.mat with variables scale (10305*400), pic_rows (112) and pic_cols (92).


For more information, you can refer to  http://www.cl.cam.ac.uk/research/dtg/attarchive/facedatabase.html
