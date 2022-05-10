# DeltaPapers
Must-read papers on parameter-efficient methods (Delta Tuning) for pre-trained models.

## Content

- [Why Delta Tuning?](#introduction)
- [Keywords Convention](#keywords-convention)
- [Papers](#papers)
  - [Overview](#overview)
  - [Methodology](#methodology)
  - [Analysis](#analysis)
  - [Applications & Tools](#applications-&-tools)
- [Contribution](#contribution)
  - [Contributors](#contributors)
  - [Contributing to this paper list](#contributing-to-this-paper-list)



## Why Parameter Efficient?

Increasingly larger pre-trained models bring both the blessing of effectiveness on existing and unknown tasks, and the curse of prohibitive adaptation cost. In this context, parameter-efficient methods (delta tuning) are developed and demonstrate a promising way to stimulate colossal models with only a small portion of tunable parameters, thereby dramatically reducing the computational and storage costs of model adaptation. In addition to the obvious practical value, delta tuning seems to imply that the particular adaptation of pre-trained models may be a very simple process, which may usher in intriguing theoretical issues that are worth exploring. 


## Keywords Convention

We follow the general idea of [PromptPapers](https://github.com/thunlp/PromptPapers) to label the papers. 

![](https://img.shields.io/badge/T5-blue) The abbreviation of the work.

![](https://img.shields.io/badge/Generation-orange) The main explored task of the work.

![](https://img.shields.io/badge/MultiTask-green) The main explored property of delta tuning methods in the work.

## Papers

### Overview

- **Delta Tuning: A Comprehensive Study of Parameter Efficient Methods for Pre-trained Language Model**, Preprint 2022. ![](https://img.shields.io/badge/Theoretical_Study-green) ![](https://img.shields.io/badge/Empirical_Study-green)

  *Ning Ding, Yujia Qin, Guang Yang, Fuchao Wei, Zonghan Yang, Yusheng Su, Shengding Hu, Yulin Chen, Chi-Min Chan, Weize Chen, Jing Yi, Weilin Zhao, Xiaozhi Wang, Zhiyuan Liu, Hai-Tao Zheng, Jianfei Chen, Yang Liu, Jie Tang, Juanzi Li, Maosong Sun*. [[pdf](https://arxiv.org/abs/2203.06904)], [[OpenDelta](https://github.com/thunlp/OpenDelta)] 

### Methodology

- **Parameter-Efficient Transfer Learning for NLP,** ICML 2019.  ![](https://img.shields.io/badge/Adapter-blue)

  *Neil Houlsby, Andrei Giurgiu, Stanislaw Jastrzebski, Bruna Morrone, Quentin de Laroussilhe, Andrea Gesmundo, Mona Attariyan, Sylvain Gelly.* [[pdf](https://arxiv.org/abs/1902.00751)], [[Project](https://github.com/google-research/adapter-bert)]

- **Prefix-Tuning: Optimizing Continuous Prompts for Generation,** ACL 2021. ![](https://img.shields.io/badge/Prefix_Tuning-blue) ![](https://img.shields.io/badge/Generation-orange)

  *Xiang Lisa Li, Percy Liang.* [[pdf](https://arxiv.org/abs/2101.00190)], [[Project]()]

- **Parameter-Efficient Transfer Learning with Diff Pruning,** ACL 2021. ![](https://img.shields.io/badge/Diff_pruning-blue)

  *Demi Guo, Alexander M. Rush, Yoon Kim*. [[pdf](https://arxiv.org/abs/2012.07463)], [[Project](https://github.com/dguo98/DiffPruning)]

- **The Power of Scale for Parameter-Efficient Prompt Tuning,** EMNLP 2021. ![](https://img.shields.io/badge/Prompt_Tuning-blue)

  *Brian Lester, Rami Al-Rfou, Noah Constant.* [[pdf](https://arxiv.org/abs/2104.08691)], [[OpenPrompt Implementation](https://github.com/thunlp/OpenPrompt/blob/main/tutorial/1.4_soft_template.py)]

- **COMPACTER: Efficient Low-Rank Hypercomplex Adapter Layers,** Neurips 2021.![](https://img.shields.io/badge/Compacter-blue)

  *Rabeeh Karimi Mahabadi, James Henderson, Sebastian Ruder*. [[pdf](https://arxiv.org/abs/2106.04647)], [[Project](https://github.com/rabeehk/compacter)]

- **Masking as an Efficient Alternative to Finetuning for Pretrained Language Models,** EMNLP 2020. ![](https://img.shields.io/badge/Masking-blue)

  *Mengjie Zhao, Tao Lin, Fei Mi, Martin Jaggi, Hinrich Schütze*. [[pdf](https://arxiv.org/abs/2004.12406)], [[Project](https://github.com/ptlmasking/maskbert)] 

- **BitFit: Simple Parameter-efficient Fine-tuning for Transformer-based Masked Language-models,** Preprint 2021. ![](https://img.shields.io/badge/BitFit-blue)

  *Elad Ben Zaken, Shauli Ravfogel, Yoav Goldberg*. [[pdf](https://arxiv.org/abs/2106.10199)], [[Project](https://github.com/benzakenelad/BitFit)]

- **LoRA: Low-Rank Adaptation of Large Language Models,** ICLR 2022. ![](https://img.shields.io/badge/LoRA-blue)

  *Edward J. Hu, Yelong Shen, Phillip Wallis, Zeyuan Allen-Zhu, Yuanzhi Li, Shean Wang, Lu Wang, Weizhu Chen.* [[pdf](https://arxiv.org/abs/2106.09685)], [[Project](https://github.com/microsoft/LoRA)]

- **Fast Model Editing at Scale,** ICLR 2022. ![](https://img.shields.io/badge/MEND-blue) ![](https://img.shields.io/badge/Knowledge_Editing-green)

  *Eric Mitchell, Charles Lin, Antoine Bosselut, Chelsea Finn, Christopher D. Manning*. [[pdf](https://arxiv.org/abs/2110.11309)], [[Project](https://github.com/eric-mitchell/mend)]

- **Editing Factual Knowledge in Language Models,** EMNLP 2021

  *Nicola De Cao, Wilker Aziz, Ivan Titov*. [[pdf](https://arxiv.org/abs/2104.08164)], [[Project](https://github.com/nicola-decao/KnowledgeEditor)]

- **Training Neural Networks with Fixed Sparse Masks,** Neurips 2021.

  *Yi-Lin Sung, Varun Nair, Colin Raffeln*. [[pdf](https://arxiv.org/abs/2111.09839)], [[Project](https://github.com/varunnair18/FISH)]

- **GPT Understands, Too,** Preprint 2020. ![](https://img.shields.io/badge/P_Tuning-blue)

  *Xiao Liu, Yanan Zheng, Zhengxiao Du, Ming Ding, Yujie Qian, Zhilin Yang, Jie Tang*. [[pdf](https://arxiv.org/abs/2103.10385)], [[Project](https://github.com/THUDM/P-tuning)]

- **LiST: Lite Self-training Makes Efficient Few-shot Learners,** Preprint 2021.

  *Yaqing Wang, Subhabrata Mukherjee, Xiaodong Liu, Jing Gao, Ahmed Hassan Awadallah, Jianfeng Gao*. [[pdf](https://arxiv.org/abs/2110.06274)], [[Project](https://github.com/microsoft/LiST)]

- **Parameter-efficient Multi-task Fine-tuning for Transformers via Shared Hypernetworks,** ACL 2021.

  *Rabeeh Karimi Mahabadi, Sebastian Ruder, Mostafa Dehghani, James Henderson*. [[pdf](https://arxiv.org/abs/2106.04489)], [[Project](https://github.com/rabeehk/hyperformer)]

- **BERT and PALs: Projected Attention Layers for Efficient Adaptation in Multi-Task,** ICML 2019.

  *Asa Cooper Stickland, Iain Murray*. [[pdf](https://arxiv.org/abs/1902.02671)], [[Project](https://github.com/AsaCooperStickland/Bert-n-Pals)]

### Analysis 

- **Towards a Unified View of Parameter-Efficient Transfer Learning,** ICLR 2022. ![](https://img.shields.io/badge/Unified_View-green)

  *Junxian He, Chunting Zhou, Xuezhe Ma, Taylor Berg-Kirkpatrick, Graham Neubig.* [[pdf](https://arxiv.org/abs/2110.04366)], [[Project](https://github.com/jxhe/unify-parameter-efficient-tuning)]

- **AdapterBias: Parameter-efficient Token-dependent Embedding Shift for Adapters in NLP Tasks,** Preprint 2021.

  *Anonymous*. [[pdf](https://openreview.net/forum?id=VZ2oO6KYbBB)]

- **AdapterFusion: Non-Destructive Task Composition for Transfer Learning,** Preprint 2020. ![](https://img.shields.io/badge/MultiTask-green)

  *Jonas Pfeiffer, Aishwarya Kamath, Andreas Rücklé, Kyunghyun Cho, Iryna Gurevych*. [[pdf](https://arxiv.org/abs/2005.00247)], [[Project](https://adapterhub.ml/)]

- **On the Effectiveness Adapter-based Tuning for Pretrained Language Model Adaptation,** ACL 2021.

  *Ruidan He, Linlin Liu, Hai Ye, Qingyu Tan, Bosheng Ding, Liying Cheng, Jia-Wei Low, Lidong Bing, Luo Si*. [[pdf](https://arxiv.org/abs/2106.03164)]

- **UNIPELT: A Unified Framework for Parameter-Efficient Language Model Tuning,** Preprint 2021. ![](https://img.shields.io/badge/Unified_View-green)

  *Yuning Mao, Lambert Mathias, Rui Hou, Amjad Almahairi, Hao Ma, Jiawei Han, Wen-tau Yih, Madian Khabsa*. [[pdf](https://arxiv.org/abs/2110.07577)], [[Project](https://github.com/morningmoni/UniPELT)]

- **Conditionally Adaptive Multi-Task Learning: Improving Transfer Learning in NLP Using Fewer Parameters & Less Data,** ICLR 2021.

  *Jonathan Pilault, Amine Elhattami, Christopher Pal*. [[pdf](https://arxiv.org/abs/2009.09139)], [[Project](https://github.com/CAMTL/CA-MTL)]

- **Raise a Child in Large Language Model: Towards Effective and Generalizable Fine-tuning,** EMNLP 2021.

  *Runxin Xu, Fuli Luo, Zhiyuan Zhang, Chuanqi Tan, Baobao Chang, Songfang Huang, Fei Huang*. [[pdf](https://arxiv.org/abs/2109.05687)], [[Project](https://github.com/alibaba/AliceMind/tree/main/ChildTuning)]

- **Exploring Low-dimensional Intrinsic Task Subspace via Prompt Tuning,** Preprint 2021. ![](https://img.shields.io/badge/Intrinsic_Space-green)

  *Yujia Qin, Xiaozhi Wang, Yusheng Su, Yankai Lin, Ning Ding, Zhiyuan Liu, Juanzi Li, Lei Hou, Peng Li, Maosong Sun, Jie Zhou*. [[pdf](https://arxiv.org/abs/2110.07867)], [[Project](https://github.com/thunlp/Intrinsic-Prompt-Tuning)]

- **Intrinsic Dimensionality Explains the Effectiveness of Language Model Fine-Tuning,** ACL 2021. ![](https://img.shields.io/badge/Intrinsic_Space-green)

  *Armen Aghajanyan, Luke Zettlemoyer, Sonal Gupta*. [[pdf](https://arxiv.org/abs/2012.13255)]

- **Enabling Lightweight Fine-tuning for Pre-trained Language Model Compression based on Matrix Product Operators,** ACL 2021.

  *Peiyu Liu, Ze-Feng Gao, Wayne Xin Zhao, Z.Y. Xie, Zhong-Yi Lu, Ji-Rong Wen*. [[pdf](https://arxiv.org/abs/2106.02205)], [[Project](https://github.com/RUCAIBox/MPOP)]

- **Movement Pruning: Adaptive Sparsity by Fine-Tuning,** Neurips 2020.

  *Victor Sanh, Thomas Wolf, Alexander M. Rush*. [[pdf](https://arxiv.org/abs/2005.07683)], [[Project](https://github.com/huggingface/block_movement_pruning)]

- **Beyond Fully-Connected Layers with Quaternions: Parameterization of Hypercomplex Multiplications with 1/n Parameters,** ICLR 2021.

  *Aston Zhang, Yi Tay, Shuai Zhang, Alvin Chan, Anh Tuan Luu, Siu Cheung Hui, Jie Fu*. [[pdf](https://arxiv.org/abs/2102.08597)]

- **Shapeshifter: a Parameter-efficient Transformer using Factorized Reshaped Matrices,** Neurips 2021.

  *Aliakbar Panahi, Seyran Saeedi, Tom Arodz*. [[pdf](https://proceedings.neurips.cc/paper/2021/file/09def3ebbc44ff3426b28fcd88c83554-Paper.pdf)], [[Project](https://github.com/tarodz/shapeshifter)]

- **Adapterdrop: On the efficiency of adapters in transformers,** EMNLP 2021.

  *Andreas Rücklé, Gregor Geigle, Max Glockner, Tilman Beck, Jonas Pfeiffer, Nils Reimers, Iryna Gurevych*. [[pdf](https://arxiv.org/abs/2010.11918)]

  ​



### Applications & Tools

- **Lightweight Adapter Tuning for Multilingual Speech Translation,** ACL 2021. ![](https://img.shields.io/badge/Speech-orange)

  *Hang Le, Juan Pino, Changhan Wang, Jiatao Gu, Didier Schwab, Laurent Besacier*. [[pdf](https://arxiv.org/abs/2106.01463)], [[Project](https://github.com/formiel/fairseq/blob/master/examples/speech_to_text/docs/adapters.md)]

- **VL-ADAPTER: Parameter-Efficient Transfer Learning for Vision-and-Language Tasks,** CVPR 2022. ![](https://img.shields.io/badge/Vision-orange)

  *Yi-Lin Sung, Jaemin Cho, Mohit Bansal*. [[pdf](https://arxiv.org/abs/2112.06825)], [[Project](https://github.com/ylsung/VL_adapter)]

- **AdapterHub: A Framework for Adapting Transformers,** EMNLP demo 2020. ![](https://img.shields.io/badge/Adapter_Tool-green)

  *Jonas Pfeiffer, Andreas Rücklé, Clifton Poth, Aishwarya Kamath, Ivan Vulić, Sebastian Ruder, Kyunghyun Cho, Iryna Gurevych.* [[pdf](https://arxiv.org/abs/2007.07779)], [[Project](https://adapterhub.ml/)]



## Contribution

### Contributors

<!-- Copy-paste in your Readme.md file -->

<a href="https://github.com/thunlp/OpenPrompt/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=thunlp/DeltaPapers" />
</a>

### Contributing to this paper list

-  First, think about which category the work should belong to. 
-  Second, use the same format as the others to describe the work. Note that there should be an empty line between the title and the author's list, and take care of the indentation.
-  Then, add [keywords tags](#keywords-convention). Add the pdf link of the paper. If it is an arxiv publication, we prefer /abs/ format to /pdf/ format.
