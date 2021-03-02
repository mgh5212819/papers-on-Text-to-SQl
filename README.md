# papers-on-Text-to-SQl
记录实习时的相关研究工作，并分别提交到ACL2021、ACL2019和EMNLP2019。



### Structure-Aware Multi-hop Attention for Document-Level Relation Extraction（sumbit to ACL2021）

文档级关系抽取旨在识别文档中实体之间的语义关系。为了捕捉句间实体之间的复杂交互，图卷积网络被广泛应用于这一任务，并取得了优异的性能。然而，基于GCN的关系抽取方法存在过度平滑和错误传播的问题，尤其是在大规模复杂文档图中。针对上述缺陷，本文提出了一种构造结构感知多跳注意力(SAMA)图神经网络的新模型。文档图通过注意力扩散执行多跳注意力计算。此外，我们利用实体节点的拓扑性质自适应地调整注意力分布。实验结果表明，我们的模型在公共数据集上取得了很好的效果，在中文金融数据集上也取得了显著的改进。此外，大量的分析表明，我们的模型可以处理上述缺陷，并在大规模复杂文档图上做更好的推理。





### Transition-based Graph Generation For Text-to-SQL Task 文本生成SQL（sumbit to ACL2019）

在本文中，我们提出了一种基于transition的神经语义解析方法来将自然语言问题映射到SQL查询。我们将SQL查询表示为一个语义图，其中知识库中的语义单元作为节点，SQL语言的关键字和运算符作为边。然后利用transition方法和Seq2Seq模型，将文本到SQL的生成过程转化为序列到图的过程，这样可以同时利用语义图表示的优点和Seq2Seq模型强大的预测能力。另外，为了提高问题与知识库匹配图节点的生成，提出了一种利用知识库的多层次粒度和语义结构的匹配网络。在wikiSQL数据集上的实验结果表明，尽管使用了相对简单的解码器，但我们的方法始终能够提高性能，取得具有竞争力的结果

详细讲解：https://blog.csdn.net/qq_38556984/article/details/107544682



### Syntax- and Execution-Aware SQL Generation with Reinforcement Learning （submit to EMNLP2019）

文本到SQL任务的目的是将自然语言语句映射为结构化的SQL查询。本文在考虑知识库结构和SQL查询语法的基础上，设计了一种新的评分方法来评价生成的SQL查询。为了改进SQL查询的生成，我们在序列到序列模型中使用这个分数作为强化目标。在wikiSQL数据集上的实验结果表明，我们提出的方法在所有指标上都显著提高了性能。新的分数优于现有系统中与强化学习一起使用的其他奖励，并且与通过与知识库交互来解码的执行是可比的。

详细讲解：https://blog.csdn.net/qq_38556984/article/details/107643043
