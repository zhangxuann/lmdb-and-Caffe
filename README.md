# lmdb-and-Caffe
    学习深度神经网络在caffe平台上的编程实现，从原始图片到caffe可读的lmdb数据集，再将数据集读入网络训练的全过程。这里的代码主要是学习和熟练应用caffe的训练，就以图片数据为例，学习如何制作lmdb数据集，以及训练调优网络。
    一，原始图片到lmdb数据集
    原始图片分为train和test文件，对应制作train.txt和test.txt，这一步需要自己编程，代码第一部分。经过上述代码处理，得到train和train.txt，同理可得test和test.txt。第二阶段制作lmdb，caffe中有相应脚本create.sh和convert.sh。最终得到train.mdb和lock.mdb。
    二，CNN-9Layers(caffe)
    和【构建CNN和RNN】中的各种神经网络不同之处：1，input层的参数不同，这里是data_param, 那里是hdf5_data_param；2，卷积层和池化层的参数不同.代码第二部分。

    
