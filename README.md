# Awesome-Multi-Objective-Deep-Learning

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![paper](https://img.shields.io/badge/arXiv-2501.10945-b31b1b.svg)](https://arxiv.org/abs/2501.10945)
[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FBaijiong-Lin%2FAwesome-Multi-Objective-Deep-Learning&count_bg=%2379C83D&title_bg=%23555555&icon=baidu.svg&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)
[![Made With Love](https://img.shields.io/badge/Made%20With-Love-orange.svg)](https://github.com/Baijiong-Lin/Awesome-Multi-Objective-Deep-Learning) 

:star: This repository hosts a curated collection of literature associated with **gradient-based multi-objective algorithms** in deep learning. Feel free to star and fork. For further details, refer to the following paper:

**[Gradient-Based Multi-Objective Deep Learning: Algorithms, Theories, Applications, and Beyond](https://arxiv.org/abs/2501.10945)**<br/>
[Weiyu Chen](https://weiyuchen.cc/)<sup><b>1,\*</b></sup>, [Xiaoyuan Zhang](https://xzhang2523.github.io/)<sup><b>2,\*</b></sup>, [Baijiong Lin](https://baijiong-lin.github.io/)<sup><b>3,\*</b></sup>, [Xi Lin](https://xi-l.github.io/)<sup><b>2</b></sup>, [Han Zhao](https://hanzhaoml.github.io/)<sup><b>4</b></sup>, [Qingfu Zhang](https://scholar.google.com/citations?user=nhL9PHwAAAAJ&hl=en)<sup><b>2</b></sup>, and [James T. Kwok](https://cse.hkust.edu.hk/~jamesk/)<sup><b>1</b></sup><br/>
<sup><b>1</b></sup>HKUST, <sup><b>2</b></sup>CityU, <sup><b>3</b></sup>HKUST(GZ), <sup><b>4</b></sup>UIUC, <b>\*</b>Equal Contribution
<br/>

![MODL](https://github.com/user-attachments/assets/87e893b2-eca7-4ae8-a6bf-9e1a48fedf31)


If you find this repository is useful for you, please cite our paper:
```
@article{chen2025modl,
      title={Gradient-Based Multi-Objective Deep Learning: Algorithms, Theories, Applications, and Beyond}, 
      author={Weiyu Chen and Xiaoyuan Zhang and Baijiong Lin and Xi Lin and Han Zhao and Qingfu Zhang and James T. Kwok},
      journal={arXiv preprint arXiv:2501.10945},
      year={2025},
}
```

## Contents
- [Related Survey](#related-survey)
- [Finding a Single Solution](#finding-a-single-solution)
  - [Loss Balancing Methods](#loss-balancing-methods)
  - [Gradient Balancing Methods](#gradient-balancing-methods)
    - [Gradient Weighting Methods](#gradient-weighting-methods)
    - [Gradient Manipulation Methods](#gradient-manipulation-methods)
- [Finding a Finite Set of Solutions](#finding-a-finite-set-of-solutions)
  - [Preference Vector-based Methods](#preference-vector-based-methods)
  - [Preference Vector-free Methods](#preference-vector-free-methods)
- [Finding an Infinite Set of Solutions](#finding-an-infinite-set-of-solutions)
  - [Hypernetwork-based Methods](#hypernetwork-based-methods)
  - [Preference-Conditioned Network-based Methods](#preference-conditioned-network-based-methods)
  - [Model Combination-based Methods](#model-combination-based-methods)
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

9. **Multi-objective Deep Learning: Taxonomy and Survey of the State of the Art** [[Paper](https://arxiv.org/abs/2412.01566)]   
   *Sebastian Peitz and Sedjro Salomon Hotegni*    
   arXiv:2412.01566, 2024.

## Finding a Single Solution
### Loss Balancing Methods

1. **Multi-Task Learning Using Uncertainty to Weigh Losses for Scene Geometry and Semantics** [[Paper](https://openaccess.thecvf.com/content_cvpr_2018/papers/Kendall_Multi-Task_Learning_Using_CVPR_2018_paper.pdf)]  
   *Alex Kendall, Yarin Gal, and Roberto Cipolla*  
   **CVPR**, 2018.
   
2. **End-To-End Multi-Task Learning With Attention** [[Paper](https://openaccess.thecvf.com/content_CVPR_2019/papers/Liu_End-To-End_Multi-Task_Learning_With_Attention_CVPR_2019_paper.pdf)]  
   *Shikun Liu, Edward Johns, and Andrew J. Davison*  
   **CVPR**, 2019.  

3. **Multi-Objective Meta Learning** [[Paper](https://openreview.net/pdf?id=wKf9iSu_TEm)] [[Code](https://github.com/Baijiong-Lin/MOML)]  
   *Feiyang Ye, Baijiong Lin, Zhixiong Yue, Pengxin Guo, Qiao Xiao, and Yu Zhang*  
   **NeurIPS**, 2021; [Journal version](https://doi.org/10.1016/j.artint.2024.104184) in **AIJ**, 2024.

4. **Towards Impartial Multi-task Learning** [[Paper](https://openreview.net/forum?id=IMPnRXEWpvr)]  
   *Liyang Liu, Yi Li, Zhanghui Kuang, Jing-Hao Xue, Yimin Chen, Wenming Yang, Qingmin Liao, and Wayne Zhang*  
   **ICLR**, 2021.

5. **Reasonable Effectiveness of Random Weighting: A Litmus Test for Multi-Task Learning** [[Paper](https://openreview.net/forum?id=jjtFD8A1Wx)]  
   *Baijiong Lin, Feiyang Ye, Yu Zhang, and Ivor W. Tsang*  
   Transactions on Machine Learning Research (**TMLR**), 2022.

6. **Auto-Lambda: Disentangling Dynamic Task Relationships** [[Paper](https://openreview.net/forum?id=KKeCMim5VN)] [[Code](https://github.com/lorenmt/auto-lambda)]  
   *Shikun Liu, Stephen James, Andrew Davison, and Edward Johns*  
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

### Gradient Balancing Methods
#### Gradient Weighting Methods

1. **GradNorm: Gradient Normalization for Adaptive Loss Balancing in Deep Multitask Networks** [[Paper](http://proceedings.mlr.press/v80/chen18a/chen18a.pdf)]  
   *Zhao Chen, Vijay Badrinarayanan, Chen-Yu Lee, and Andrew Rabinovich*  
   **ICML**, 2018.

2. **Multi-Task Learning as Multi-Objective Optimization** [[Paper](https://papers.nips.cc/paper/2018/hash/432aca3a1e345e339f35a30c8f65edce-Abstract.html)] [[Code](https://github.com/isl-org/MultiObjectiveOptimization)]  
   *Ozan Sener and Vladlen Koltun*  
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
   *Peiyao Xiao, Hao Ban, and Kaiyi Ji*  
   **NeurIPS**, 2023.

10. **Dual-Balancing for Multi-Task Learning** [[Paper](https://arxiv.org/abs/2308.12029)]  
    *Baijiong Lin, Weisen Jiang, Feiyang Ye, Yu Zhang, Pengguang Chen, Ying-Cong Chen, Shu Liu, and James T. Kwok*  
    arXiv:2308.12029, 2023.

11. **Fair Resource Allocation in Multi-Task Learning** [[Paper](https://openreview.net/forum?id=KLmWRMg6nL)] [[Code](https://github.com/OptMN-Lab/fairgrad)]  
   *Hao Ban and Kaiyi Ji*  
   **ICML**, 2024.

12. **Jacobian Descent for Multi-Objective Optimization** [[Paper](https://arxiv.org/abs/2406.16232)] [[Code](https://github.com/TorchJD/torchjd)]   
   *Pierre Quinton and Valérian Rey*
   arXiv:2406.16232, 2024.

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

## Finding a Finite Set of Solutions
### Preference Vector-based Methods

1. **Pareto Multi-Task Learning** [[Paper](https://proceedings.neurips.cc/paper_files/paper/2019/file/685bfde03eb646c27ed565881917c71c-Paper.pdf)] [[Code](https://github.com/Xi-L/ParetoMTL)]   
   *Xi Lin, Hui-Ling Zhen, Zhenhua Li, Qingfu Zhang, and Sam Kwong*  
   **NeurIPS**, 2019.

2. **Multi-Task Learning with User Preferences: Gradient Descent with Controlled Ascent in Pareto Optimization** [[Paper](https://proceedings.mlr.press/v119/mahapatra20a.html)]  
   *Debabrata Mahapatra and Vaibhav Rajan*  
   **ICML**, 2020.

3. **Exact Pareto Optimal Search for Multi-Task Learning and Multi-Criteria Decision-Making** [[Paper](https://arxiv.org/abs/2108.00597v2)]  
   *Debabrata Mahapatra and Vaibhav Rajan*  
   arXiv:2108.00597, 2021

4. **A Multi-objective / Multi-task Learning Framework Induced by Pareto Stationarity** [[Paper](https://proceedings.mlr.press/v162/momma22a.html)]  
   *Michinari Momma, Chaosheng Dong, and Jia Liu*  
   **ICML**, 2022.

5. **Multi-Objective Deep Learning with Adaptive Reference Vectors** [[Paper](https://openreview.net/forum?id=9-8YT5G36g-)]  
   *Weiyu Chen and James T. Kwok*  
   **NeurIPS**, 2022.

6. **PMGDA: A Preference-based Multiple Gradient Descent Algorithm** [[Paper](https://arxiv.org/abs/2402.09492)]  
   *Xiaoyuan Zhang, Xi Lin, and Qingfu Zhang*  
   arXiv:2402.09492, 2024.

7. **FERERO: A Flexible Framework for Preference-Guided Multi-Objective Learning** [[Paper](https://openreview.net/forum?id=BmG3NgH5xu)] [[Code](https://github.com/lisha-chen/FERERO/)]  
   *Lisha Chen, A F M Saif, Yanning Shen, and Tianyi Chen*  
   **NeurIPS**, 2024.

8. **Gliding over the Pareto Front with Uniform Designs** [[Paper](https://openreview.net/forum?id=WoEXVQcHFw)]   
   *Xiaoyuan Zhang, Genghui Li, Xi Lin, Yichi Zhang, Yifan Chen, and Qingfu Zhang*   
   **NeurIPS**, 2024.

### Preference Vector-free Methods

1. **Multi-objective Optimization by Uncrowded Hypervolume Gradient Ascent** [[Paper](https://doi.org/10.1007/978-3-030-58115-2_13)] [[Code](https://github.com/scmaree/uncrowded-hypervolume)]   
   *Timo M. Deist, Stefanus C. Maree, Tanja Alderliesten, and Peter A.N. Bosman*  
   **PPSN**, 2020.

2. **Multi-Objective Learning to Predict Pareto Fronts Using Hypervolume Maximization** [[Paper](https://arxiv.org/abs/2102.04523)]   
   *Timo M. Deist, Monika Grewal, Frank J.W.M. Dankers, Tanja Alderliesten, and Peter A.N. Bosman*   
   arXiv:2102.04523, 2021.

3. **Profiling Pareto Front With Multi-Objective Stein Variational Gradient Descent** [[Paper](https://openreview.net/forum?id=S2-j0ZegyrE)] [[Code](https://github.com/gnobitab/MultiObjectiveSampling)]  
   *Xingchao Liu, Xin Tong, and Qiang Liu*   
   **NeurIPS**, 2021.

4. **Efficient Algorithms for Sum-Of-Minimum Optimization** [[Paper](https://openreview.net/forum?id=jsmaWEdx9g)]   
   *Lisang Ding, Ziang Chen, Xinshang Wang, and Wotao Yin*   
   **ICML**, 2024.

5. **Few for Many: Tchebycheff Set Scalarization for Many-Objective Optimization** [[Paper](https://arxiv.org/abs/2405.19650)]   
   *Xi Lin, Yilu Liu, Xiaoyuan Zhang, Fei Liu, Zhenkun Wang, and Qingfu Zhang*   
   arXiv:2405.19650, 2024.

6. **Many-Objective Multi-Solution Transport** [[Paper](https://arxiv.org/abs/2403.04099)]   
   *Ziyue Li, Tian Li, Virginia Smith, Jeff Bilmes, and Tianyi Zhou*  
   arXiv:2403.04099, 2024.

## Finding an Infinite Set of Solutions
### Hypernetwork-based Methods

1. **Controllable Pareto Multi-Task Learning** [[Paper](https://arxiv.org/abs/2010.06313)]  
   *Xi Lin, Zhiyuan Yang, Qingfu Zhang, and Sam Kwong*  
   arXiv:2010.06313, 2020.

2. **Learning the Pareto Front with Hypernetworks** [[Paper](https://openreview.net/forum?id=NjF772F4ZZR)] [[Code](https://github.com/AvivNavon/pareto-hypernetworks)]    
   *Aviv Navon, Aviv Shamsian, Ethan Fetaya, and Gal Chechik*  
   **ICLR**, 2021.

3. **Learning a Neural Pareto Manifold Extractor with Constraints** [[Paper](https://openreview.net/forum?id=BcIfJuIscx5)]   
   *Soumyajit Gupta, Gurpreet Singh, Raghu Bollapragada, and Matthew Lease*   
   **UAI**, 2022.

4. **Improving Pareto Front Learning via Multi-Sample Hypernetworks** [[Paper](https://ojs.aaai.org/index.php/AAAI/article/view/25953)]  
   *Long P. Hoang, Dung D. Le, Tran Anh Tuan, and Tran Ngoc Thang*   
   **AAAI**, 2023.

5. **A Hyper-Transformer model for Controllable Pareto Front Learning with Split Feasibility Constraints** [[Paper](https://arxiv.org/pdf/2402.05955)]  
   *Tran Anh Tuan, Nguyen Viet Dung, and Tran Ngoc Thang*  
   arXiv:2402.05955, 2024.

### Preference-Conditioned Network-based Methods

1. **You Only Train Once: Loss-Conditional Training of Deep Networks** [[Paper](https://openreview.net/pdf?id=HyxY6JHKwr)]  
   *Alexey Dosovitskiy and Josip Djolonga*  
   **ICLR** 2020.

2. **Scalable Pareto Front Approximation for Deep Multi-Objective Learning** [[Paper](https://ieeexplore.ieee.org/document/9679014)]  
   *Michael Ruchte and Josif Grabocka*  
   **ICDM**, 2021.

3. **Controllable Dynamic Multi-Task Architectures** [[Paper](https://openaccess.thecvf.com/content/CVPR2022/html/Raychaudhuri_Controllable_Dynamic_Multi-Task_Architectures_CVPR_2022_paper.html)]   
   *Dripta S. Raychaudhuri, Yumin Suh, Samuel Schulter, Xiang Yu, Masoud Faraki, Amit K. Roy-Chowdhury, and Manmohan Chandraker*   
   **CVPR**, 2022.

### Model Combination-based Methods

1. **Pareto Manifold Learning: Tackling Multiple Tasks via Ensembles of Single-Task Models** [[Paper](https://openreview.net/forum?id=BUlx0rh7ha)] [[Code](https://github.com/nik-dim/pamal)]  
   *Nikolaos Dimitriadis, Pascal Frossard, and Francois Fleuret*  
   **ICML**, 2023.

2. **Efficient Pareto Manifold Learning with Low-Rank Structure** [[Paper](https://openreview.net/forum?id=a2uFstsHPb)]   
   *Weiyu Chen and James T. Kwok*   
   **ICML**, 2024.

3. **Panacea: Pareto Alignment via Preference Adaptation for LLMs** [[Paper](https://openreview.net/forum?id=gL5nT4y8fn)]  
   *Yifan Zhong, Chengdong Ma, Xiaoyuan Zhang, Ziran Yang, Haojun Chen, Qingfu Zhang, Siyuan Qi, and Yaodong Yang*  
   **NeurIPS**, 2024.

4. **You Only Merge Once: Learning the Pareto Set of Preference-Aware Model Merging** [[Paper](https://arxiv.org/abs/2408.12105)]   
   *Weiyu Chen and James T. Kwok*   
   arXiv:2408.12105, 2024.

5. **Towards Efficient Pareto Set Approximation via Mixture of Experts Based Model Fusion** [[Paper](https://arxiv.org/pdf/2406.09770)]  
   *Anke Tang, Li Shen, Yong Luo, Shiwei Liu, Han Hu, and Bo Du*  
   arXiv:2406.09770, 2024.

6. **Pareto Low-Rank Adapters: Efficient Multi-Task Learning with Preferences** [[Paper](https://arxiv.org/abs/2407.08056)]   
   *Nikolaos Dimitriadis, Pascal Frossard, and Francois Fleuret*   
   arXiv:2407.08056, 2024.

## Resources
### Software
1. **LibMTL: A PyTorch Library for Multi-Task Learning** [[Paper](https://jmlr.org/papers/v24/22-0347.html)] [[Code](https://github.com/median-research-group/LibMTL)] [![GitHub stars](https://img.shields.io/github/stars/median-research-group/LibMTL.svg?style=social)](https://github.com/median-research-group/LibMTL) [![GitHub forks](https://img.shields.io/github/forks/median-research-group/LibMTL.svg?style=social)](https://github.com/median-research-group/LibMTL)    
   *Baijiong Lin and Yu Zhang*  
   Journal of Machine Learning Research (**JMLR**), 2023.
   
2. **LibMOON: A Gradient-based MultiObjective OptimizatioN Library in PyTorch** [[Paper](https://openreview.net/forum?id=etdXLAMZoc)] [[Code](https://github.com/xzhang2523/libmoon)] [![GitHub stars](https://img.shields.io/github/stars/xzhang2523/libmoon.svg?style=social)](https://github.com/xzhang2523/libmoon) [![GitHub forks](https://img.shields.io/github/forks/xzhang2523/libmoon.svg?style=social)](https://github.com/xzhang2523/libmoon)    
   *Xiaoyuan Zhang, Liang Zhao, Yingying Yu, Xi Lin, Zhenkun Wang, Han Zhao, and Qingfu Zhang*  
   **NeurIPS** Datasets and Benchmarks Track, 2024.
