# CODA

## model

* %dataset name%.yml:数据集配置

* %dataset name%_adv.yml:用于对抗训练和测试的数据集配置

## src/lib

* dataset
  * DataPrepare.py：为训练/测试准备训练/验证/测试列表 （把图片地址+" "+真值路径写入一个.txt文件）
  * shanghaitech/mall.py：数据集重定义 （数据增强等处理）
* network
  - cn.py:计数模型定义
  - dicriminator.py:鉴别器定义
* opt
     * train.py: 训练计数网络
     * train_adv.py: 对抗训练
     * lr_policy.py: lr policy 
* utils
     * image_opt.py: 图像可视化
     * Loger.py: tensorboard logger

