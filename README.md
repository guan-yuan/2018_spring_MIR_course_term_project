# 2018 spring MIR course term project
此為MIR term project之repository, 如有要補充或新增的內容歡迎自行edit。Porject主要會有的分工項目有**1. 收集跟整理datasets**, **2. 音樂特徵處理或格式轉換**, **3.deep larning model設計跟程式撰寫**。盡量於每週二了解彼此該周進度，並共同擬定下週進度。  

## Memo:
#### 4/24:
``` 
分析與比較目前現有且公開的資料集。分類或回歸相關的tasks皆可，這個階段先放寬選擇，廣度優先。理想的datasets有下列兩種形式：  
1. For Multitask Training:
理想的datasets為large-scale且具有多種類型的資料標註(e.g. 情感分類, 調性分析...)。
2. For Domain Adversarial Training (Domain Adaptation):
理想為數個(至少兩個, 最好三個以上)不同domain的datasets，其具有相同的分類或回歸目標(e.g. 同為情感分類)。 

若datasets之資料標註有部份缺失或不足，我們也可以評估是否值得自行標註，或許可以一併拿到資料標註方面的分數。第一周先放寬選擇，建議可以先上完李宏毅transfer learning的影片再開始著手研究。Multitask Training與Domain Adversarial Training皆為可行的方向。
```

#### 6/19:
```
Term Project Presentation
```


## Ideal Target:
經過兩個多月的努力，相關研究成果如果能投上國際甚至是頂級的Conferences，當然是最理想的。相關投稿與研究經驗，應該也能對之後的碩士論文及自己的研究有所幫助。以下為deadline與期末較為相近的Top Conferences:
```
AAAI 2019, about September
```

## Tutorials:
- [李宏毅 ML Lecture 19 Transfer Learning (優先)](https://www.youtube.com/watch?v=qD6iD4TFsdQ)

- [PyTorch Tutorials (推薦)](http://pytorch.org/tutorials/)

- [MMD: maximum mean discrepancy (Domain Adaptation 常用的數學理論)](https://blog.csdn.net/a1154761720/article/details/51516273)


## Papers:
- [A Tutorial on Deep Learning for Music Information Retrieval (拉高發deep learning for music論文門檻的論文)](https://arxiv.org/abs/1709.04396)

- [Learning Transferable Features with Deep Adaptation Networks (經典domain adaptation相關論文)](https://arxiv.org/abs/1502.02791)

- [Transfer learning for music classification and regression tasks, ISMIR 2017 (Transfer learning for music的重要論文)](https://arxiv.org/abs/1703.09179)

- [A Kernel Method for the Two-Sample-Problem (MMD原始論文)](http://www.cyberneum.de/fileadmin/user_upload/files/publications/NIPS2006_0583_4193%5B0%5D.pdf)

- [Optimal kernel choice for large-scale two-sample tests (多核MMD論文，含Linear Time近似解推導)](https://papers.nips.cc/paper/4727-optimal-kernel-choice-for-large-scale-two-sample-tests)

- [Multi-label Music Genre Classification from Audio, Text, and Images Using Deep Features, ISMIR 2017 (如其名使用多種特徵做多類別分類, using MuMu dataset)](https://arxiv.org/abs/1707.04916)


## Codes:
- [迁移学习 Transfer Learning 代碼全集](https://github.com/jindongwang/transferlearning/tree/master/code)

- [Transfer learning for music classification and regression tasks 原作代碼](https://github.com/keunwoochoi/transfer_learning_music)

- [Deep Learning for audio and text (Tartarus is a python module for Deep Learning experiments on Audio and Text and their combination)](https://github.com/sergiooramas/tartarus)

## Datasets:
- [ISMIR Resources](http://www.ismir.net/resources.html#datasets)

- [Nottingham Music Database: over 1000 folk tunes](http://abc.sourceforge.net/NMD/)

- [Cleaned version of the Nottingham dataset (with MIDI conversion)](https://github.com/jukedeck/nottingham-dataset)

- [Piano-midi.de: classical piano pieces](http://www.piano-midi.de/)

- [Kaggle上關於Music的datasets](https://www.kaggle.com/datasets?sortBy=hottest&group=public&page=1&pageSize=20&size=all&filetype=all&license=all&tagids=2304)

- [FMA: A Dataset For Music Analysis, ISMIR 2017](https://github.com/mdeff/fma)

- [Million Song Dataset](https://labrosa.ee.columbia.edu/millionsong/)

- [MIR-1K Dataset](https://sites.google.com/site/unvoicedsoundseparation/mir-1k)

- [Multi Media Eval](http://www.multimediaeval.org/datasets/)

- [MuMu (a Multimodal Music dataset with multi-label genre annotations)](https://www.upf.edu/en/web/mtg/mumu)
