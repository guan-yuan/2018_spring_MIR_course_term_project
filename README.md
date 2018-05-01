# 2018 spring MIR course term project
此為MIR term project之repository, 如有要補充或新增的內容歡迎自行edit。Porject主要會有的分工項目有**1. 收集跟整理datasets**, **2. 音樂特徵處理或格式轉換**, **3.deep larning model設計跟程式撰寫**。盡量於每週二了解彼此該周進度，並共同擬定下週進度。  

## Memo:
#### ~~4/24:~~
``` 
分析與比較目前現有且公開的資料集。分類或回歸相關的tasks皆可，這個階段先放寬選擇，廣度優先。理想的datasets有下列兩種形式：  
1. For Multitask Training:
理想的datasets為large-scale且具有多種類型的資料標註(e.g. 情感分類, 調性分析...)。
2. For Domain Adversarial Training (Domain Adaptation):
理想為數個(至少兩個, 最好三個以上)不同domain的datasets，其具有相同的分類或回歸目標(e.g. 同為情感分類)。 

若datasets之資料標註有部份缺失或不足，我們也可以評估是否值得自行標註，或許可以一併拿到資料標註方面的分數。第一周先放寬選擇，建議可以先上完李宏毅transfer learning的影片再開始著手研究。Multitask Training與Domain Adversarial Training皆為可行的方向。
```

#### ~~5/01:~~
``` 
繼續datasets之整理(同上週)，並將datasets相關的Statistics(e.g. sizes, features, labels, 及相關descriptions)紀錄於"Dataset Statistics"。  

註: Dataset Statistics之紀錄格式可參考論文"FMA: A DATASET FOR MUSIC ANALYSIS"，或者有任何想法都歡迎提出。主要希望能了解該dataset提供哪些features, labels，以及較適合用於Multitask or Domain Adaptation，以便將來設計相關實驗。  
```
[Dataset Statistics](https://docs.google.com/spreadsheets/d/1BjONqtJ2Y_mOxV7hvBo4GrFjOgYHwnxiLCXZUS1XXqA/edit?usp=sharing)  
[FMA: A DATASET FOR MUSIC ANALYSIS](https://arxiv.org/pdf/1612.01840.pdf)

#### 5/08:
```  
針對Datasets(tasks)設計或者找出相關的models。Baseline或者自己設計的models都可以，並將相關的參數及實驗結果紀錄於"Models Statistics"。

繼續datasets之整理(同上週)，並將datasets相關的Statistics(e.g. sizes, features, labels, 及相關descriptions)紀錄於"Dataset Statistics"。可以盡量找與FMA相關(具有相關或相同的features或labels)的datasets。  
```
[Models Statistics](https://docs.google.com/spreadsheets/d/1Ny_7KXNcD0C547nvd-2EmmWnhEhZ-_mGjLmKRjUnz5Q/edit?usp=sharing)

註: 由於[FMA: A Dataset For Music Analysis, ISMIR 2017](https://github.com/mdeff/fma)的品質跟資料數量皆相當不錯，較適合與其他dataset做Domain Adversarial Training，且提供相當豐富的features，建議可以先run看看其提供的相關工具及baseline models(附於dataset之github中)。

[FMA Baselines](https://nbviewer.jupyter.org/github/mdeff/fma/blob/outputs/baselines.ipynb#Baselines) 
![test image size](https://github.com/guan-yuan/2018_spring_MIR_course_term_project/blob/master/imgs/fma_baselines.PNG){:height="50%" width="50%"}   

#### 6/19:
```
Term Project Presentation (Order:17th)
(10min Presentataion + 3min Q&A)
```

#### 6/26:
```
Term Paper Deadline
(Including Members' Contribution)
```
## Google Docs:
- [Dataset Statistics (for datasets descriptions)](https://docs.google.com/spreadsheets/d/1BjONqtJ2Y_mOxV7hvBo4GrFjOgYHwnxiLCXZUS1XXqA/edit?usp=sharing)

- [Models Statistics (紀錄models之架構、超參數以及實驗結果)](https://docs.google.com/spreadsheets/d/1Ny_7KXNcD0C547nvd-2EmmWnhEhZ-_mGjLmKRjUnz5Q/edit?usp=sharing)

## Ideal Target:
經過兩個多月的努力，相關研究成果如果能投上國際甚至是頂級的Conferences，當然是最理想的。相關投稿與研究經驗，應該也能對之後的碩士論文及自己的研究有所幫助。以下為deadline與期末較為相近的Top Conferences:
```
AAAI 2019, 
Deadline: September 5, 2018
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

- [Multi-label Music Genre Classification from Audio, Text, and Images Using Deep Features, ISMIR 2017 (如其名，使用多種特徵做多類別分類using MuMu dataset)](https://arxiv.org/abs/1707.04916)

- [FMA: A Dataset For Music Analysis, ISMIR 2017 (FMA dataset的論文)](https://arxiv.org/abs/1612.01840)


## Codes:
- [迁移学习 Transfer Learning 代碼全集](https://github.com/jindongwang/transferlearning/tree/master/code)

- [Transfer learning for music classification and regression tasks 原作代碼](https://github.com/keunwoochoi/transfer_learning_music)

- [Deep Learning for audio and text (Tartarus is a python module for Deep Learning experiments on Audio and Text and their combination)](https://github.com/sergiooramas/tartarus)

## Datasets:
- [ISMIR Resources](http://www.ismir.net/resources.html#datasets)

- ~~[Nottingham Music Database: over 1000 folk tunes](http://abc.sourceforge.net/NMD/)~~

- ~~[Cleaned version of the Nottingham dataset (with MIDI conversion)](https://github.com/jukedeck/nottingham-dataset)~~

- ~~[Piano-midi.de: classical piano pieces](http://www.piano-midi.de/)~~

- [Kaggle上關於Music的datasets](https://www.kaggle.com/datasets?sortBy=hottest&group=public&page=1&pageSize=20&size=all&filetype=all&license=all&tagids=2304)

- [FMA: A Dataset For Music Analysis, ISMIR 2017](https://github.com/mdeff/fma)

- [Million Song Dataset](https://labrosa.ee.columbia.edu/millionsong/)

- [Million Song Dataset Benchmarks](http://www.ifs.tuwien.ac.at/mir/msd/)

- [MIR-1K Dataset](https://sites.google.com/site/unvoicedsoundseparation/mir-1k)

- [Multi Media Eval](http://www.multimediaeval.org/datasets/)

- [MuMu (a Multimodal Music dataset with multi-label genre annotations)](https://www.upf.edu/en/web/mtg/mumu)

- [OHHLA Lyrics](https://raw.githubusercontent.com/brannondorsey/ml4music-workshop/master/data/lyrics/data/ohhla_lyrics/input.txt)

- [SALAMI Dataset](https://github.com/DDMAL/salami-data-public)


-----from AWT_2015_Tutorial-----

#### Polyphonic datasets – chords/isolated notes

- [UIOWA Musical Instrument Samples](http://theremin.music.uiowa.edu/MIS.html)
- [RWC Musical Instrument Sounds](https://staff.aist.go.jp/m.goto/RWC-MDB/rwc-mdb-i.html)
- [McGill University Master Samples]
- [MAPS samples](http://www.tsi.telecom-paristech.fr/aao/)

#### Polyphonic datasets – music pieces

- [RWC database - classical subset](https://staff.aist.go.jp/m.goto/RWC-MDB/rwc-mdb-c.html)
- [RWC database – jazz subset](https://staff.aist.go.jp/m.goto/RWC-MDB/rwc-mdb-j.html)
- [MAPS database](http://www.tsi.telecom-paristech.fr/aao/)
- [TRIOS dataset](http://c4dm.eecs.qmul.ac.uk/rdr/handle/123456789/27)
- [LabROSA Automatic Piano Transcription dataset](http://labrosa.ee.columbia.edu/projects/piano/)
- [Bach10 dataset](http://www.ece.rochester.edu/~zduan/resource/Resources.html)
- [MIREX multiF0 development dataset](http://www.music-ir.org/evaluation/MIREX/data/2007/multiF0/index.htm)
- [Score-informed piano transcription dataset](http://c4dm.eecs.qmul.ac.uk/rdr/handle/123456789/13)

#### Melody/baseline datasets

- [RWC database –popular/royalty-free/genre subsets](https://staff.aist.go.jp/m.goto/RWC-MDB/)

#### Percussive transcription datasets

- [ENST-Drums](http://www.tsi.telecom-paristech.fr/aao/en/software-and-database/)
- [200 Drum Machines](http://colinraffel.com/datasets/200DrumMachines.tar.gz)
- [DREANSS dataset](http://mtg.upf.edu/download/datasets/dreanss)
- [IDMT-SMT-Drums](http://www.idmt.fraunhofer.de/en/business_units/smt/drums.html)

#### Additional datasets

- [KSN database](http://hil.t.u-tokyo.ac.jp/software/KSN/)
- [AIST RWC annotations](https://staff.aist.go.jp/m.goto/RWC-MDB/AIST-Annotation/)

