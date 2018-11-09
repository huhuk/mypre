Finacial News Sentiment Classification with Embedding and SVM

@author: huhu

---

# 舆情分析

- 文本向量化
- 分类模型

---

## 文本向量化

- 预处理
- 分词
- 向量化

~~

### 预处理

```python
def pre_process(s):
    s = str(s)
    s = re.sub('&nbsp;', '', s)
    s = re.sub('\\u3000', '', s)
    s = re.sub('<.*?>', '', s)
    return s
```
~~

### 分词

- jieba
- thulac
- 哈工大LTP

~~

### 向量化

- tfidf
- embedding
    + 迁移学习
        * Corpus: Financial News 金融新闻
        * Context Features: Word
        * Skip-Gram with Negative Sampling (SGNS)
    + 等权重/tfidf权重

---

## 分类模型

- 罗杰斯特回归
- 随机森林
- XGBoost
- SVM
- RNN

~~ 

### SVM

- rbf kernel
- grid search
  + c, gamma

~~ 

### RNN

---

# END
