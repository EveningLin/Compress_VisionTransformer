# Compress_VisionTransformer

参照BERT-of-Theseus对vit进行压缩
训练步骤：
（1）本地（微调）数据集对教师模型进行训练
（2）开始压缩

"""
python train.py 
[训练参数参照文档 https://huggingface.co/docs/timm/training_script]
[
压缩参数：
--replacing_rate 0.3 
--scheduler linear 
--scheduler_linear_k 0.0006
]
"""
我用的是ImageNet10k进行尝试，时间有点久，成本有点大
