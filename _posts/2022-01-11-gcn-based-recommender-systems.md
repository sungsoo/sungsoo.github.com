---
layout: post
title: GNN based Recommender Systems
date: 2022-01-12
categories: [computer science]
tags: [machine learning, graph mining]

---

### Article Source

* [GNN based Recommender Systems](https://github.com/tsinghua-fib-lab/GNN-Recommender-Systems)



---

# GNN based Recommender Systems
An index of recommendation algorithms that are based on Graph Neural Networks.

Our survey **Graph Neural Networks for Recommender Systems: Challenges, Methods, and Directions** is available on arxiv: [link](https://arxiv.org/pdf/2109.12843.pdf)

Please cite our survey paper if this index is helpful.

```
@article{gao2021graph,
  title={Graph Neural Networks for Recommender Systems: Challenges, Methods, and Directions},
  author={Gao, Chen and Zheng, Yu and Li, Nian and Li, Yinfeng and Qin, Yingrong and Piao, Jinghua and Quan, Yuhan and Chang, Jianxin and Jin, Depeng and He, Xiangnan and others},
  journal={arXiv preprint arXiv:2109.12843},
  year={2021}
}
```
```
Gao, C., Zheng, Y., Li, N., Li, Y., Qin, Y., Piao, J., Quan, Y., Chang, J., Jin, D., He, X., & Li, Y. (2021). Graph Neural Networks for Recommender Systems: Challenges, Methods, and Directions. arXiv preprint arXiv:2109.12843.
```

# Table of Contents

- [GNN in different recommendation stages](#Recommendation-Stages)
   - [Matching](#Matching)
   - [Ranking](#Ranking)
   - [Re-ranking](#Re-ranking)
- [GNN in different recommendation scenarios](#Recommendation-Scenarios)
   - [Social Recommendation](#Social-Recommendation)
   - [Sequential Recommendation](#Sequential-Recommendation)
   - [Session Recommendation](#Session-Recommendation)
   - [Bundle Recommendation](#Bundle-Recommendation)
   - [Cross Domain Recommendation](#Cross-Domain-Recommendation)
   - [Multi-behavior Recommendation](#Multi-behavior-Recommendation)
- [GNN for different recommendation objectives](#Recommendation-Objectives)
   - [Diversity](#Diversity)
   - [Explainability](#Explainability)
   - [Fairness](#Fairness)
   - 
## Recommendation Stages
### Matching

| **Name** | **Paper** | **Venue** | **Year** | **Code** |
| --- | --- | --- | --- | --- |
| GCMC | [Berg, R. V. D., Kipf, T. N., & Welling, M. (2017). Graph convolutional matrix completion. _arXiv preprint arXiv:1706.02263_.](https://arxiv.org/pdf/1706.02263.pdf) | arxiv | 2017 | [Python](https://paperswithcode.com/paper/graph-convolutional-matrix-completion) |
| Pin-Sage | [Ying, R., He, R., Chen, K., Eksombatchai, P., Hamilton, W. L., & Leskovec, J. (2018, July). Graph convolutional neural networks for web-scale recommender systems. In Proceedings of the 24th ACM SIGKDD International Conference on Knowledge Discovery & Data Mining (pp. 974-983).](https://arxiv.org/pdf/1806.01973) | KDD | 2018 | [Python](https://paperswithcode.com/paper/graph-convolutional-neural-networks-for-web) |
| NGCF | [Wang, X., He, X., Wang, M., Feng, F., & Chua, T. S. (2019, July). Neural graph collaborative filtering. In _Proceedings of the 42nd international ACM SIGIR conference on Research and development in Information Retrieval_ (pp. 165-174).](https://arxiv.org/pdf/1905.08108.pdf) | SIGIR | 2019 | [Python](https://paperswithcode.com/paper/neural-graph-collaborative-filtering) |
| DGCF | [Wang, X., Jin, H., Zhang, A., He, X., Xu, T., & Chua, T. S. (2020, July). Disentangled graph collaborative filtering. In _Proceedings of the 43rd International ACM SIGIR Conference on Research and Development in Information Retrieval_ (pp. 1001-1010).](https://arxiv.org/pdf/2007.01764) | SIGIR | 2020 | [Python](https://paperswithcode.com/paper/disentangled-graph-collaborative-filtering) |
| LightGCN | [He, X., Deng, K., Wang, X., Li, Y., Zhang, Y., & Wang, M. (2020, July). Lightgcn: Simplifying and powering graph convolution network for recommendation. In _Proceedings of the 43rd International ACM SIGIR conference on research and development in Information Retrieval_ (pp. 639-648).](https://arxiv.org/pdf/2002.02126.pdf) | SIGIR | 2020 | [Python](https://paperswithcode.com/paper/lightgcn-simplifying-and-powering-graph) |
| NIA-GCN | [Sun, J., Zhang, Y., Guo, W., Guo, H., Tang, R., He, X., ... & Coates, M. (2020, July). Neighbor interaction aware graph convolution networks for recommendation. In Proceedings of the 43rd International ACM SIGIR Conference on Research and Development in Information Retrieval (pp. 1289-1298).](https://dl.acm.org/doi/abs/10.1145/3397271.3401123) | SIGIR | 2020 | NA |
| SGL | [Wu, J., Wang, X., Feng, F., He, X., Chen, L., Lian, J., & Xie, X. (2021, July). Self-supervised graph learning for recommendation. In _Proceedings of the 44th International ACM SIGIR Conference on Research and Development in Information Retrieval_ (pp. 726-735).](https://arxiv.org/pdf/2010.10783) | SIGIR | 2021 | [Python](https://github.com/wujcan/SGL) |

### Ranking

| **Name** | **Paper** | **Venue** | **Year** | **Code** |
| --- | --- | --- | --- | --- |
| Fi-GNN | [Li, Z., Cui, Z., Wu, S., Zhang, X., & Wang, L. (2019, November). Fi-gnn: Modeling feature interactions via graph neural networks for ctr prediction. In _Proceedings of the 28th ACM International Conference on Information and Knowledge Management_ (pp. 539-548).](https://arxiv.org/pdf/1910.05552.pdf) | CIKM | 2019 | [Python](https://paperswithcode.com/paper/fi-gnn-modeling-feature-interactions-via) |
| PUP | [Zheng, Y., Gao, C., He, X., Li, Y., & Jin, D. (2020, April). Price-aware recommendation with graph convolutional networks. In _2020 IEEE 36th International Conference on Data Engineering (ICDE)_ (pp. 133-144). IEEE.](https://arxiv.org/pdf/2003.03975.pdf) | ICDE | 2020 | [Python](https://github.com/DavyMorgan/ICDE20-PUP) |
| L0-SIGN | [Su, Y., Zhang, R., Erfani, S., & Xu, Z. (2021, May). Detecting Beneficial Feature Interactions for Recommender Systems. In _Proceedings of the 34th AAAI Conference on Artificial Intelligence (AAAI)_.](https://arxiv.org/pdf/2008.00404.pdf) | AAAI | 2021 | [Python](https://github.com/ruizhang-ai/SIGN-Detecting-Beneficial-Feature-Interactions-for-Recommender-Systems) |
| DG-ENN | [Guo, W., Su, R., Tan, R., Guo, H., Zhang, Y., Liu, Z., ... & He, X. (2021). Dual Graph enhanced Embedding Neural Network for CTRPrediction. _arXiv preprint arXiv:2106.00314_.](https://arxiv.org/pdf/2106.00314.pdf) | KDD | 2021 | NA |
| SHCF | [Li, C., Hu, L., Shi, C., Song, G., & Lu, Y. (2021). Sequence-aware Heterogeneous Graph Neural Collaborative Filtering. In _Proceedings of the 2021 SIAM International Conference on Data Mining (SDM)_ (pp. 64-72). Society for Industrial and Applied Mathematics.](http://www.shichuan.org/doc/98.pdf) | SDM | 2021 | [Python](http://www.shichuan.org/dataset/SHCF.zip) |
| GCM | [Wu, J., He, X., Wang, X., Wang, Q., Chen, W., Lian, J., & Xie, X. (2020). Graph Convolution Machine for Context-aware Recommender System. _arXiv preprint arXiv:2001.11402_.](https://arxiv.org/pdf/2001.11402.pdf) | Frontiers of Computer Science | 2021 | [Python](https://github.com/wujcan/GCM) |

### Re-ranking

| **Name** | **Paper** | **Venue** | **Year** | **Code** |
| --- | --- | --- | --- | --- |
| IRGPR | [Liu, W., Liu, Q., Tang, R., Chen, J., He, X., & Heng, P. A. (2020, October). Personalized Re-ranking with Item Relationships for E-commerce. In _Proceedings of the 29th ACM International Conference on Information & Knowledge Management_ (pp. 925-934).](https://dl.acm.org/doi/abs/10.1145/3340531.3412332) | CIKM | 2020 | NA |

## Recommendation Scenarios
### Social Recommendation

| **Name** | **Paper** | **Venue** | **Year** | **Code** |
| --- | --- | --- | --- | --- |
| DGRec | [Song, W., Xiao, Z., Wang, Y., Charlin, L., Zhang, M., & Tang, J. (2019, January). Session-based social recommendation via dynamic graph attention networks. In _Proceedings of the Twelfth ACM international conference on web search and data mining_ (pp. 555-563).](https://arxiv.org/pdf/1902.09362) | WSDM | 2019 | [Python](https://github.com/DeepGraphLearning/RecommenderSystems) |
| GraphRec | [Fan, W., Ma, Y., Li, Q., He, Y., Zhao, E., Tang, J., & Yin, D. (2019, May). Graph neural networks for social recommendation. In _The World Wide Web Conference_ (pp. 417-426).](https://arxiv.org/pdf/1902.07243) | WWW | 2019 | [Python](https://paperswithcode.com/paper/graph-neural-networks-for-social) |
| DANSER | [Wu, Q., Zhang, H., Gao, X., He, P., Weng, P., Gao, H., & Chen, G. (2019, May). Dual graph attention networks for deep latent representation of multifaceted social effects in recommender systems. In _The World Wide Web Conference_ (pp. 2091-2102).](https://arxiv.org/pdf/1903.10433) | WWW | 2019 | [Python](https://github.com/qitianwu/DANSER-WWW-19) |
| DiffNet | [Wu, L., Sun, P., Fu, Y., Hong, R., Wang, X., & Wang, M. (2019, July). A neural influence diffusion model for social recommendation. In _Proceedings of the 42nd international ACM SIGIR conference on research and development in information retrieval_ (pp. 235-244).](https://arxiv.org/pdf/1904.10322) | SIGIR | 2019 | [Python](https://paperswithcode.com/paper/a-neural-influence-diffusion-model-for-social) |
| RecoGCN | [Xu, F., Lian, J., Han, Z., Li, Y., Xu, Y., & Xie, X. (2019, November). Relation-aware graph convolutional networks for agent-initiated social e-commerce recommendation. In _Proceedings of the 28th ACM international conference on information and knowledge management_ (pp. 529-538).](https://dl.acm.org/doi/10.1145/3357384.3357924) | CIKM | 2019 | [Python](https://github.com/xfl15/RecoGCN) |
| HGP | [Kim, K. M., Kwak, D., Kwak, H., Park, Y. J., Sim, S., Cho, J. H., ... & Ha, J. W. (2019). Tripartite heterogeneous graph propagation for large-scale social recommendation. _arXiv preprint arXiv:1908.02569_.](https://arxiv.org/pdf/1908.02569) | RecSys | 2019 | NA |
| GAT-NSR | [Mu, N., Zha, D., He, Y., & Tang, Z. (2019, November). Graph attention networks for neural social recommendation. In _2019 IEEE 31st International Conference on Tools with Artificial Intelligence (ICTAI)_ (pp. 1320-1327). IEEE.](https://ieeexplore.ieee.org/abstract/document/8995280) | ICTAI | 2019 | NA |
| SR-HGNN | [Xu, H., Huang, C., Xu, Y., Xia, L., Xing, H., & Yin, D. (2020, November). Global context enhanced social recommendation with hierarchical graph neural networks. In _2020 IEEE International Conference on Data Mining (ICDM)_ (pp. 701-710). IEEE.](https://ieeexplore.ieee.org/abstract/document/9338365) | ICDM | 2020 | [Python](https://github.com/xhcdream/SR-HGNN) |
| TGRec | [Bai, T., Zhang, Y., Wu, B., & Nie, J. Y. (2020, December). Temporal Graph Neural Networks for Social Recommendation. In _2020 IEEE International Conference on Big Data (Big Data)_ (pp. 898-903). IEEE.](https://ieeexplore.ieee.org/abstract/document/9378444) | ICBD | 2020 | NA |
| DiffNet++ | [Wu, L., Li, J., Sun, P., Hong, R., Ge, Y., & Wang, M. (2020). Diffnet++: A neural influence and interest diffusion network for social recommendation. _IEEE Transactions on Knowledge and Data Engineering_.](https://arxiv.org/pdf/2002.00844) | TKDE | 2020 | [Python](https://github.com/PeiJieSun/diffnet) |
| ESRF | [Yu, J., Yin, H., Li, J., Gao, M., Huang, Z., & Cui, L. (2020). Enhance social recommendation with adversarial graph convolutional networks. _IEEE Transactions on Knowledge and Data Engineering_.](https://arxiv.org/pdf/2004.02340) | TKDE | 2020 | [Python](https://github.com/Coder-Yu/QRec) |
| HOSR | [Liu, Y., Liang, C., He, X., Peng, J., Zheng, Z., & Tang, J. (2020). Modelling high-order social relations for item recommendation. _IEEE Transactions on Knowledge and Data Engineering_.](https://arxiv.org/pdf/2003.10149) | TKDE | 2020 | NA |
| GNN-SoR | [Guo, Z., & Wang, H. (2020). A deep graph neural network-based mechanism for social recommendations. _IEEE Transactions on Industrial Informatics_, _17_(4), 2776-2783.](https://ieeexplore.ieee.org/abstract/document/9063418) | TII | 2020 | NA |
| ASR | [Luo, D., Bian, Y., Zhang, X., & Huan, J. (2020). Attentive Social Recommendation: Towards User And Item Diversities. _arXiv preprint arXiv:2011.04797_.](https://arxiv.org/pdf/2011.04797) | arxiv | 2020 | [Python](https://github.com/flyingdoog/ASR) |
| KCGN | [Huang, C., Xu, H., Xu, Y., Dai, P., Xia, L., Lu, M., ... & Ye, Y. (2021, January). Knowledge-aware coupled graph neural network for social recommendation. In _AAAI Conference on Artificial Intelligence (AAAI)_.](https://www.aaai.org/AAAI21Papers/AAAI-9069.HuangC.pdf) | AAAI | 2021 | [Python](https://github.com/xhcdream/KCGN) |
| MHCN | [Yu, J., Yin, H., Li, J., Wang, Q., Hung, N. Q. V., & Zhang, X. (2021, April). Self-Supervised Multi-Channel Hypergraph Convolutional Network for Social Recommendation. In _Proceedings of the Web Conference 2021_ (pp. 413-424).](https://arxiv.org/pdf/2101.06448) | WWW | 2021 | [Python](https://github.com/Coder-Yu/QRec) |
| GBGCN | [Zhang, J., Gao, C., Jin, D., & Li, Y. (2021, April). Group-Buying Recommendation for Social E-Commerce. In _2021 IEEE 37th International Conference on Data Engineering (ICDE)_ (pp. 1536-1547). IEEE.](https://arxiv.org/pdf/2010.06848) | ICDE | 2021 | [Python](https://github.com/Sweetnow/group-buying-recommendation) |
| SEPT | [Yu, J., Yin, H., Gao, M., Xia, X., Zhang, X., & Hung, N. Q. V. (2021). Socially-Aware Self-Supervised Tri-Training for Recommendation. _arXiv preprint arXiv:2106.03569_.](https://arxiv.org/pdf/2106.03569) | KDD | 2021 | [Python](https://github.com/Coder-Yu/QRec) |
| DiffNetLG | [Song, C., Wang, B., Jiang, Q., Zhang, Y., He, R., & Hou, Y. (2021, July). Social Recommendation with Implicit Social Influence. In _Proceedings of the 44th International ACM SIGIR Conference on Research and Development in Information Retrieval_ (pp. 1788-1792).](https://dl.acm.org/doi/abs/10.1145/3404835.3463043) | SIGIR | 2021 | NA |

### Sequential Recommendation

| **Name** | **Paper** | **Venue** | **Year** | **Code** |
| --- | --- | --- | --- | --- |
| GME | [Xie, M., Yin, H., Xu, F., Wang, H., & Zhou, X. (2016, November). Graph-based metric embedding for next poi recommendation. In _International Conference on Web Information Systems Engineering_ (pp. 207-222). Springer, Cham.](http://net.pku.edu.cn/daim/hongzhi.yin/papers/WISE-2016.pdf) | WISE | 2016 | NA |
| MA-GNN | [Ma, C., Ma, L., Zhang, Y., Sun, J., Liu, X., & Coates, M. (2020, April). Memory augmented graph neural networks for sequential recommendation. In _Proceedings of the AAAI Conference on Artificial Intelligence_ (Vol. 34, No. 04, pp. 5045-5052).](https://ojs.aaai.org/index.php/AAAI/article/download/5945/5801) | AAAI | 2020 | NA |
| ISSR | [Liu, F., Liu, W., Li, X., & Ye, Y. (2020). Inter-sequence Enhanced Framework for Personalized Sequential Recommendation. _arXiv preprint arXiv:2004.12118_.](https://arxiv.org/pdf/2004.12118) | AAAI | 2020 | NA |
| STP-UDGAT | [Lim, N., Hooi, B., Ng, S. K., Wang, X., Goh, Y. L., Weng, R., & Varadarajan, J. (2020, October). STP-UDGAT: Spatial-Temporal-Preference User Dimensional Graph Attention Network for Next POI Recommendation. In _Proceedings of the 29th ACM International Conference on Information & Knowledge Management_ (pp. 845-854).](https://arxiv.org/pdf/2010.07024) | CIKM | 2020 | NA |
| GPR | [Chang, B., Jang, G., Kim, S., & Kang, J. (2020, October). Learning graph-based geographical latent representation for point-of-interest recommendation. In _Proceedings of the 29th ACM International Conference on Information & Knowledge Management_ (pp. 135-144).](https://dl.acm.org/doi/abs/10.1145/3340531.3411905) | CIKM | 2020 | NA |
| Wang _et al._ | [Wang, B., & Cai, W. (2020). Knowledge-enhanced graph neural networks for sequential recommendation. _Information_, _11_(8), 388.](https://www.mdpi.com/2078-2489/11/8/388/pdf) | Information | 2020 | NA |
| SGRec | [Li, Y., Chen, T., Yin, H., & Huang, Z. (2021). Discovering Collaborative Signals for Next POI Recommendation with Iterative Seq2Graph Augmentation. _arXiv preprint arXiv:2106.15814_.](https://arxiv.org/pdf/2106.15814) | IJCAI | 2021 | NA |
| RetaGNN | [Hsu, C., & Li, C. T. (2021, April). RetaGNN: Relational Temporal Attentive Graph Neural Networks for Holistic Sequential Recommendation. In _Proceedings of the Web Conference 2021_ (pp. 2968-2979).](https://arxiv.org/pdf/2101.12457) | WWW | 2021 | [Python](https://github.com/retagnn/RetaGNN) |
| SURGE | [Chang, J., Gao, C., Zheng, Y., Hui, Y., Niu, Y., Song, Y., ... & Li, Y. (2021, July). Sequential Recommendation with Graph Neural Networks. In _Proceedings of the 44th International ACM SIGIR Conference on Research and Development in Information Retrieval_ (pp. 378-387).](https://arxiv.org/pdf/2106.14226) | SIGIR | 2021 | [Python](https://github.com/tsinghua-fib-lab/SIGIR21-SURGE) |
| TGSRec | [Fan, Z., Liu, Z., Zhang, J., Xiong, Y., Zheng, L., & Yu, P. S. (2021). Continuous-Time Sequential Recommendation with Temporal Graph Collaborative Transformer. _arXiv preprint arXiv:2108.06625_.](https://arxiv.org/pdf/2108.06625) | CIKM | 2021 | [Python](https://github.com/DyGRec/TGSRec) |
| GES-SASRec | [Zhu, T., Sun, L., & Chen, G. (2021). Graph-based Embedding Smoothing for Sequential Recommendation. _IEEE Transactions on Knowledge and Data Engineering_.](https://ieeexplore.ieee.org/abstract/document/9405450/) | TKDE | 2021 | [Python](https://github.com/zhuty16/GES) |
| DGSR | [Zhang, M., Wu, S., Yu, X., & Wang, L. (2021). Dynamic Graph Neural Networks for Sequential Recommendation. _arXiv preprint arXiv:2104.07368_.](https://arxiv.org/pdf/2104.07368) | arxiv | 2021 | NA |

### Session Recommendation

| **Name** | **Paper** | **Venue** | **Year** | **Code** |
| --- | --- | --- | --- | --- |
| SR-GNN | [Wu, S., Tang, Y., Zhu, Y., Wang, L., Xie, X., & Tan, T. (2019, July). Session-based recommendation with graph neural networks. In _Proceedings of the AAAI Conference on Artificial Intelligence_ (Vol. 33, No. 01, pp. 346-353).](https://ojs.aaai.org/index.php/AAAI/article/view/3804/3682) | AAAI | 2019 | [Python](https://paperswithcode.com/paper/session-based-recommendation-with-graph) |
| GC-SAN | [Xu, C., Zhao, P., Liu, Y., Sheng, V. S., Xu, J., Zhuang, F., ... & Zhou, X. (2019, August). Graph Contextualized Self-Attention Network for Session-based Recommendation. In _IJCAI_ (Vol. 19, pp. 3940-3946).](https://www.ijcai.org/proceedings/2019/0547.pdf) | IJCAI | 2019 | [Python](https://github.com/RUCAIBox/RecBole/blob/master/recbole/model/sequential_recommender/gcsan.py) |
| FGNN | [Qiu, R., Li, J., Huang, Z., & Yin, H. (2019, November). Rethinking the item order in session-based recommendation with graph neural networks. In _Proceedings of the 28th ACM International Conference on Information and Knowledge Management_ (pp. 579-588).](https://arxiv.org/pdf/1911.11942) | CIKM | 2019 | [Python](https://github.com/RuihongQiu/FGNN) |
| MGNN-SPred | [Wang, W., Zhang, W., Liu, S., Liu, Q., Zhang, B., Lin, L., & Zha, H. (2020, April). Beyond clicks: Modeling multi-relational item graph for session-based target behavior prediction. In _Proceedings of The Web Conference 2020_ (pp. 3056-3062).](https://arxiv.org/pdf/2002.07993) | WWW | 2020 | [Python](https://github.com/Autumn945/MGNN-SPred) |
| LESSR | [Chen, T., & Wong, R. C. W. (2020, August). Handling information loss of graph neural networks for session-based recommendation. In Proceedings of the 26th ACM SIGKDD International Conference on Knowledge Discovery & Data Mining (pp. 1172-1180).](http://home.cse.ust.hk/~raywong/paper/kdd20-informationLoss-GNN.pdf) | KDD | 2020 | [Python](https://github.com/twchen/lessr) |
| TA-GNN | [Yu, F., Zhu, Y., Liu, Q., Wu, S., Wang, L., & Tan, T. (2020, July). TAGNN: Target attentive graph neural networks for session-based recommendation. In _Proceedings of the 43rd International ACM SIGIR Conference on Research and Development in Information Retrieval_ (pp. 1921-1924).](https://arxiv.org/pdf/2005.02844) | SIGIR | 2020 | [Python](https://github.com/CRIPAC-DIG/TAGNN) |
| GCE-GNN | [Wang, Z., Wei, W., Cong, G., Li, X. L., Mao, X. L., & Qiu, M. (2020, July). Global context enhanced graph neural networks for session-based recommendation. In _Proceedings of the 43rd International ACM SIGIR Conference on Research and Development in Information Retrieval_ (pp. 169-178).](https://arxiv.org/pdf/2106.05081) | SIGIR | 2020 | [Python](https://github.com/CCIIPLab/GCE-GNN) |
| MKM-SR | [Meng, W., Yang, D., & Xiao, Y. (2020, July). Incorporating user micro-behaviors and item knowledge into multi-task learning for session-based recommendation. In Proceedings of the 43rd International ACM SIGIR Conference on Research and Development in Information Retrieval (pp. 1091-1100).](https://arxiv.org/pdf/2006.06922) | SIGIR | 2020 | [Python](https://github.com/ciecus/MKM-SR) |
| GAG | [Qiu, R., Yin, H., Huang, Z., & Chen, T. (2020, July). Gag: Global attributed graph neural network for streaming session-based recommendation. In _Proceedings of the 43rd International ACM SIGIR Conference on Research and Development in Information Retrieval_ (pp. 669-678).](https://arxiv.org/pdf/2007.02747) | SIGIR | 2020 | [Python](https://github.com/RuihongQiu/GAG) |
| SGNN-HN | [Pan, Z., Cai, F., Chen, W., Chen, H., & de Rijke, M. (2020, October). Star graph neural networks for session-based recommendation. In _Proceedings of the 29th ACM International Conference on Information & Knowledge Management_ (pp. 1195-1204).](https://irlab.science.uva.nl/wp-content/papercite-data/pdf/pan-2020-star.pdf) | CIKM | 2020 | NA |
| CAGE | [Sheu, H. S., & Li, S. (2020, September). Context-aware graph embedding for session-based news recommendation. In Fourteenth ACM conference on recommender systems (pp. 657-662).](https://dl.acm.org/doi/abs/10.1145/3383313.3418477) | RecSys | 2020 | NA |
| A-PGNN | [Zhang, M., Wu, S., Gao, M., Jiang, X., Xu, K., & Wang, L. (2020). Personalized graph neural networks with attention mechanism for session-aware recommendation. IEEE Transactions on Knowledge and Data Engineering.](https://arxiv.org/pdf/1910.08887) | TKDE | 2020 | [Python](https://paperswithcode.com/paper/personalizing-graph-neural-networks-with) |
| DGTN | [Zheng, Y., Liu, S., Li, Z., & Wu, S. (2020, November). DGTN: Dual-channel Graph Transition Network for Session-based Recommendation. In _2020 International Conference on Data Mining Workshops (ICDMW)_ (pp. 236-242). IEEE.](https://arxiv.org/pdf/2009.10002) | ICDMW | 2020 | [Python](https://github.com/kunwuz/DGTN) |
| DHCN | [Xia, X., Yin, H., Yu, J., Wang, Q., Cui, L., & Zhang, X. (2020). Self-supervised hypergraph convolutional networks for session-based recommendation. _arXiv preprint arXiv:2012.06852_.](https://ojs.aaai.org/index.php/AAAI/article/view/16578) | AAAI | 2021 | [Python](https://github.com/xiaxin1998/DHCN) |
| SERec | [Chen, T., & Wong, R. C. W. (2021, March). An Efficient and Effective Framework for Session-based Social Recommendation. In Proceedings of the 14th ACM International Conference on Web Search and Data Mining (pp. 400-408).](http://www.cse.ust.hk/~raywong/paper/wsdm21-SEFrame.pdf) | WSDM | 2021 | [Python](https://github.com/twchen/SEFrame) |
| TASRec | [Zhou, H., Tan, Q., Huang, X., Zhou, K., & Wang, X. (2021). Temporal Augmented Graph Neural Networks for Session-Based Recommendations.](https://www4.comp.polyu.edu.hk/~xiaohuang/docs/Huachi_sigir2021.pdf) | SIGIR | 2021 | NA |
| DAT-MDI | [Chen, C., Guo, J., & Song, B. (2021, July). Dual Attention Transfer in Session-based Recommendation with Multi-dimensional Integration. In Proceedings of the 44th International ACM SIGIR Conference on Research and Development in Information Retrieval (pp. 869-878).](https://dl.acm.org/doi/abs/10.1145/3404835.3462866) | SIGIR | 2021 | NA |
| COTREC | [Xia, X., Yin, H., Yu, J., Shao, Y., & Cui, L. (2021). Self-Supervised Graph Co-Training for Session-based Recommendation. arXiv preprint arXiv:2108.10560.](https://arxiv.org/pdf/2108.10560) | CIKM | 2021 | [Python](https://github.com/xiaxin1998/COTREC) |
| SHARE | [Wang, J., Ding, K., Zhu, Z., & Caverlee, J. (2021). Session-based Recommendation with Hypergraph Attention Networks. In _Proceedings of the 2021 SIAM International Conference on Data Mining (SDM)_ (pp. 82-90). Society for Industrial and Applied Mathematics.](https://epubs.siam.org/doi/pdf/10.1137/1.9781611976700.10) | SDM | 2021 | NA |

### Bundle Recommendation

| **Name** | **Paper** | **Venue** | **Year** | **Code** |
| --- | --- | --- | --- | --- |
| BGCN | [Chang, J., Gao, C., He, X., Jin, D., & Li, Y. (2020, July). Bundle recommendation with graph convolutional networks. In _Proceedings of the 43rd international ACM SIGIR conference on Research and development in Information Retrieval_ (pp. 1673-1676).](https://arxiv.org/pdf/2005.03475) | SIGIR | 2020 | [Python](https://github.com/cjx0525/BGCN) |
| HFGN | [Li, X., Wang, X., He, X., Chen, L., Xiao, J., & Chua, T. S. (2020, July). Hierarchical fashion graph network for personalized outfit recommendation. In _Proceedings of the 43rd International ACM SIGIR Conference on Research and Development in Information Retrieval_ (pp. 159-168).](https://arxiv.org/pdf/2005.12566) | SIGIR | 2020 | [Python](https://github.com/xcppy/hierarchical_fashion_graph_network) |
| BundleNet | [Deng, Q., Wang, K., Zhao, M., Zou, Z., Wu, R., Tao, J., ... & Chen, L. (2020, October). Personalized Bundle Recommendation in Online Games. In _Proceedings of the 29th ACM International Conference on Information & Knowledge Management_ (pp. 2381-2388).](https://arxiv.org/pdf/2104.05307) | CIKM | 2020 | NA |
| DPR | [Zheng, Z., Wang, C., Xu, T., Shen, D., Qin, P., Huai, B., ... & Chen, E. (2021, April). Drug Package Recommendation via Interaction-aware Graph Induction. In _Proceedings of the Web Conference 2021_ (pp. 1284-1295).](https://arxiv.org/pdf/2102.03577) | WWW | 2021 | NA |

### Cross Domain Recommendation

| **Name** | **Paper** | **Venue** | **Year** | **Code** |
| --- | --- | --- | --- | --- |
| PPGN | [Zhao, C., Li, C., & Fu, C. (2019, November). Cross-domain recommendation via preference propagation graphnet. In _Proceedings of the 28th ACM International Conference on Information and Knowledge Management_ (pp. 2165-2168).](https://dl.acm.org/doi/abs/10.1145/3357384.3358166) | CIKM | 2019 | [Python](https://github.com/WHUIR/PPGN) |
| BiTGCF | [Liu, M., Li, J., Li, G., & Pan, P. (2020, October). Cross Domain Recommendation via Bi-directional Transfer Graph Collaborative Filtering Networks. In _Proceedings of the 29th ACM International Conference on Information & Knowledge Management_ (pp. 885-894).](https://dl.acm.org/doi/abs/10.1145/3340531.3412012) | CIKM | 2020 | [Python](https://github.com/sunshinelium/Bi-TGCF) |
| DAN | [Wang, B., Zhang, C., Zhang, H., Lyu, X., & Tang, Z. (2020, October). Dual Autoencoder Network with Swap Reconstruction for Cold-Start Recommendation. In _Proceedings of the 29th ACM International Conference on Information & Knowledge Management_ (pp. 2249-2252).](https://dl.acm.org/doi/abs/10.1145/3340531.3412069) | CIKM | 2020 | NA |
| HeroGRAPH | [Cui, Q., Wei, T., Zhang, Y., & Zhang, Q. (2020). HeroGRAPH: A Heterogeneous Graph Framework for Multi-Target Cross-Domain Recommendation. In _ORSUM@ RecSys_.](http://ceur-ws.org/Vol-2715/paper6.pdf) | RecSys | 2020 | [Python](https://github.com/cuiqiang1990/HeroGRAPH) |
| DAGCN | [Guo, L., Tang, L., Chen, T., Zhu, L., Nguyen, Q. V. H., & Yin, H. (2021). DA-GCN: A Domain-aware Attentive Graph Convolution Network for Shared-account Cross-domain Sequential Recommendation. _arXiv preprint arXiv:2105.03300_.](https://arxiv.org/pdf/2105.03300) | IJCAI | 2021 | NA |

### Multi-behavior Recommendation

| **Name** | **Paper** | **Venue** | **Year** | **Code** |
| --- | --- | --- | --- | --- |
| MGNN-SPred | [Wang, W., Zhang, W., Liu, S., Liu, Q., Zhang, B., Lin, L., & Zha, H. (2020, April). Beyond clicks: Modeling multi-relational item graph for session-based target behavior prediction. In _Proceedings of The Web Conference 2020_ (pp. 3056-3062).](https://arxiv.org/pdf/2002.07993) | WWW | 2020 | [Python](https://github.com/Autumn945/MGNN-SPred) |
| MBGCN | [Jin, B., Gao, C., He, X., Jin, D., & Li, Y. (2020, July). Multi-behavior recommendation with graph convolutional networks. In _Proceedings of the 43rd International ACM SIGIR Conference on Research and Development in Information Retrieval_ (pp. 659-668).](http://staff.ustc.edu.cn/~hexn/papers/sigir20-MBGCN.pdf) | SIGIR | 2020 | NA |
| MGNN | [Zhang, W., Mao, J., Cao, Y., & Xu, C. (2020, October). Multiplex Graph Neural Networks for Multi-behavior Recommendation. In _Proceedings of the 29th ACM International Conference on Information & Knowledge Management_ (pp. 2313-2316).](https://dl.acm.org/doi/abs/10.1145/3340531.3412119) | CIKM | 2020 | NA |
| KHGT | [Xia, L., Huang, C., Xu, Y., Dai, P., Zhang, X., Yang, H., ... & Bo, L. (2021, May). Knowledge-Enhanced Hierarchical Graph Transformer Network for Multi-Behavior Recommendation. In _Proceedings of the AAAI Conference on Artificial Intelligence_ (Vol. 35, No. 5, pp. 4486-4493).](https://www.aaai.org/AAAI21Papers/AAAI-3071.XiaL.pdf) | AAAI | 2021 | [Python](https://github.com/akaxlh/KHGT) |
| GHCF | [Chen, C., Ma, W., Zhang, M., Wang, Z., He, X., Wang, C., ... & Ma, S. (2021, May). Graph Heterogeneous Multi-Relational Recommendation. In _Proceedings of the AAAI Conference on Artificial Intelligence_ (Vol. 35, No. 5, pp. 3958-3966).](https://www.aaai.org/AAAI21Papers/AAAI-615.ChenC.pdf) | AAAI | 2021 | [Python](https://github.com/chenchongthu/GHCF) |
| GNMR | [Xia, L., Huang, C., Xu, Y., Dai, P., Lu, M., & Bo, L. (2021, April). Multi-Behavior Enhanced Recommendation with Cross-Interaction Collaborative Relation Modeling. In _2021 IEEE 37th International Conference on Data Engineering (ICDE)_ (pp. 1931-1936). IEEE.](https://ieeexplore.ieee.org/abstract/document/9458929) | ICDE | 2021 | [Python](https://github.com/akaxlh/GNMR) |
| DMBGN | [Xiao, F., Li, L., Xu, W., Zhao, J., Yang, X., Lang, J., & Wang, H. (2021). DMBGN: Deep Multi-Behavior Graph Networks for Voucher Redemption Rate Prediction. _arXiv preprint arXiv:2106.03356_.](https://arxiv.org/pdf/2106.03356) | KDD | 2021 | [Python](https://github.com/fengtong-xiao/DMBGN) |
| MB-GMN | [Xia, L., Xu, Y., Huang, C., Dai, P., & Bo, L. (2021, July). Graph meta network for multi-behavior recommendation. In _Proceedings of the 44th International ACM SIGIR Conference on Research and Development in Information Retrieval_ (pp. 757-766).](https://dl.acm.org/doi/abs/10.1145/3404835.3462972) | SIGIR | 2021 | [Python](https://github.com/akaxlh/MB-GMN) |
| HMG-CR | [Yang, H., Chen, H., Li, L., Yu, P. S., & Xu, G. (2021). Hyper Meta-Path Contrastive Learning for Multi-Behavior Recommendation. _arXiv preprint arXiv:2109.02859_.](https://arxiv.org/pdf/2109.02859) | ICDM | 2021 | [Python](https://github.com/Haoran-Young/HMG-CR) |
| LP-MRGNN | [Wang, W., Zhang, W., Liu, S., Liu, Q., Zhang, B., Lin, L., & Zha, H. (2021). Incorporating Link Prediction into Multi-Relational Item Graph Modeling for Session-based Recommendation. _IEEE Transactions on Knowledge and Data Engineering_.](https://ieeexplore.ieee.org/abstract/document/9536374/) | TKDE | 2021 | NA |
| GNNH | [Yu, B., Zhang, R., Chen, W., & Fang, J. (2021). Graph neural network based model for multi-behavior session-based recommendation. _GeoInformatica_, 1-19.](https://link.springer.com/article/10.1007/s10707-021-00439-w) | GeoInformatica | 2021 | NA |

## Recommendation Objectives
### Diversity

| **Name** | **Paper** | **Venue** | **Year** | **Code** |
| --- | --- | --- | --- | --- |
| V2HT | [Li, M., Gan, T., Liu, M., Cheng, Z., Yin, J., & Nie, L. (2019, November). Long-tail hashtag recommendation for micro-videos with graph convolutional network. In _Proceedings of the 28th ACM International Conference on Information and Knowledge Management_ (pp. 509-518).](https://dl.acm.org/doi/abs/10.1145/3357384.3357912) | CIKM | 2019 | NA |
| BGCF | [Sun, J., Guo, W., Zhang, D., Zhang, Y., Regol, F., Hu, Y., ... & Coates, M. (2020, August). A framework for recommending accurate and diverse items using bayesian graph convolutional neural networks. In _Proceedings of the 26th ACM SIGKDD International Conference on Knowledge Discovery & Data Mining_ (pp. 2030-2039).](https://www.researchgate.net/profile/Jianing-Sun-5/publication/343780326_A_Framework_for_Recommending_Accurate_and_Diverse_Items_Using_Bayesian_Graph_Convolutional_Neural_Networks/links/5f85d507299bf1b53e23724f/A-Framework-for-Recommending-Accurate-and-Diverse-Items-Using-Bayesian-Graph-Convolutional-Neural-Networks.pdf) | KDD | 2020 | [Python](https://gitee.com/mindspore/models/tree/master/official/gnn/bgcf) |
| DGCN | [Zheng, Y., Gao, C., Chen, L., Jin, D., & Li, Y. (2021, April). DGCN: Diversified Recommendation with Graph Convolutional Networks. In _Proceedings of the Web Conference 2021_ (pp. 401-412).](https://arxiv.org/pdf/2108.06952.pdf) | WWW | 2021 | [Python](https://github.com/tsinghua-fib-lab/DGCN) |
| FH-HAT | [Xie, R., Liu, Q., Liu, S., Zhang, Z., Cui, P., Zhang, B., & Lin, L. (2021). Improving Accuracy and Diversity in Matching of Recommendation with Diversified Preference Network. arXiv preprint arXiv:2102.03787.](https://arxiv.org/pdf/2102.03787) | TBD | 2021 | NA |
| Isufi _et al._ | [Isufi, E., Pocchiari, M., & Hanjalic, A. (2021). Accuracy-diversity trade-off in recommender systems via graph convolutions. _Information Processing & Management_, _58_(2), 102459.](https://www.sciencedirect.com/science/article/pii/S0306457320309511) | IPM | 2021 | [Python](https://github.com/esilezz/accdiv-via-graphconv) |

### Explainability

| **Name** | **Paper** | **Venue** | **Year** | **Code** |
| --- | --- | --- | --- | --- |
| RippleNet | [Wang, H., Zhang, F., Wang, J., Zhao, M., Li, W., Xie, X., & Guo, M. (2018, October). Ripplenet: Propagating user preferences on the knowledge graph for recommender systems. In _Proceedings of the 27th ACM International Conference on Information and Knowledge Management_ (pp. 417-426).](https://arxiv.org/pdf/1803.03467) | CIKM | 2018 | [Python](https://paperswithcode.com/paper/ripplenet-propagating-user-preferences-on-the) |
| KPRN | [Wang, X., Wang, D., Xu, C., He, X., Cao, Y., & Chua, T. S. (2019, July). Explainable reasoning over knowledge graphs for recommendation. In _Proceedings of the AAAI Conference on Artificial Intelligence_ (Vol. 33, No. 01, pp. 5329-5336).](https://ojs.aaai.org/index.php/AAAI/article/view/4470/4348) | AAAI | 2019 | [Python](https://paperswithcode.com/paper/explainable-reasoning-over-knowledge-graphs) |
| RuleRec | [Ma, W., Zhang, M., Cao, Y., Jin, W., Wang, C., Liu, Y., ... & Ren, X. (2019, May). Jointly learning explainable rules for recommendation with knowledge graph. In _The World Wide Web Conference_ (pp. 1210-1221).](https://arxiv.org/pdf/1903.03714) | WWW | 2019 | [Python](https://github.com/THUIR/RuleRec) |
| KGAT | [Wang, X., He, X., Cao, Y., Liu, M., & Chua, T. S. (2019, July). Kgat: Knowledge graph attention network for recommendation. In _Proceedings of the 25th ACM SIGKDD International Conference on Knowledge Discovery & Data Mining_ (pp. 950-958).](https://arxiv.org/pdf/1905.07854) | KDD | 2019 | [Python](https://paperswithcode.com/paper/kgat-knowledge-graph-attention-network-for) |
| PGPR | [Xian, Y., Fu, Z., Muthukrishnan, S., De Melo, G., & Zhang, Y. (2019, July). Reinforcement knowledge graph reasoning for explainable recommendation. In _Proceedings of the 42nd international ACM SIGIR conference on research and development in information retrieval_ (pp. 285-294).](https://arxiv.org/pdf/1906.05237) | SIGIR | 2019 | [Python](https://github.com/orcax/PGPR) |
| ECFKG | [Bose, A., & Hamilton, W. (2019, May). Compositional fairness constraints for graph embeddings. In _International Conference on Machine Learning_ (pp. 715-724). PMLR.](http://proceedings.mlr.press/v97/bose19a/bose19a.pdf) | ICML | 2019 | [Python](https://github.com/joeybose/Flexible-Fairness-Constraints) |
| EIUM | [Huang, X., Fang, Q., Qian, S., Sang, J., Li, Y., & Xu, C. (2019, October). Explainable interaction-driven user modeling over knowledge graph for sequential recommendation. In _Proceedings of the 27th ACM International Conference on Multimedia_ (pp. 548-556).](https://dl.acm.org/doi/abs/10.1145/3343031.3350893) | MM | 2019 | NA |
| HAGERec | [Yang, Z., & Dong, S. (2020). HAGERec: hierarchical attention graph convolutional network incorporating knowledge graph for explainable recommendation. _Knowledge-Based Systems_, _204_, 106194.](https://www.sciencedirect.com/science/article/pii/S0950705120304196) | KBS | 2020 | NA |
| TMER | [Chen, H., Li, Y., Sun, X., Xu, G., & Yin, H. (2021, March). Temporal meta-path guided explainable recommendation. In _Proceedings of the 14th ACM International Conference on Web Search and Data Mining_ (pp. 1056-1064).](https://arxiv.org/pdf/2101.01433) | WSDM | 2021 | [Python](https://github.com/Abigale001/TMER) |

### Fairness

| **Name** | **Paper** | **Venue** | **Year** | **Code** |
| --- | --- | --- | --- | --- |
| Fairwalk | [Rahman, T., Surma, B., Backes, M., & Zhang, Y. (2019). Fairwalk: Towards fair graph embedding.](https://publications.cispa.saarland/2933/1/IJCAI19.pdf) | IJCAI | 2019 | [Python](https://paperswithcode.com/paper/fairwalk-towards-fair-graph-embedding) |
| CFCGE | [Bose, A., & Hamilton, W. (2019, May). Compositional fairness constraints for graph embeddings. In _International Conference on Machine Learning_ (pp. 715-724). PMLR.](http://proceedings.mlr.press/v97/bose19a/bose19a.pdf) | ICML | 2019 | [Python](https://github.com/joeybose/Flexible-Fairness-Constraints) |
| FairGNN | [Dai, E., & Wang, S. (2021, March). Say no to the discrimination: Learning fair graph neural networks with limited sensitive attribute information. In _Proceedings of the 14th ACM International Conference on Web Search and Data Mining_ (pp. 680-688).](https://arxiv.org/pdf/2009.01454) | WSDM | 2021 | [Python](https://github.com/EnyanDai/FairGNN) |
| FairGo | [Wu, L., Chen, L., Shao, P., Hong, R., Wang, X., & Wang, M. (2021, April). Learning Fair Representations for Recommendation: A Graph-based Perspective. In _Proceedings of the Web Conference 2021_ (pp. 2198-2208).](https://arxiv.org/pdf/2102.09140) | WWW | 2021 | [Python](https://github.com/newlei/FairGo) |


