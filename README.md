## 项目描述
NLP 领域常见任务的实现，包括新词发现, 以及基于pytorch的词向量、中文文本分类、实体识别、文本生成等。 

## 依赖
```
python 3.7
pytorch 1.8.0
torchtext 0.9.1
optuna 2.6.0
transformers 3.0.2
```

## 目录

### 0. 新词发现算法

- 0-1. [New Words Discovery](0-1.WordsDiscovery)

### 1. 词向量

- 1-1. [Word2Vec(Skip-gram)](1-1.Word2Vec)
- 1-2. [Glove](1-2.Glove)

### 2. 文本分类 (每个模型内部使用[optuna](https://optuna.org/)进行调参)

- 2-1. [TextCNN](2-1.TextCNN)
- 2-2. [FastText](2-2.FastText)
- 2-3. [TextRCNN](2-3.TextRCNN)
- 2-4. [TextRNN_Att](2-4.TextRNN_Att)
- 2-5. [DPCNN](2-5.DPCNN)
- 2-6. [XGBoost](2-6.XGboost)
- 2-7. [Distill_& fine tune Bert](2-7.Distill_finetune_Bert)
- 2-8. [Pattern-Exploiting-Training 利用MLM做文本分类](2-8.Pattern-Exploiting-Training)
- 2-9. [R-Drop](2-9.R-drop)
 
数据集(data文件夹)： 二分类舆情数据集，划分如下：

数据集|数据量
--|--
训练集|56700
验证集|7000
测试集|6300

### 3. 实体识别NER 

- 3-1. [BILSTM_CRF_NER](3-1.BiLSTM_CRF)
- 3-2. [Lattice_LSTM](3-2.Lattice_LSTM)
- 3-3. [Bert_CRF](3-3.Bert_CRF)

### 4. 文本摘要生成

#### 1). 生成式
- 4-1. [Seq2seq 模型](4-1.Seq2seq)
- 4-2. [Seq2seq 模型+注意力机制](4-2.Seq2seq_Att)
- 4-3. [Transformer 模型](4-3.Transformer)
- 4-4. [GPT 摘要生成](4-4.GPT)
- 4-5. [Bert-seq2seq](4-5.Bert-seq2seq)
#### 2). 抽取式
- 4-6. [Bert-extractive-summarizer](4-6.Bert-extractive-summarizer)

### 5. [PaperwithCode](5.PaperwithCode)

该文件夹记录一些paper及其所对应的模型代码:
- 5.1. [Co-Interactive-Transformer](https://github.com/jasoncao11/nlp-notebook/tree/master/5.PaperwithCode/1.Co-Interactive-Transformer)
- 5.2. [DSSM](https://github.com/jasoncao11/nlp-notebook/tree/master/5.PaperwithCode/2.DSSM)
- 5.3. [P-tuning](https://github.com/jasoncao11/nlp-notebook/tree/master/5.PaperwithCode/3.P-tuning)

### 6. [QA](QA)

该文件夹内记录机器学习/深度学习一些知识点的简单总结。

### 7. [algo](algo)

该文件夹内记录leetcode最热门的100道算法题，部分解题思路搬运自leetcode题解。
