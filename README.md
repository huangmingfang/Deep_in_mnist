# Deep_in_mnist
- 这是一个学习和研究机器学习和神经网络算法的项目，基于mnist手写数字数据集。作者计划在这个项目中由浅入深逐步实现一些比较先进的机器学习和神经网络算法；
- 因为主要是学习之用，所以在实现核心功能的前提下，重点是代码简单易读；
- 作者将主要参考一些经典的以及近些年的论文，这里有关于mnist识别项目研究论文的一个汇总：[rodrigob.github.io : Classifiction datasets results](http://rodrigob.github.io/are_we_there_yet/build/classification_datasets_results.html#4d4e495354) 
- 关于代码文件，我全部是上传在我本地电脑Jupyter Notebook中保存的文件，里面包括代码、注释、以及交互式运行结果，读者可以下载后直接在Jupyter Notebook中打开即可，界面十分友好，在这里作者也强烈推荐使用Jupyter Notebook进行学习。
## 文件说明
### 1. mnist.pkl.gz
- 这是一个包装很好的mnist数据集，包含所有原始的mnist数据；
- 里面的数据分为3部分，训练集、验证集和测试集，每个数据集都是(X, y)格式，X、y分别为特征数组和标签数组。
- 由于习惯于使用csv格式的数据，以及想自己调整三个数据集的大小，所以我在本地电脑上将其转换成了单个地csv文件，不过文件大小超过了上传限制，所以这里又上传了我的格式转换代码save_all_mnist_to_csv.py。
- 另外需要提醒一下，这个数据集里面的特征数组已经归一化了。
### 2. save_all_mnist_to_csv.py
- 提取mnist.pkl.gz中的数据，得到一个完整数据的.csv文件，其中数据的大小为（70000, 785），共70000个数据，其中标签在第一列。
### 3. 
- 自己动手搭建ANN识别mnist手写数字（正确率91.4%）
### 4. 
- 使用TensorFlow搭建ANN识别mnist手写数字（正确率98.3%）
### 5. 
- 使用TensorFlow搭建CNN识别mnist手写数字（正确率99.3%）-（参考LeNet-5，论文地址：http://yann.lecun.com/exdb/publis/pdf/lecun-98.pdf）-