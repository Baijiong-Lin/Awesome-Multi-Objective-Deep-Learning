# Awesome-Multi-Objective-Deep-Learning

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

:star: This repository hosts a curated collection of literature associated with **gradient-based multi-objective algorithms** in deep learning. Feel free to star and fork. For further details, refer to the following paper:

**[Gradient-Based Multi-Objective Deep Learning: Algorithms, Theories, Applications, and Beyond](https://arxiv.org/)**<br/>
[Weiyu Chen](https://weiyuchen.cc/)<sup>1,\*</sup>, [Xiaoyuan Zhang](https://xzhang2523.github.io/)<sup>2,\*</sup>, [Baijiong Lin](https://baijiong-lin.github.io/)<sup>3,\*</sup>, [Xi Lin](https://xi-l.github.io/)<sup>2</sup>, [Han Zhao](https://hanzhaoml.github.io/)<sup>4</sup>, [Qingfu Zhang](https://scholar.google.com/citations?user=nhL9PHwAAAAJ&hl=en)<sup>2</sup>, and [James T. Kwok](https://cse.hkust.edu.hk/~jamesk/)<sup>1</sup><br/>
<sup>1</sup>HKUST, <sup>2</sup>CityU, <sup>3</sup>HKUST(GZ), <sup>4</sup>UIUC, \*Equal Contribution
<br/>

If you find this repository is useful for you, please cite our paper:
```
@article{2025modl,
      title={Gradient-Based Multi-Objective Deep Learning: Algorithms, Theories, Applications, and Beyond}, 
      author={Weiyu Chen and Xiaoyuan Zhang and Baijiong Lin and Xi Lin and Han Zhao and Qingfu Zhang and James T. Kwok},
      year={2025},
}
```

## Contents
- [Related Survey](#related-survey)
- [Finding a Single Pareto Optimal Solution](#finding-a-single-pareto-optimal-solution)
  - [Loss Balancing Methods](#loss-balancing-methods)
  - [Gradient Balancing Methods](#gradient-balancing-methods)
    - [Gradient Weighting Methods](#gradient-weighting-methods)
    - [Gradient Manipulation Methods](#gradient-manipulation-methods)
- [Resources](#resources)
  - [Software](#software)

## Related Survey

1. **Multi-task learning with deep neural networks: A survey** [[Paper](https://arxiv.org/abs/2009.09796)]    
   *Michael Crawshaw*  
   arXiv:2009.09796, 2020.

2. **A Survey on Multi-Task Learning** [[Paper](https://ieeexplore.ieee.org/document/9392366/)]   
   *Yu Zhang and Qiang Yang*   
   IEEE Transactions on Knowledge and Data Engineering (**TKDE**), 2021.  

3. **A Review on Evolutionary Multi-Task Optimization: Trends and Challenges** [[Paper](https://ieeexplore.ieee.org/document/9665768)]  
   *Tingyang Wei, Shibin Wang, Jinghui Zhong, Dong Liu, and Jun Zhang*  
   IEEE Transactions on Evolutionary Computation (**TEVC**), 2021.  

4. **Multi-Task Learning for Dense Prediction Tasks: A Survey** [[Paper](https://ieeexplore.ieee.org/document/9336293)]  
   *Simon Vandenhende, Stamatios Georgoulis, Wouter Van Gansbeke, Marc Proesmans, Dengxin Dai, and Luc Van Gool*  
   IEEE Transactions on Pattern Analysis and Machine Intelligence (**TPAMI**), 2021.  

5. **Twenty years of continuous multiobjective optimization in the twenty-first century** [[Paper](https://www.sciencedirect.com/science/article/pii/S2192440621001416)]  
   *Gabriele Eichfelder*  
   **EURO Journal on Computational Optimization**, 2021.  

6. **Advances and Challenges of Multi-task Learning Method in Recommender System: A Survey** [[Paper](https://arxiv.org/abs/2305.13843)]  
   *Mingzhu Zhang, Ruiping Yin, Zhen Yang, Yipeng Wang, and Kan Li*  
   arXiv:2305.13843, 2023.  

7. **Unleashing the Power of Multi-Task Learning: A Comprehensive Survey Spanning Traditional, Deep, and Pretrained Foundation Model Eras** [[Paper](https://arxiv.org/abs/2404.18961)]  
   *Jun Yu, Yutong Dai, Xiaokang Liu, Jin Huang, Yishan Shen, Ke Zhang, Rong Zhou, Eashan Adhikarla, Wenxuan Ye, Yixin Liu, Zhaoming Kong, Kai Zhang, Yilong Yin, Vinod Namboodiri, Brian D. Davison, Jason H. Moore, and Yong Chen*  
   arXiv:2404.18961, 2024.  

8. **Multi-Task Learning in Natural Language Processing: An Overview** [[Paper](https://dl.acm.org/doi/10.1145/3663363)]  
   *Shijie Chen, Yu Zhang, and Qiang Yang*  
   ACM Computing Surveys (**CSUR**), 2024.

## Finding a Single Pareto Optimal Solution
### Loss Balancing Methods

1. **Multi-Task Learning Using Uncertainty to Weigh Losses for Scene Geometry and Semantics** [[Paper](https://openaccess.thecvf.com/content_cvpr_2018/papers/Kendall_Multi-Task_Learning_Using_CVPR_2018_paper.pdf)]  
   *Alex Kendall, Yarin Gal, and Roberto Cipolla*  
   **CVPR**, 2018.
   
2. **End-To-End Multi-Task Learning With Attention** [[Paper](https://openaccess.thecvf.com/content_CVPR_2019/papers/Liu_End-To-End_Multi-Task_Learning_With_Attention_CVPR_2019_paper.pdf)]  
   *Shikun Liu, Edward Johns, and Andrew J. Davison*  
   **CVPR**, 2019.  

3. **Multi-Objective Meta Learning** [[Paper](https://openreview.net/pdf?id=wKf9iSu_TEm)] [[Code](https://github.com/Baijiong-Lin/MOML)]  
   *Feiyang Ye, Baijiong Lin, Zhixiong Yue, Pengxin Guo, Qiao Xiao, and Yu Zhang*  
   **NeurIPS**, 2021

4. **Towards Impartial Multi-task Learning** [[Paper](https://openreview.net/forum?id=IMPnRXEWpvr)]  
   *Liyang Liu, Yi Li, Zhanghui Kuang, Jing-Hao Xue, Yimin Chen, Wenming Yang, Qingmin Liao, and Wayne Zhang*  
   **ICLR**, 2021.

5. **Reasonable Effectiveness of Random Weighting: A Litmus Test for Multi-Task Learning** [[Paper](https://openreview.net/forum?id=jjtFD8A1Wx)]  
   *Baijiong Lin, Feiyang Ye, Yu Zhang, and Ivor W. Tsang*  
   Transactions on Machine Learning Research (**TMLR**), 2022.

6. **Auto-Lambda: Disentangling Dynamic Task Relationships** [[Paper](https://openreview.net/forum?id=KKeCMim5VN)] [[Code](https://github.com/lorenmt/auto-lambda)]  
   *Shikun Liu, Stephen James, Andrew Davison, Edward Johns*  
   Transactions on Machine Learning Research (**TMLR**), 2022.

7. **Dual-Balancing for Multi-Task Learning** [[Paper](https://arxiv.org/abs/2308.12029)]  
   *Baijiong Lin, Weisen Jiang, Feiyang Ye, Yu Zhang, Pengguang Chen, Ying-Cong Chen, Shu Liu, and James T. Kwok*  
   arXiv:2308.12029, 2023.

8. **A First-Order Multi-Gradient Algorithm for Multi-Objective Bi-Level Optimization** [[Paper](https://ebooks.iospress.nl/doi/10.3233/FAIA240793)] [[Code](https://github.com/Baijiong-Lin/FORUM)]    
   *Feiyang Ye, Baijiong Lin, Xiaofeng Cao, Yu Zhang, and Ivor W. Tsang*  
   **ECAI**, 2024.

9. **Smooth Tchebycheff Scalarization for Multi-Objective Optimization** [[Paper](https://openreview.net/forum?id=m4dO5L6eCp)]  
   *Xi Lin, Xiaoyuan Zhang, Zhiyuan Yang, Fei Liu, Zhenkun Wang, and Qingfu Zhang*  
   **ICML**, 2024.

10. **Multi-Objective Meta-Learning** [[Paper](https://doi.org/10.1016/j.artint.2024.104184)]  
   *Feiyang Ye, Baijiong Lin, Zhixiong Yue, Yu Zhang, and Ivor W. Tsang*   
   Artificial Intelligence (**AIJ**), 2024. 

### Gradient Balancing Methods
#### Gradient Weighting Methods

1. **GradNorm: Gradient Normalization for Adaptive Loss Balancing in Deep Multitask Networks** [[Paper](http://proceedings.mlr.press/v80/chen18a/chen18a.pdf)]  
   *Zhao Chen, Vijay Badrinarayanan, Chen-Yu Lee, and Andrew Rabinovich*  
   **ICML**, 2018.

2. **Multi-Task Learning as Multi-Objective Optimization** [[Paper](https://papers.nips.cc/paper/2018/hash/432aca3a1e345e339f35a30c8f65edce-Abstract.html)] [[Code](https://github.com/isl-org/MultiObjectiveOptimization)]  
   *Ozan Sener, and Vladlen Koltun*  
   **NeurIPS**, 2018

3. **Towards Impartial Multi-task Learning** [[Paper](https://openreview.net/forum?id=IMPnRXEWpvr)]  
   *Liyang Liu, Yi Li, Zhanghui Kuang, Jing-Hao Xue, Yimin Chen, Wenming Yang, Qingmin Liao, and Wayne Zhang*  
   **ICLR**, 2021.

4. **Conflict-Averse Gradient Descent for Multi-task Learning** [[Paper](https://openreview.net/forum?id=_61Qh8tULj_)] [[Code](https://github.com/Cranial-XIX/CAGrad)]  
   *Bo Liu, Xingchao Liu, Xiaojie Jin, Peter Stone, and Qiang Liu*  
   **NeurIPS**, 2021

5. **Multi-Task Learning as a Bargaining Game** [[Paper](https://proceedings.mlr.press/v162/navon22a/navon22a.pdf)] [[Code](https://github.com/AvivNavon/nash-mtl)]  
   *Aviv Navon, Aviv Shamsian, Idan Achituve, Haggai Maron, Kenji Kawaguchi, Gal Chechik, and Ethan Fetaya*  
   **ICML**, 2022.

6. **Mitigating Gradient Bias in Multi-objective Learning: A Provably Convergent Approach** [[Paper](https://openreview.net/forum?id=dLAYGdKTi2)]  
   *Heshan Devaka Fernando, Han Shen, Miao Liu, Subhajit Chaudhury, Keerthiram Murugesan, and Tianyi Chen*  
   **ICLR**, 2023.

7. **Independent Component Alignment for Multi-Task Learning** [[Paper](https://openaccess.thecvf.com/content/CVPR2023/html/Senushkin_Independent_Component_Alignment_for_Multi-Task_Learning_CVPR_2023_paper.html)] [[Code](https://github.com/SamsungLabs/MTL)]  
   *Dmitry Senushkin, Nikolay Patakin, Arseny Kuznetsov, and Anton Konushin*  
   **CVPR**, 2023.

8. **FAMO: Fast Adaptive Multitask Optimization** [[Paper](https://papers.nips.cc/paper_files/paper/2023/hash/b2fe1ee8d936ac08dd26f2ff58986c8f-Abstract-Conference.html)]  
   *Bo Liu, Yihao Feng, Peter Stone, and Qiang Liu*  
   **NeurIPS**, 2023.

9. **Direction-oriented Multi-objective Learning: Simple and Provable Stochastic Algorithms** [[Paper](https://openreview.net/forum?id=4Ks8RPcXd9)] [[Code](https://github.com/OptMN-Lab/sdmgrad)]  
   *Peiyao Xiao, Hao Ban, Kaiyi Ji*  
   **NeurIPS**, 2023.

10. **Dual-Balancing for Multi-Task Learning** [[Paper](https://arxiv.org/abs/2308.12029)]  
    *Baijiong Lin, Weisen Jiang, Feiyang Ye, Yu Zhang, Pengguang Chen, Ying-Cong Chen, Shu Liu, and James T. Kwok*  
    arXiv:2308.12029, 2023.

11. **Fair Resource Allocation in Multi-Task Learning** [[Paper](https://openreview.net/forum?id=KLmWRMg6nL)] [[Code](https://github.com/OptMN-Lab/fairgrad)]  
   *Hao Ban and Kaiyi Ji*  
   **ICML**, 2024.

#### Gradient Manipulation Methods

1. **Just Pick a Sign: Optimizing Deep Multitask Models with Gradient Sign Dropout** [[Paper](https://papers.nips.cc/paper/2020/hash/16002f7a455a94aa4e91cc34ebdb9f2d-Abstract.html)] [[Code](https://github.com/tensorflow/lingvo/blob/master/lingvo/core/graddrop.py)]  
   *Zhao Chen, Jiquan Ngiam, Yanping Huang, Thang Luong, Henrik Kretzschmar, Yuning Chai, and Dragomir Anguelov*  
   **NeurIPS**, 2020

2. **Gradient Surgery for Multi-Task Learning** [[Paper](https://papers.nips.cc/paper/2020/hash/3fe78a8acf5fda99de95303940a2420c-Abstract.html)] [[Code](https://github.com/tianheyu927/PCGrad)]  
   *Tianhe Yu, Saurabh Kumar, Abhishek Gupta, Sergey Levine, Karol Hausman, and Chelsea Finn*  
   **NeurIPS**, 2020

3. **Gradient Vaccine: Investigating and Improving Multi-task Optimization in Massively Multilingual Models** [[Paper](https://openreview.net/forum?id=F1vEjWK-lH_)]    
   *Zirui Wang, Yulia Tsvetkov, Orhan Firat, and Yuan Cao*  
   **ICLR**, 2021

## Resources
### Software
1. **LibMTL: A PyTorch Library for Multi-Task Learning** [[Paper](https://jmlr.org/papers/v24/22-0347.html)] [[Code](https://github.com/median-research-group/LibMTL)]    
   *Baijiong Lin and Yu Zhang*  
   Journal of Machine Learning Research (**JMLR**), 2023
   
2. **LibMOON: A Gradient-based MultiObjective OptimizatioN Library in PyTorch** [[Paper](https://openreview.net/forum?id=etdXLAMZoc)] [[Code](https://github.com/xzhang2523/libmoon)]  
   *Xiaoyuan Zhang, Liang Zhao, Yingying Yu, Xi Lin, Zhenkun Wang, Han Zhao, and Qingfu Zhang*  
   **NeurIPS** Datasets and Benchmarks Track, 2024       
