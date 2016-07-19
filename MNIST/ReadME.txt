
MNIST是一个开放的、带标签的手写体数字数据库，它包括训练集和测试集两部分。其中，训练集有60000张28*28尺寸的手写体数字灰度图片，而测试集有10000张同样性质的图片。在本文中，每张图片可表示成一个28*28的行列矩阵，并将其按列伸展成一个784*1的列向量，然后在最后一位后面添加该图片的类别标签，组成一个785*1的列向量；故此，MNIST数据集可以编码成一个785*60000+785*10000（训练集+测试集）尺度的矩阵，每一列前784代表一个手写体数字样本，最后1位是该样本的标签。具体数据参看mnist.mat文件：train=（785*60000），test=（785*10000），pic_rows=28,pic_cols=28。

The MNIST database is a public large database of handwritten digits, which are allocated manually supplied labels and divided into training and testing parts respectively. More specifically, the training set holds 60000 grayscale pictures with 28*28 dimensions for each, while there are 10000 images accordingly in the testing part. In this article, each handwritten digit picture would be represented to a 28*28 matrix, and further be reshaped to a 784*1 vector; and then convert each vector into 785*1 shape by putting corresponding label on its bottom. Consequently, the whole handwritten digit corpus equates to two separate matrices: 785*60000 (training set) and 785*10000 (testing set), and each column represents one handwritten digit image. The concrete digital dataset is coded in mnist.mat with variables train (785*60000), test(785*10000), pic_rows (28), and pic_cols (28).

For more information, you can refer to http://yann.lecun.com/exdb/mnist/.


