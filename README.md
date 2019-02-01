
ELMo预训练模型 文本分类
1、执行ELMo/elmo_main.py，训练情感分类模型（双向的LSTM+Attention）。

2、/ELMo/bilm/下是ELMo源码，在情感分类项目中调用源码中的函数，

3、/ELMo/modelParams/下是各种文件。
（1）elmo_options.json和elmo_weights.hdf5是elmo的模型的配置参数和已经预训练好的模型参数权重，从https://allennlp.org/elmo的Pre-trained ELMo Models 版块下下载Small规格的模型。
（2）elmo_token_embeddings.hdf5是调用elmo源码，微调elmo词向量，用到的文件：elmo_options.json、elmo_weights.hdf5、vocab.txt
（3）vocab.txt是词典文件，从训练样本中提取出来的。
