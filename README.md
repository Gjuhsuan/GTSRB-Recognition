# GTSRB-Recognition
## 项目介绍
* data 目录用于存放数据集，如果要复现，将以下三个文件下载并解压到 data 目录下即可，来自[德国波鸿鲁尔大学的神经信息学研究所](https://benchmark.ini.rub.de/gtsrb_dataset.html)
    * [训练集](https://sid.erda.dk/public/archives/daaeac0d7ce1152aea9b61d9f1e19370/GTSRB_Final_Training_Images.zip)
    * [测试集图片](https://sid.erda.dk/public/archives/daaeac0d7ce1152aea9b61d9f1e19370/GTSRB_Final_Test_Images.zip)
    * [测试集标签](https://sid.erda.dk/public/archives/daaeac0d7ce1152aea9b61d9f1e19370/GTSRB_Final_Test_GT.zip)
* models 目录中是保存的模型文件
    * `GTSRBNet.pth`是训练好的最终模型
    * `LeNet.pth`是用于对比的基线模型
    * `GTSRBNet_no_sampler.pth`是过采样消融实验得到的模型
    * `GTSRBNet_no_dropout.pth`是 Dropout 消融实验得到的模型
* main.ipynb 是本实验的全部代码，可以直接运行，暂时将所有保存模型的语句注释掉了，可以通过搜索`torch.save`找到
* requirements.txt 是 python 环境中的包列表
* main.html 是将 Jupyter Notebook 导出为 html 文件的结果