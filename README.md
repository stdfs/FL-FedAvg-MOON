# 基于对比学习的联邦学习算法研究
联邦学习是一种分布式机器学习技术，可以在保护数据隐私的前提下实现多方协同建模。然而联邦学习依然面临着数据异构性问题。在这种数据分布下，联邦学习的模型性能明显下降，成为了限制联邦学习实际应用的关键原因。国内外研究人员针对联邦学习遇到的各种困难都进行了进一步的改进。本文研究的MOON算法（Model-Contrastive Federated Learning）是一种面向数据异构的联邦学习算法，它通过在联邦学习中引入对比学习机制，最大化当前本地模型与全局模型特征表示的相似性，减小本地模型与前一次模型特征表示的相似性，约束模型的训练方向，从而提高模型性能。本研究通过系统的实验对比了MOON算法与传统的FedAvg算法，使用CIFAR-10和MNIST数据集，通过调整数据分布情况来评估两种算法的模型性能，最终的实验结果表明，MOON算法在不同数据分布情况下的性能均优于传统的FedAvg算法。

Federated learning is a distributed machine learning technique that enables collaborative modeling among multiple parties while preserving data privacy, yet it still faces the critical challenge of data heterogeneity that significantly deteriorates model performance and limits practical applications. Researchers worldwide have proposed various improvements to address these federated learning challenges, with this study focusing on the data-heterogeneity-oriented MOON algorithm (Model-Contrastive Federated Learning) which introduces a contrastive learning mechanism to maximize feature representation similarity between current local and global models while minimizing similarity between local and previous models, thereby constraining training direction and enhancing performance. Through systematic experiments comparing MOON with traditional FedAvg on CIFAR-10 and MNIST datasets under varied data distributions, the results demonstrate MOON's consistent superiority over FedAvg across all scenarios.


### CIFAR-10数据集实验

实验代码：https://www.kaggle.com/code/qmzqbt66/cifar-10


### MNIST数据集试验

实验代码：https://www.kaggle.com/code/qmzqbt66/mnist

### 额外的本地画图代码

代码上传文件名FL.ipynb
