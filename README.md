# GTSRB-Recognition
## 项目介绍
* data 目录中是数据集，来自[德国波鸿鲁尔大学的神经信息学研究所](https://benchmark.ini.rub.de/gtsrb_dataset.html)
* models 目录中是保存的模型文件
    * `GTSRBNet.pth`是训练好的最终模型
    * `LeNet.pth`是用于对比的基线模型
    * `GTSRBNet_no_sampler.pth`是过采样消融实验得到的模型
    * `GTSRBNet_no_dropout.pth`是 Dropout 消融实验得到的模型
* main.ipynb 是本实验的全部代码，可以直接运行，暂时将所有保存模型的语句注释掉了，可以通过搜索`torch.save`找到
* requirements.txt 是 python 环境中的包列表
* main.html 是将 Jupyter Notebook 导出为 html 文件的结果