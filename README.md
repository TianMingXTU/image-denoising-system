# image-denoising-system
image-denoising-system
在这里，我将使用一个常用的数据集CIFAR-10作为我们的训练和测试数据集。您需要安装torchvision库来获取CIFAR-10数据集。
现在，您可以使用--train选项训练自编码器模型，并使用CIFAR-10数据集。训练完成后，模型将保存为autoencoder_model.pth文件。之后，您可以使用这个预训练的模练好的模型对输入的图像进行去噪。以下是您可以尝试的一些命令行参数示例：
python main.py --method autoencoder --train
使用中值滤波去噪：python main.py --image input_image.png --method median
使用高斯滤波去噪：python main.py --image input_image.png --method gaussian
使用自编码器去噪：python main.py --image input_image.png --method autoencoder
项目已经添加了均值滤波和双边滤波方法，同时还优化了自编码器结构。这将有助于提高去噪效果。mean\bilateral
