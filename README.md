# Awesome Video Diffusions [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of latest research papers, projects and resources related to Video Diffusion Models and Video Generation. Content is automatically updated daily.

> Last Update: 2026-05-28 03:38:10

## 📰 Latest Updates

🚀 **[2026-02] Project Launched — v1.0**
- Adapted from [awesome-gaussians](https://github.com/limingwei/awesome-gaussians) framework for tracking video diffusion research
- **Unified CLI**: Single entry point `python main.py` with subcommands: `init`, `search`, `suggest`, `export-bib`, `readme`
- **Interactive Configuration Wizard**: Run `python main.py init` to set up keywords, domains, time range, and API keys step-by-step
- **Custom Time Range Filtering**: Support relative periods (`6m`, `1y`, `2y`) and absolute date ranges
- **Smart Link Extraction**: Automatically extracts and classifies GitHub, project page, dataset, video, demo, and HuggingFace links from paper abstracts
- **BibTeX Export**: Fetch BibTeX from arXiv and export to `.bib` files with category/date filters
- **LLM Keyword Suggestion**: Paste a few paper titles or arXiv IDs, and an LLM automatically generates optimized search keywords
- **arXiv Domain Filtering**: Restrict searches to specific arXiv categories (e.g., `cs.CV`, `cs.AI`, `cs.MM`)
- **16 Research Categories**: Comprehensive taxonomy covering T2V, I2V, video editing, controllable generation, world models, and more

- View detailed updates: [News.md](News.md) 📋

---

## Categories

- [3D-aware Video Generation](#3d-aware-video-generation) (16 papers) - Video generation with 3D awareness, multi-view consistency, and 4D content creation
- [Applications](#applications) (56 papers) - Domain-specific applications of video diffusion models
- [Architecture & Efficiency](#architecture-&-efficiency) (362 papers) - Architectural innovations (DiT, UNet), flow matching, and training/inference efficiency
- [Audio & Multi-modal](#audio-&-multi-modal) (32 papers) - Audio-driven and multi-modal conditioned video generation
- [Controllable Generation](#controllable-generation) (130 papers) - Controllable video generation with motion, camera, pose, or layout guidance
- [Human & Character Animation](#human-&-character-animation) (24 papers) - Human-centric video generation including talking heads, dance, and character animation
- [Image-to-Video Generation](#image-to-video-generation) (41 papers) - Methods for animating still images into videos
- [Long Video Generation](#long-video-generation) (125 papers) - Generating temporally consistent long-form videos beyond short clips
- [Personalization & Customization](#personalization-&-customization) (83 papers) - Personalized video generation with custom subjects, identities, or styles
- [Physical Understanding](#physical-understanding) (153 papers) - Physics-aware video generation and dynamics modeling
- [Surveys & Benchmarks](#surveys-&-benchmarks) (231 papers) - Survey papers, benchmarks, and evaluation metrics for video generation
- [Text-to-Video Generation](#text-to-video-generation) (47 papers) - Foundation models and methods for generating videos from text prompts
- [Video Editing](#video-editing) (33 papers) - Diffusion-based video editing, style transfer, and manipulation
- [Video Inpainting & Completion](#video-inpainting-&-completion) (10 papers) - Video inpainting, completion, outpainting, and temporal prediction
- [Video Super-Resolution & Enhancement](#video-super-resolution-&-enhancement) (65 papers) - Video quality improvement, upscaling, restoration, and frame interpolation
- [World Models & Simulation](#world-models-&-simulation) (122 papers) - Video generation as world simulators and interactive environment generation



## Table of Contents

- [Categorized Papers](#categorized-papers)
- [Classic Papers](#classic-papers)
- [Open Source Projects](#open-source-projects)
- [Applications](#applications)
- [Tutorials & Blogs](#tutorials--blogs)





## Categorized Papers

### 3D-aware Video Generation

- **[Full-4D: Generating Full-Scope 4D Scenes from a Single-View Video](https://arxiv.org/abs/2605.25500v1)**  
  Authors: Tingxi Chen, Ke Hao, Yabo Chen, Zhengxue Cheng, Rong Xie, Li Song, Haibin Huang, Chi Zhang, Xuelong Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25500v1.pdf)  
  Keywords: distillation, 4d generation, flow matching, video synthesis, interactive, multi-view video, diffusion model, video diffusion, dit, video interpolation, physical  
- **[Pantheon360: Taming Digital Twin Generation via 3D-Aware 360° Video Diffusion](https://arxiv.org/abs/2605.25449v1)**  
  Authors: Ting-Hsuan Chen, Ying-Huan Chen, Tao Tu, Jie-Ying Lee, Cho-Ying Wu, Fangzhou Lin, Hengyuan Zhang, David Paz, Xinyu Huang, Yuliang Guo, Yu-Lun Liu, Yue Wang, Liu Ren  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25449v1.pdf)  
  Keywords: controllable, temporal consistency, camera control, 3d-aware, trajectory, diffusion model, video generation, video diffusion, simulation  
- **[SRUG: Shadow-Guided Relightable Urban Scene with Generation Model](https://arxiv.org/abs/2605.24700v1)**  
  Authors: Yonghao Zhao, Zexin Yin, Jian Yang, Beibei Wang, Jin Xie  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.24700v1.pdf)  
  Keywords: evaluation, novel view, dit, physical  
- **[3DPhysVideo: Consistency-Guided Flow SDE for Video Generation via 3D Scene Reconstruction and Physical Simulation](https://arxiv.org/abs/2605.16795v1)**  
  Authors: Hwidong Kim, Yunho Kim, Tae-Kyun Kim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.16795v1.pdf)  
  Keywords: dynamics, benchmark, denoising, video generation, image-to-video, evaluation, physics, physical simulation, dit, efficient, i2v, novel view, simulation, physical  
- **[GTA: Advancing Image-to-3D World Generation via Geometry Then Appearance Video Diffusion](https://arxiv.org/abs/2605.12957v1)**  
  Authors: Hanxin Zhu, Cong Wang, Peiyan Tu, Jiayi Luo, Tianyu He, Xin Jin, Zhibo Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.12957v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://hanxinzhu-lab.github.io/GTA)  
  Keywords: diffusion model, autonomous driving, video diffusion, novel view, dit  
- **[GaitProtector: Impersonation-Driven Gait De-Identification via Training-Free Diffusion Latent Optimization](https://arxiv.org/abs/2605.12431v1)**  
  Authors: Huiran Duan, Qian Zhou, Zhongliang Guo, Junhao Dong, Yuqi Li, Guoying Zhao, Yingli Tian  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.12431v1.pdf)  
  Keywords: identity, trajectory, diffusion model, 3d video, video diffusion, dynamics  
- **[VidSplat: Gaussian Splatting Reconstruction with Geometry-Guided Video Diffusion Priors](https://arxiv.org/abs/2605.11424v1)**  
  Authors: Jimin Tang, Wenyuan Zhang, Junsheng Zhou, Zian Huang, Kanle Shi, Shenkun Xu, Yu-Shen Liu, Zhizhong Han  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.11424v1.pdf)  
  Keywords: 3d consistent, benchmark, denoising, video diffusion, novel view  
- **[LoViF 2026 The First Challenge on Holistic Quality Assessment for 4D World Model (PhyScore)](https://arxiv.org/abs/2605.05187v1)**  
  Authors: Wei Luo, Yiting Lu, Xin Li, Haoran Li, Fengbin Guan, Chen Gao, Xin Jin, Yong Li, Zhibo Chen, Sijing Wu, Kang Fu, Yunhao Li, Ziang Xiao, Huiyu Duan, Jing Liu, Qiang Hu, Xiongkuo Min, Guangtao Zhai, Manxi Sun, Zixuan Guo, Yun Li, Ziyang Chen, Manabu Tsukada, Zhengyang Li, Zhenglin Du, Yi Wen, Licheng Jiao, Fang Liu, Lingling Li, Yiwen Ren, Zhilong Song, Dubing Chen, Yucheng Zhou, Tianyi Yan, Huan Zheng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.05187v1.pdf)  
  Keywords: 4d generation, temporal consistency, world model, dynamics, benchmark, creative, evaluation, physics, dit, physical  
- **[AnyRecon: Arbitrary-View 3D Reconstruction with Video Diffusion Model](https://arxiv.org/abs/2604.19747v1)**  
  Authors: Yutian Chen, Shi Guo, Renbiao Jin, Tianshuo Yang, Xin Cai, Yawen Luo, Mingxin Yang, Mulin Yu, Linning Xu, Tianfan Xue  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2604.19747v1.pdf)  
  Keywords: distillation, diffusion model, video diffusion, novel view, dit  
- **[MultiWorld: Scalable Multi-Agent Multi-View Video World Models](https://arxiv.org/abs/2604.18564v2)**  
  Authors: Haoyu Wu, Jiwen Yu, Yingtian Zou, Xihui Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2604.18564v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://multi-world.github.io)  
  Keywords: world model, dynamics, multi-view video, video generation, dit, action-conditioned  

### Applications

*Showing the latest 50 out of 56 papers*

- **[DriveWAM: Video Generative Priors Enable Scalable World-Action Modeling for Autonomous Driving](https://arxiv.org/abs/2605.28544v1)**  
  Authors: Chen Shi, Jinrui Xu, Shaoshuai Shi, Kehua Sheng, Bo Zhang, Li Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28544v1.pdf)  
  Keywords: diffusion transformer, autoregressive, architecture, benchmark, autonomous driving, video diffusion, dynamics, physical  
- **[Turning Video Models into Generalist Robot Policies](https://arxiv.org/abs/2605.27817v1)**  
  Authors: Sizhe Lester Li, Evan Kim, Xingjian Bai, Tong Zhao, Tao Pang, Max Simchowitz, Vincent Sitzmann  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.27817v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://vera.csail.mit.edu)  
  Keywords: world model, benchmark, efficient, robotics, dynamics  
- **[AnyScene: Towards Highly Controllable Driving Scene Generation at Anywhere and Beyond](https://arxiv.org/abs/2605.26113v1)**  
  Authors: Haiming Zhang, Junfei Zhou, Feng Jiang, Jingzhong Li, Zhenglong Guo, Penglin Dai, Jifeng Dai, Yan Xie, Benjin Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.26113v1.pdf)  
  Keywords: controllable, diffusion transformer, autoregressive, video synthesis, video generation, layout, autonomous driving, dit, simulation  
- **[DexSIM: Real-time Dexterous Simulation with Unified Causal Video Diffusion](https://arxiv.org/abs/2605.24630v1)**  
  Authors: Adam Lee  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.24630v1.pdf)  
  Keywords: autoregressive, trajectory, interactive, diffusion model, video diffusion, robotics, simulation, physical  
- **[EvalVerse: Pipeline-Aware and Expert-Calibrated Benchmarking for Professional Cinematic Video Generation](https://arxiv.org/abs/2605.23271v1)**  
  Authors: Songlin Yang, Haobin Zhong, Ruilin Zhang, Xiaotong Zhao, Shuai Li, Kai Zheng, Xuyi Yang, Zhe Wang, Zhenchen Tang, Yang Li, Bohai Gu, Zhengwei Peng, Yidan Huang, Mengzhou Luo, Yihang Bo, Dalu Feng, Yujia Zhang, Juntao Ma, Ruiqi Wang, Lvmin Zhang, Yuwei Guo, Frank Guan, Maneesh Agrawala, Hongbo Fu, Alan Zhao, Anyi Rao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.23271v1.pdf)  
  Keywords: evaluation, film, benchmark, video generation  
- **[Cell Phantom Video Generation in Elliptical Fourier Descriptor Domain](https://arxiv.org/abs/2605.22563v1)**  
  Authors: Francesco Benedetto, Roberto Basla, Luca Magri, Giacomo Boracchi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.22563v1.pdf) | [![GitHub](https://img.shields.io/github/stars/FrancescoBenedetto99/efd-cell-video-gen?style=social)](https://github.com/FrancescoBenedetto99/efd-cell-video-gen)  
  Keywords: efficient, medical, video generation  
- **[CogOmniControl: Reasoning-Driven Controllable Video Generation via Creative Intent Cognition](https://arxiv.org/abs/2605.19995v1)**  
  Authors: Hongji Yang, Songlian Li, Yucheng Zhou, Xiaotong Zhao, Alan Zhao, Chengzhong Xu, Jianbing Shen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.19995v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://um-lab.github.io/CogOmniControl)  
  Keywords: controllable, benchmark, architecture, creative, video generation, diffusion model, dit  
- **[CodeBind: Decoupled Representation Learning for Multimodal Alignment with Unified Compositional Codebook](https://arxiv.org/abs/2605.18257v1)**  
  Authors: Zeyu Chen, Jie Li, Kai Han  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.18257v1.pdf)  
  Keywords: robotics, dit  
- **[Xiaomi Auto World Model: A Joint World Model Integrating Reconstruction and Generation for Autonomous Driving](https://arxiv.org/abs/2605.18137v5)**  
  Authors: Lijun Zhou, Hongcheng Luo, Zhenxin Zhu, Cheng Chi, Mingfei Tu, Kaixin Xiong, Lei Gong, Zhanqian Wu, Zehan Zhang, Fangzhen Li, Hao Li, Yingying Shen, Jiale He, Haohui Zhu, Shan Zhao, Kai Wang, Zhiwei Zhan, Yuechuan Pu, Kaiyuan Tan, Ruiling Yang, Xianqi Wang, Tianyi Yan, Jiawei Zhou, Lei Zhang, Jingyang Zhao, Xi Zhou, Chitian Sun, Chenming Wu, Jiong Deng, Hongwei Xie, Ming Lu, Kun Ma, Long Chen, Guang Chen, Hangjun Ye, Bing Wang, Haiyang Sun  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.18137v5.pdf)  
  Keywords: distillation, world model, architecture, denoising, video generation, autonomous driving, simulation  
- **[Soap2Soap: Long Cinematic Video Remaking via Multi-Agent Collaboration](https://arxiv.org/abs/2605.17423v1)**  
  Authors: Yiren Song, Huilin Zhong, Kevin Qinghong Lin, Haofan Wang, Mike Zheng Shou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.17423v1.pdf)  
  Keywords: identity, video synthesis, video generation, video-to-video, dit, film  

### Architecture & Efficiency

*Showing the latest 50 out of 362 papers*

- **[Gamma-World: Generative Multi-Agent World Modeling Beyond Two Players](https://arxiv.org/abs/2605.28816v1)**  
  Authors: Fangfu Liu, Kai He, Tianchang Shen, Tianshi Cao, Sanja Fidler, Yueqi Duan, Jun Gao, Igor Gilitschenski, Zian Wang, Xuanchi Ren  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28816v1.pdf)  
  Keywords: controllable, world model, identity, interactive, video generation, dit, efficient, simulation  
- **[HarmoVid: Relightful Video Portrait Harmonization](https://arxiv.org/abs/2605.28811v1)**  
  Authors: Jun Myeong Choi, Jae Shin Yoon, Luchao Qi, Roni Sengupta, Joon-Young Lee  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28811v1.pdf)  
  Keywords: physical, dit, diffusion model, video diffusion  
- **[OSP-Next: Efficient High-Quality Video Generation with Sparse Sequence Parallelism, HiF8 Quantization, and Reinforcement Learning](https://arxiv.org/abs/2605.28691v1)**  
  Authors: Yunyang Ge, Xianyi He, Zezhong Zhang, Bin Lin, Bin Zhu, Xinhua Cheng, Li Yuan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28691v1.pdf)  
  Keywords: diffusion transformer, architecture, video generation, text-to-video, efficient, dit  
- **[DriveWAM: Video Generative Priors Enable Scalable World-Action Modeling for Autonomous Driving](https://arxiv.org/abs/2605.28544v1)**  
  Authors: Chen Shi, Jinrui Xu, Shaoshuai Shi, Kehua Sheng, Bo Zhang, Li Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28544v1.pdf)  
  Keywords: diffusion transformer, autoregressive, architecture, benchmark, autonomous driving, video diffusion, dynamics, physical  
- **[Sketch2Motion: Text-driven 2D Sketch to 3D Animation via Diffusion-guided Skeleton Optimization](https://arxiv.org/abs/2605.28394v1)**  
  Authors: Gaurav Rai, Ojaswa Sharma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28394v1.pdf)  
  Keywords: distillation, diffusion model, text-to-video, physics, video diffusion, dit, physical  
- **[VidPrism: Heterogeneous Mixture of Experts for Image-to-Video Transfer](https://arxiv.org/abs/2605.28229v1)**  
  Authors: Rui Lin, Chuanming Wang, Huadong Ma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28229v1.pdf) | [![GitHub](https://img.shields.io/github/stars/Lrrrr549/VidPrism.git?style=social)](https://github.com/Lrrrr549/VidPrism.git)  
  Keywords: efficient, benchmark, image-to-video  
- **[Refining Multidimensional Video Reward Models via Disentangled Influence Functions](https://arxiv.org/abs/2605.28203v1)**  
  Authors: Muyao Wang, Zeke Xie, Hideki Nakayama  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28203v1.pdf)  
  Keywords: evaluation, text-to-video, efficient, t2v  
- **[CogPortrait: Fine-Grained Eye-Region Control in Portrait Animation via Hierarchical Agent Planning](https://arxiv.org/abs/2605.28056v1)**  
  Authors: He Feng, Yongjia Ma, Donglin Di, Lei Fan, Tonghua Su  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28056v1.pdf)  
  Keywords: dynamics, benchmark, identity, video generation, motion control, dit  
- **[VCap: Hypergeometric Rewards for Weak-to-Strong Visual Captioning](https://arxiv.org/abs/2605.28023v1)**  
  Authors: Xingyu Lu, Jinpeng Wang, Yi-Fan Zhang, Yankai Yang, Yancheng Long, Yiyang Fan, Xuanyu Zheng, Haonan Fan, Kaiyu Jiang, Tianke Zhang, Changyi Liu, Bin Wen, Fan Yang, Tingting Gao, Han Li, Chun Yuan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28023v1.pdf)  
  Keywords: evaluation, dit, benchmark, distillation  
- **[SmartDirector: Keyframe-Conditioned Cinematic Video Generation with Narrative Pacing Control](https://arxiv.org/abs/2605.27891v1)**  
  Authors: Zhida Zhang, Jie Ma, Zhan Peng, Haoxue Wu, Yang Han, Jun Liang, Jie Cao, Jing Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.27891v1.pdf)  
  Keywords: dit, video generation  

### Audio & Multi-modal

- **[LongCat-Video-Avatar 1.5 Technical Report](https://arxiv.org/abs/2605.26486v1)**  
  Authors: Meituan LongCat Team, Xunliang Cai, Meng Cheng, Feng Gao, Zhe Kong, Jiamu Li, Le Li, Weiheng Li, Hongyu Liu, Shuai Tan, Xiaoming Wei, Tianyu Yang, Yong Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.26486v1.pdf)  
  Keywords: distillation, benchmark, identity, video generation, evaluation, avatar, audio-driven, dit  
- **[StreamChar: Long-Horizon Streaming Character Audio-Video Generation with Decoupled Orchestration](https://arxiv.org/abs/2605.25659v1)**  
  Authors: Linrui Tian, Qi Wang, Bang Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25659v1.pdf)  
  Keywords: distillation, autoregressive, denoising, identity, video generation, streaming, efficient, audio-driven, dit  
- **[Test-Time Self-Adaptive Conditioning for Stable Audio-Driven Talking-Head Generation](https://arxiv.org/abs/2605.25488v1)**  
  Authors: Zhicheng Zhang, Lei Wang, Yu Zhang, Yongsheng Gao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25488v1.pdf)  
  Keywords: dynamics, benchmark, identity, video generation, audio-driven, dit  
- **[AVBench: Human-Aligned and Automated Evaluation Benchmark for Audio-Video Generative Models](https://arxiv.org/abs/2605.24652v1)**  
  Authors: Jialiang Yang, Bin Xia, Ruihang Chu, Dingdong Wang, Wanke Xia, Zhun Mou, Tianyang Zhong, Yiting Zhao, Wenming Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.24652v1.pdf)  
  Keywords: benchmark, sound, evaluation, style, dit  
- **[What Semantics Survive the Connector? Diagnosing VLM-to-DiT Alignment in Video Editing](https://arxiv.org/abs/2605.20795v1)**  
  Authors: Hangyu Lin, Chao Wen, Chengming Xu, Jianxiong Gao, Jiangning Zhang, Xiaobin Hu, Yanwei Fu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20795v1.pdf)  
  Keywords: video editing, architecture, multi-modal, flow matching, evaluation, dit  
- **[Sound Sparks Motion: Audio and Text Tuning for Video Editing](https://arxiv.org/abs/2605.15307v1)**  
  Authors: AmirHossein Naghi Razlighi, Aryan Mikaeili, Ali Mahdavi-Amiri, Daniel Cohen-Or, Yiorgos Chrysanthou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.15307v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://amirhossein-razlighi.github.io/Sound_Sparks_Motion)  
  Keywords: video editing, sound, video generation, motion control, dit  
- **[OmniNFT: Modality-wise Omni Diffusion Reinforcement for Joint Audio-Video Generation](https://arxiv.org/abs/2605.12480v1)**  
  Authors: Guohui Zhang, XiaoXiao Ma, Jie Huang, Hang Xu, Hu Yu, Siming Fu, Yuming Li, Zeyue Xue, Lin Song, Haoyang Huang, Nan Duan, Feng Zhao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.12480v1.pdf)  
  Keywords: efficient, multi-modal, dit, video generation  
- **[AllocMV: Optimal Resource Allocation for Music Video Generation via Structured Persistent State](https://arxiv.org/abs/2605.10723v1)**  
  Authors: Huimin Wang, Leilei Ouyang, Chang Xia, Yongqi Kang, Yu Fu, Yuqi Ouyang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.10723v1.pdf)  
  Keywords: video synthesis, music video, dit, video generation  
- **[Omni-DeepSearch: A Benchmark for Audio-Driven Omni-Modal Deep Search](https://arxiv.org/abs/2605.08762v1)**  
  Authors: Tao Yu, yiming ding, Shenghua Chai, Minghui Zhang, Zhongtian Luo, Xinming Wang, Xinlong Chen, Zhaolu Kang, Junhao Gong, Yuxuan Zhou, Haopeng Jin, Zhiqing Cui, Jiabing Yang, YiFan Zhang, Hongzhu Yi, Zheqi He, Xi Yang, Yan Huang, Liang Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.08762v1.pdf)  
  Keywords: audio-driven, benchmark  
- **[Unison: Harmonizing Motion, Speech, and Sound for Human-Centric Audio-Video Generation](https://arxiv.org/abs/2605.08729v1)**  
  Authors: Shihao Cheng, Jiaxu Zhang, Quanyue Song, Shansong Liu, Zhizhi Guo, Xiaolei Zhang, Chi Zhang, Xuelong Li, Zhigang Tu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.08729v1.pdf)  
  Keywords: sound, dit, video generation, denoising  

### Controllable Generation

*Showing the latest 50 out of 130 papers*

- **[Gamma-World: Generative Multi-Agent World Modeling Beyond Two Players](https://arxiv.org/abs/2605.28816v1)**  
  Authors: Fangfu Liu, Kai He, Tianchang Shen, Tianshi Cao, Sanja Fidler, Yueqi Duan, Jun Gao, Igor Gilitschenski, Zian Wang, Xuanchi Ren  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28816v1.pdf)  
  Keywords: controllable, world model, identity, interactive, video generation, dit, efficient, simulation  
- **[CogPortrait: Fine-Grained Eye-Region Control in Portrait Animation via Hierarchical Agent Planning](https://arxiv.org/abs/2605.28056v1)**  
  Authors: He Feng, Yongjia Ma, Donglin Di, Lei Fan, Tonghua Su  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28056v1.pdf)  
  Keywords: dynamics, benchmark, identity, video generation, motion control, dit  
- **[Timestep-Aware SVDQuant-GPTQ for W4A4 Quantization of Wan2.2-I2V](https://arxiv.org/abs/2605.27003v1)**  
  Authors: Junhao Wu, Dezhong Yao, Hai Jin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.27003v1.pdf)  
  Keywords: diffusion transformer, benchmark, denoising, trajectory, video diffusion, i2v, dit  
- **[E$^3$C: Video Generation with 3D Environmental Memory and Ego-Exo Human Pose Control](https://arxiv.org/abs/2605.26316v1)**  
  Authors: Qiao Gu, Lingni Ma, Adam W Harley, Richard Newcombe, Florian Shkurti, Julian Straub  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.26316v1.pdf)  
  Keywords: controllable, dynamics, video synthesis, video generation, video diffusion, dit, physical  
- **[AnyScene: Towards Highly Controllable Driving Scene Generation at Anywhere and Beyond](https://arxiv.org/abs/2605.26113v1)**  
  Authors: Haiming Zhang, Junfei Zhou, Feng Jiang, Jingzhong Li, Zhenglong Guo, Penglin Dai, Jifeng Dai, Yan Xie, Benjin Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.26113v1.pdf)  
  Keywords: controllable, diffusion transformer, autoregressive, video synthesis, video generation, layout, autonomous driving, dit, simulation  
- **[PixelWizard: Towards Efficient High-Fidelity Video Generation at Ultra-Large Spatial Resolution](https://arxiv.org/abs/2605.25801v1)**  
  Authors: Wenxue Li, Jingjing Ren, Peng Zhang, Tian Ye, Daiguo Zhou, Jian Luan, Lei Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25801v1.pdf)  
  Keywords: distillation, efficient, trajectory, video generation  
- **[Pantheon360: Taming Digital Twin Generation via 3D-Aware 360° Video Diffusion](https://arxiv.org/abs/2605.25449v1)**  
  Authors: Ting-Hsuan Chen, Ying-Huan Chen, Tao Tu, Jie-Ying Lee, Cho-Ying Wu, Fangzhou Lin, Hengyuan Zhang, David Paz, Xinyu Huang, Yuliang Guo, Yu-Lun Liu, Yue Wang, Liu Ren  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25449v1.pdf)  
  Keywords: controllable, temporal consistency, camera control, 3d-aware, trajectory, diffusion model, video generation, video diffusion, simulation  
- **[DeltaCam: Differential Intrinsic Camera Modeling for Video Generation](https://arxiv.org/abs/2605.25266v1)**  
  Authors: Debabrata Mandal, Zhihan Peng, Yujie Wang, Praneeth Chakravarthula  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25266v1.pdf)  
  Keywords: controllable, dynamics, video generation, video-to-video, video style transfer, video diffusion, style, dit  
- **[DexSIM: Real-time Dexterous Simulation with Unified Causal Video Diffusion](https://arxiv.org/abs/2605.24630v1)**  
  Authors: Adam Lee  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.24630v1.pdf)  
  Keywords: autoregressive, trajectory, interactive, diffusion model, video diffusion, robotics, simulation, physical  
- **[Geo-Align: Video Generation Alignment via Metric Geometry Reward](https://arxiv.org/abs/2605.23903v1)**  
  Authors: Zizun Li, Haoyu Guo, Runzhe Teng, Chunhua Shen, Tong He  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.23903v1.pdf)  
  Keywords: camera control, video generation, video-to-video, dit, physical  

### Human & Character Animation

- **[LongCat-Video-Avatar 1.5 Technical Report](https://arxiv.org/abs/2605.26486v1)**  
  Authors: Meituan LongCat Team, Xunliang Cai, Meng Cheng, Feng Gao, Zhe Kong, Jiamu Li, Le Li, Weiheng Li, Hongyu Liu, Shuai Tan, Xiaoming Wei, Tianyu Yang, Yong Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.26486v1.pdf)  
  Keywords: distillation, benchmark, identity, video generation, evaluation, avatar, audio-driven, dit  
- **[RoMo: A Large-Scale, Richly Organized Dataset and Semantic Taxonomy for Human Motion Generation](https://arxiv.org/abs/2605.26241v1)**  
  Authors: Jiahao Zhang, Joseph Liu, Young-Yoon Lee, Seonghyeon Moon, Victor Zordan, Guy Tevet, Karen Liu, Stephen Gould, Oren Jacob, Haomiao Jiang, Mubbasir Kapadia, Yizhak Ben-Shabat  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.26241v1.pdf)  
  Keywords: evaluation, human motion  
- **[iTryOn: Mastering Interactive Video Virtual Try-On with Spatial-Semantic Guidance](https://arxiv.org/abs/2605.21431v1)**  
  Authors: Jun Zheng, Zhengze Xu, Mengting Chen, Jing Wang, Jinsong Lan, Xiaoyong Zhu, Kaifu Zhang, Bo Zheng, Xiaodan Liang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.21431v1.pdf)  
  Keywords: controllable, temporal consistency, diffusion transformer, dynamics, benchmark, interactive, virtual try-on, video diffusion, dit  
- **[EverAnimate: Minute-Scale Human Animation via Latent Flow Restoration](https://arxiv.org/abs/2605.15042v1)**  
  Authors: Wuyang Li, Yang Gao, Mariam Hassan, Lan Feng, Wentao Pan, Po-Chien Luan, Alexandre Alahi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.15042v1.pdf)  
  Keywords: long-form, identity, flow matching, video generation, human motion, human animation, efficient  
- **[PhyMotion: Structured 3D Motion Reward for Physics-Grounded Human Video Generation](https://arxiv.org/abs/2605.14269v1)**  
  Authors: Yidong Huang, Zun Wang, Han Lin, Dong-Ki Kim, Shayegan Omidshafiei, Jaehong Yoon, Jaemin Cho, Yue Zhang, Mohit Bansal  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.14269v1.pdf)  
  Keywords: autoregressive, video generation, evaluation, physics, human motion, dynamics, physical  
- **[SocialDirector: Training-Free Social Interaction Control for Multi-Person Video Generation](https://arxiv.org/abs/2605.10079v1)**  
  Authors: Liangyang Ouyang, Ruicong Liu, Caixin Kang, Yifei Huang, Yoichi Sato  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.10079v1.pdf)  
  Keywords: video generation, gesture, evaluation, robotics, dynamics, film  
- **[MoCoTalk: Multi-Conditional Diffusion with Adaptive Router for Controllable Talking Head Generation](https://arxiv.org/abs/2605.08050v1)**  
  Authors: Xinyan Ye, Jiankang Deng, Abbas Edalat  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.08050v1.pdf)  
  Keywords: controllable, talking head, dynamics, identity, video diffusion, dit  
- **[Omni-Fake: Benchmarking Unified Multimodal Social Media Deepfake Detection](https://arxiv.org/abs/2605.01638v1)**  
  Authors: Tianxiao Li, Zhenglin Huang, Haiquan Wen, Yiwei He, Xinze Li, Bingyu Zhu, Wuhui Duan, Congang Chen, Zeyu Fu, Yi Dong, Baoyuan Wu, Jason Li, Guangliang Cheng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.01638v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://tianxiao1201.github.io/omni-fake-project-page)  
  Keywords: dit, talking head, benchmark  
- **[Generate Your Talking Avatar from Video Reference](https://arxiv.org/abs/2604.27918v1)**  
  Authors: Zujin Guo, Zhenhui Ye, Yi Ren, Yuanming Li, Ce Chen, Zhibin Hong, Chen Change Loy  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2604.27918v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://www.heygen.com/research)  
  Keywords: benchmark, identity, image-to-video, avatar, dit  
- **[HuM-Eval: A Coarse-to-Fine Framework for Human-Centric Video Evaluation](https://arxiv.org/abs/2604.25361v1)**  
  Authors: Bingzi Zhang, Kaisi Guan, Ruihua Song  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2604.25361v1.pdf)  
  Keywords: benchmark, video generation, evaluation, text-to-video, human motion  

### Image-to-Video Generation

- **[Proprio: Latent Self-Scoring and Inference-Time Refinement for Physically Plausible Video Generation](https://arxiv.org/abs/2605.28230v1)**  
  Authors: Mariam Hassan, Kaouther Messaoud, Wuyang Li, Alexandre Alahi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28230v1.pdf)  
  Keywords: benchmark, video generation, image-to-video, evaluation, text-to-video, physics, dynamics, physical  
- **[VidPrism: Heterogeneous Mixture of Experts for Image-to-Video Transfer](https://arxiv.org/abs/2605.28229v1)**  
  Authors: Rui Lin, Chuanming Wang, Huadong Ma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28229v1.pdf) | [![GitHub](https://img.shields.io/github/stars/Lrrrr549/VidPrism.git?style=social)](https://github.com/Lrrrr549/VidPrism.git)  
  Keywords: efficient, benchmark, image-to-video  
- **[PARE: Pruning and Adaptive Routing for Efficient Video Generation](https://arxiv.org/abs/2605.27336v1)**  
  Authors: Yutong Wang, Yunke Wang, Tianfan Xue, Yu Qiao, Yaohui Wang, Xinyuan Chen, Chang Xu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.27336v1.pdf)  
  Keywords: distillation, diffusion transformer, architecture, denoising, acceleration, video generation, image-to-video, text-to-video, video diffusion, efficient, dit  
- **[Timestep-Aware SVDQuant-GPTQ for W4A4 Quantization of Wan2.2-I2V](https://arxiv.org/abs/2605.27003v1)**  
  Authors: Junhao Wu, Dezhong Yao, Hai Jin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.27003v1.pdf)  
  Keywords: diffusion transformer, benchmark, denoising, trajectory, video diffusion, i2v, dit  
- **[Teaching Video Generators to Remember: Eliciting Dynamic Memory for Out-of-Sight State Evolution](https://arxiv.org/abs/2605.25333v1)**  
  Authors: Tianshuo Xu, Yichen Xie, Depu Meng, Chensheng Peng, Quentin Herau, Bo Jiang, Yihan Hu, Wei Zhan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25333v1.pdf)  
  Keywords: world model, diffusion transformer, image-to-video, evaluation, video diffusion, dynamics  
- **[SimInsert: Seamless Video Object Insertion via Regional Sparse Attention Fusion](https://arxiv.org/abs/2605.23245v1)**  
  Authors: Xinyu Chen, Yuyi Qian, Jiang Lin, Shenyi Wang, Gao Wang, Zhiqiu Zhang, Jizhi Zhang, Mingjie Wang, Qiang Tang, Qian Wang, Song Wu, Zili Yi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.23245v1.pdf)  
  Keywords: video editing, denoising, trajectory, interactive, diffusion model, image-to-video, video diffusion, efficient, dit  
- **[MotiMotion: Motion-Controlled Video Generation with Visual Reasoning](https://arxiv.org/abs/2605.22818v1)**  
  Authors: Lee Hsin-Ying, Hanwen Jiang, Yiqun Mei, Jing Shi, Ming-Hsuan Yang, Zhixin Shu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.22818v1.pdf)  
  Keywords: benchmark, video generation, image-to-video, evaluation, motion control  
- **[Aero-World: Action-Conditioned Aerial Video Generation from Inertial Controls](https://arxiv.org/abs/2605.19728v1)**  
  Authors: Abdul Mohaimen Al Radi, Kunyang Li, Yuzhang Shang, Mubarak Shah, Yu Tian  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.19728v1.pdf)  
  Keywords: controllable, diffusion transformer, benchmark, acceleration, trajectory, diffusion model, video generation, evaluation, image-to-video, physics, video diffusion, dit, simulation, action-conditioned, physical  
- **[Rebalancing Reference Frame Dominance to Improve Motion in Image-to-Video Models](https://arxiv.org/abs/2605.19398v2)**  
  Authors: Wooseok Jeon, Seungho Park, Seunghyun Shin, Sangeyl Lee, Hyeonho Jeong, Hae-Gon Jeon  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.19398v2.pdf)  
  Keywords: dynamics, denoising, image-to-video, text-to-video, i2v, dit  
- **[Image-to-Video Diffusion: From Foundations to Open Frontiers](https://arxiv.org/abs/2605.17248v1)**  
  Authors: Xianlong Wang, Wenbo Pan, Shijia Zhou, Ke Li, Yuqi Wang, Zeyu Ye, Hangtao Zhang, Leo Yu Zhang, Xiaohua Jia  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.17248v1.pdf)  
  Keywords: architecture, identity, video generation, image-to-video, evaluation, video diffusion, i2v, dit  

### Long Video Generation

*Showing the latest 50 out of 125 papers*

- **[DriveWAM: Video Generative Priors Enable Scalable World-Action Modeling for Autonomous Driving](https://arxiv.org/abs/2605.28544v1)**  
  Authors: Chen Shi, Jinrui Xu, Shaoshuai Shi, Kehua Sheng, Bo Zhang, Li Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28544v1.pdf)  
  Keywords: diffusion transformer, autoregressive, architecture, benchmark, autonomous driving, video diffusion, dynamics, physical  
- **[ReCA: Multi-Shot Long Video Extrapolation via Recursive Context Allocation](https://arxiv.org/abs/2605.26525v1)**  
  Authors: Akide Liu, Jinbo Xing, Chaojie Mao, Ye Li, Zeyu Zhang, Yefei He, Weijie Wang, Zihan Wang, Yu Liu, Gholamreza Haffari, Bohan Zhuang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.26525v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://reca.vmv.re)  
  Keywords: long video, benchmark, video generation, identity  
- **[Quantized Keys Steal Attention: Bias Correction for KV-Cache Compression in Video Diffusion](https://arxiv.org/abs/2605.26266v1)**  
  Authors: Tuna Tuncer, Felix Becker, Thomas Pfeil  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.26266v1.pdf)  
  Keywords: autoregressive, dit, diffusion model, video diffusion  
- **[AnyScene: Towards Highly Controllable Driving Scene Generation at Anywhere and Beyond](https://arxiv.org/abs/2605.26113v1)**  
  Authors: Haiming Zhang, Junfei Zhou, Feng Jiang, Jingzhong Li, Zhenglong Guo, Penglin Dai, Jifeng Dai, Yan Xie, Benjin Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.26113v1.pdf)  
  Keywords: controllable, diffusion transformer, autoregressive, video synthesis, video generation, layout, autonomous driving, dit, simulation  
- **[On-Policy Adversarial Flow Distillation for Autoregressive Video Generation](https://arxiv.org/abs/2605.26105v1)**  
  Authors: Yang Luo, Shengju Qian, Xiaohang Tang, Zirui Zhu, Yong Liu, Xin Wang, Yang You  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.26105v1.pdf)  
  Keywords: distillation, autoregressive, architecture, denoising, interactive, video generation, physics, streaming, efficient, dit  
- **[StreamChar: Long-Horizon Streaming Character Audio-Video Generation with Decoupled Orchestration](https://arxiv.org/abs/2605.25659v1)**  
  Authors: Linrui Tian, Qi Wang, Bang Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25659v1.pdf)  
  Keywords: distillation, autoregressive, denoising, identity, video generation, streaming, efficient, audio-driven, dit  
- **[Pantheon360: Taming Digital Twin Generation via 3D-Aware 360° Video Diffusion](https://arxiv.org/abs/2605.25449v1)**  
  Authors: Ting-Hsuan Chen, Ying-Huan Chen, Tao Tu, Jie-Ying Lee, Cho-Ying Wu, Fangzhou Lin, Hengyuan Zhang, David Paz, Xinyu Huang, Yuliang Guo, Yu-Lun Liu, Yue Wang, Liu Ren  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25449v1.pdf)  
  Keywords: controllable, temporal consistency, camera control, 3d-aware, trajectory, diffusion model, video generation, video diffusion, simulation  
- **[DexSIM: Real-time Dexterous Simulation with Unified Causal Video Diffusion](https://arxiv.org/abs/2605.24630v1)**  
  Authors: Adam Lee  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.24630v1.pdf)  
  Keywords: autoregressive, trajectory, interactive, diffusion model, video diffusion, robotics, simulation, physical  
- **[EM-Vid: Training-Free Entity-Centric Memory for Efficient and Consistent Multi-Shot Video Generation](https://arxiv.org/abs/2605.23610v1)**  
  Authors: Jente Vandersanden, Matheus Gadelha, Chun-Hao P. Huang, Hyeonho Jeong, Yulia Gryaditskaya  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.23610v1.pdf)  
  Keywords: efficient, autoregressive, dit, video generation  
- **[DrawVideo: Generating Long Video from Storyboard Keyframe Sketches](https://arxiv.org/abs/2605.23508v1)**  
  Authors: Chuanzhi Xu, Huiqi Liang, Bang Shi, Huiming Zhang, Yifan Xiao, Guangcheng Lin, Haodong Chen, Qiang Qu, Zhicheng Lu, Weidong Cai  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.23508v1.pdf)  
  Keywords: controllable, long video, identity, video generation, layout, text-to-video, style, dynamics  

### Personalization & Customization

*Showing the latest 50 out of 83 papers*

- **[Gamma-World: Generative Multi-Agent World Modeling Beyond Two Players](https://arxiv.org/abs/2605.28816v1)**  
  Authors: Fangfu Liu, Kai He, Tianchang Shen, Tianshi Cao, Sanja Fidler, Yueqi Duan, Jun Gao, Igor Gilitschenski, Zian Wang, Xuanchi Ren  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28816v1.pdf)  
  Keywords: controllable, world model, identity, interactive, video generation, dit, efficient, simulation  
- **[Which Pretraining Paradigm Better Serves Spatial Intelligence? An Empirical Comparison of Vision-Language and Video Generation Models](https://arxiv.org/abs/2605.28132v1)**  
  Authors: Haozhan Shen, Tiancheng Zhao, Kangjia Zhao, Jianwei Yin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28132v1.pdf) | [![GitHub](https://img.shields.io/github/stars/om-ai-lab/Probing-VLM-VGM?style=social)](https://github.com/om-ai-lab/Probing-VLM-VGM)  
  Keywords: concept, video generation, physical  
- **[CogPortrait: Fine-Grained Eye-Region Control in Portrait Animation via Hierarchical Agent Planning](https://arxiv.org/abs/2605.28056v1)**  
  Authors: He Feng, Yongjia Ma, Donglin Di, Lei Fan, Tonghua Su  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28056v1.pdf)  
  Keywords: dynamics, benchmark, identity, video generation, motion control, dit  
- **[PlayClass: Automated Play Behaviour Classification in Poultry](https://arxiv.org/abs/2605.27304v1)**  
  Authors: Prince Ravi Leow, Neil Scheidwasser, Rebecca Oscarsson, Per Jensen, Samir Bhatt, David Alejandro Duchêne  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.27304v1.pdf)  
  Keywords: identity  
- **[ReCA: Multi-Shot Long Video Extrapolation via Recursive Context Allocation](https://arxiv.org/abs/2605.26525v1)**  
  Authors: Akide Liu, Jinbo Xing, Chaojie Mao, Ye Li, Zeyu Zhang, Yefei He, Weijie Wang, Zihan Wang, Yu Liu, Gholamreza Haffari, Bohan Zhuang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.26525v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://reca.vmv.re)  
  Keywords: long video, benchmark, video generation, identity  
- **[LongCat-Video-Avatar 1.5 Technical Report](https://arxiv.org/abs/2605.26486v1)**  
  Authors: Meituan LongCat Team, Xunliang Cai, Meng Cheng, Feng Gao, Zhe Kong, Jiamu Li, Le Li, Weiheng Li, Hongyu Liu, Shuai Tan, Xiaoming Wei, Tianyu Yang, Yong Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.26486v1.pdf)  
  Keywords: distillation, benchmark, identity, video generation, evaluation, avatar, audio-driven, dit  
- **[LongAV-Compass: Towards Unified Evaluation of Minute-Scale Audio-Visual Generation Across T2AV, I2AV, and V2AV](https://arxiv.org/abs/2605.26244v1)**  
  Authors: Tengfei Liu, Yang Shi, Xuanyu Zhu, Jiafu Tang, Liu Yang, Qixun Wang, Zhuoran Zhang, Yuqi Tang, Fengxiang Wang, Yuhao Dong, Xinlong Chen, Bozhou Li, Bohan Zeng, Yue Ding, Xiaohan Zhang, Jialu Chen, Haotian Wang, Yuanxing Zhang, Pengfei Wan, Leye Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.26244v1.pdf)  
  Keywords: evaluation, dit, benchmark, identity  
- **[Where Concept Erasure Should Occur: Concept-Layer Alignment in Text-to-Video Diffusion Models](https://arxiv.org/abs/2605.25941v1)**  
  Authors: Yiwei Xie, Ping Liu, Zheng Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25941v1.pdf)  
  Keywords: diffusion transformer, diffusion model, text-to-video, video diffusion, concept  
- **[StreamChar: Long-Horizon Streaming Character Audio-Video Generation with Decoupled Orchestration](https://arxiv.org/abs/2605.25659v1)**  
  Authors: Linrui Tian, Qi Wang, Bang Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25659v1.pdf)  
  Keywords: distillation, autoregressive, denoising, identity, video generation, streaming, efficient, audio-driven, dit  
- **[Test-Time Self-Adaptive Conditioning for Stable Audio-Driven Talking-Head Generation](https://arxiv.org/abs/2605.25488v1)**  
  Authors: Zhicheng Zhang, Lei Wang, Yu Zhang, Yongsheng Gao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25488v1.pdf)  
  Keywords: dynamics, benchmark, identity, video generation, audio-driven, dit  

### Physical Understanding

*Showing the latest 50 out of 153 papers*

- **[HarmoVid: Relightful Video Portrait Harmonization](https://arxiv.org/abs/2605.28811v1)**  
  Authors: Jun Myeong Choi, Jae Shin Yoon, Luchao Qi, Roni Sengupta, Joon-Young Lee  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28811v1.pdf)  
  Keywords: physical, dit, diffusion model, video diffusion  
- **[DriveWAM: Video Generative Priors Enable Scalable World-Action Modeling for Autonomous Driving](https://arxiv.org/abs/2605.28544v1)**  
  Authors: Chen Shi, Jinrui Xu, Shaoshuai Shi, Kehua Sheng, Bo Zhang, Li Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28544v1.pdf)  
  Keywords: diffusion transformer, autoregressive, architecture, benchmark, autonomous driving, video diffusion, dynamics, physical  
- **[Sketch2Motion: Text-driven 2D Sketch to 3D Animation via Diffusion-guided Skeleton Optimization](https://arxiv.org/abs/2605.28394v1)**  
  Authors: Gaurav Rai, Ojaswa Sharma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28394v1.pdf)  
  Keywords: distillation, diffusion model, text-to-video, physics, video diffusion, dit, physical  
- **[Proprio: Latent Self-Scoring and Inference-Time Refinement for Physically Plausible Video Generation](https://arxiv.org/abs/2605.28230v1)**  
  Authors: Mariam Hassan, Kaouther Messaoud, Wuyang Li, Alexandre Alahi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28230v1.pdf)  
  Keywords: benchmark, video generation, image-to-video, evaluation, text-to-video, physics, dynamics, physical  
- **[Which Pretraining Paradigm Better Serves Spatial Intelligence? An Empirical Comparison of Vision-Language and Video Generation Models](https://arxiv.org/abs/2605.28132v1)**  
  Authors: Haozhan Shen, Tiancheng Zhao, Kangjia Zhao, Jianwei Yin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28132v1.pdf) | [![GitHub](https://img.shields.io/github/stars/om-ai-lab/Probing-VLM-VGM?style=social)](https://github.com/om-ai-lab/Probing-VLM-VGM)  
  Keywords: concept, video generation, physical  
- **[CogPortrait: Fine-Grained Eye-Region Control in Portrait Animation via Hierarchical Agent Planning](https://arxiv.org/abs/2605.28056v1)**  
  Authors: He Feng, Yongjia Ma, Donglin Di, Lei Fan, Tonghua Su  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28056v1.pdf)  
  Keywords: dynamics, benchmark, identity, video generation, motion control, dit  
- **[Turning Video Models into Generalist Robot Policies](https://arxiv.org/abs/2605.27817v1)**  
  Authors: Sizhe Lester Li, Evan Kim, Xingjian Bai, Tong Zhao, Tao Pang, Max Simchowitz, Vincent Sitzmann  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.27817v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://vera.csail.mit.edu)  
  Keywords: world model, benchmark, efficient, robotics, dynamics  
- **[Tensor Memory: Fixed-Size Recurrent State for Long-Horizon Transformers](https://arxiv.org/abs/2605.27686v1)**  
  Authors: Kabir Swain, Sijie Han, Daniel Karl I. Weidele, Mauro Martino, Antonio Torralba  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.27686v1.pdf)  
  Keywords: efficient, dynamics, benchmark  
- **[What-If World: A Causal Benchmark for General World Models in Embodied Scenarios](https://arxiv.org/abs/2605.27589v1)**  
  Authors: Kunlin Cai, Rui Song, Jinghuai Zhang, Kaiyuan Zhang, Pranav Bodapati, Alicia Yu, Fnu Suya, Mohammad Rostami, Jiaqi Ma, Yuan Tian  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.27589v1.pdf)  
  Keywords: world model, benchmark, video generation, physics, world simulator, dit, simulation, action-conditioned, physical  
- **[E$^3$C: Video Generation with 3D Environmental Memory and Ego-Exo Human Pose Control](https://arxiv.org/abs/2605.26316v1)**  
  Authors: Qiao Gu, Lingni Ma, Adam W Harley, Richard Newcombe, Florian Shkurti, Julian Straub  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.26316v1.pdf)  
  Keywords: controllable, dynamics, video synthesis, video generation, video diffusion, dit, physical  

### Surveys & Benchmarks

*Showing the latest 50 out of 231 papers*

- **[DriveWAM: Video Generative Priors Enable Scalable World-Action Modeling for Autonomous Driving](https://arxiv.org/abs/2605.28544v1)**  
  Authors: Chen Shi, Jinrui Xu, Shaoshuai Shi, Kehua Sheng, Bo Zhang, Li Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28544v1.pdf)  
  Keywords: diffusion transformer, autoregressive, architecture, benchmark, autonomous driving, video diffusion, dynamics, physical  
- **[Proprio: Latent Self-Scoring and Inference-Time Refinement for Physically Plausible Video Generation](https://arxiv.org/abs/2605.28230v1)**  
  Authors: Mariam Hassan, Kaouther Messaoud, Wuyang Li, Alexandre Alahi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28230v1.pdf)  
  Keywords: benchmark, video generation, image-to-video, evaluation, text-to-video, physics, dynamics, physical  
- **[VidPrism: Heterogeneous Mixture of Experts for Image-to-Video Transfer](https://arxiv.org/abs/2605.28229v1)**  
  Authors: Rui Lin, Chuanming Wang, Huadong Ma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28229v1.pdf) | [![GitHub](https://img.shields.io/github/stars/Lrrrr549/VidPrism.git?style=social)](https://github.com/Lrrrr549/VidPrism.git)  
  Keywords: efficient, benchmark, image-to-video  
- **[Refining Multidimensional Video Reward Models via Disentangled Influence Functions](https://arxiv.org/abs/2605.28203v1)**  
  Authors: Muyao Wang, Zeke Xie, Hideki Nakayama  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28203v1.pdf)  
  Keywords: evaluation, text-to-video, efficient, t2v  
- **[CogPortrait: Fine-Grained Eye-Region Control in Portrait Animation via Hierarchical Agent Planning](https://arxiv.org/abs/2605.28056v1)**  
  Authors: He Feng, Yongjia Ma, Donglin Di, Lei Fan, Tonghua Su  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28056v1.pdf)  
  Keywords: dynamics, benchmark, identity, video generation, motion control, dit  
- **[MTAVG-Bench 2.0: Diagnosing Failure Modes of Cinematic Expressiveness in Multi-Talker Audio-Video Generation](https://arxiv.org/abs/2605.28035v1)**  
  Authors: Haitian Li, Yanghao Zhou, Heyan Huang, Liangji Chen, YiMing Cheng, Xu Liu, Dian Jin, Jiajun Xu, Jingyun Liao, Tian Lan, Ziqin Zhou, Yueying Liu, Yu Bai, Changsen Yuan, Jinxing Zhou, Xian-Ling Mao, Xuefeng Chen, Yousheng Feng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28035v1.pdf)  
  Keywords: evaluation, benchmark, video generation  
- **[VCap: Hypergeometric Rewards for Weak-to-Strong Visual Captioning](https://arxiv.org/abs/2605.28023v1)**  
  Authors: Xingyu Lu, Jinpeng Wang, Yi-Fan Zhang, Yankai Yang, Yancheng Long, Yiyang Fan, Xuanyu Zheng, Haonan Fan, Kaiyu Jiang, Tianke Zhang, Changyi Liu, Bin Wen, Fan Yang, Tingting Gao, Han Li, Chun Yuan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28023v1.pdf)  
  Keywords: evaluation, dit, benchmark, distillation  
- **[Turning Video Models into Generalist Robot Policies](https://arxiv.org/abs/2605.27817v1)**  
  Authors: Sizhe Lester Li, Evan Kim, Xingjian Bai, Tong Zhao, Tao Pang, Max Simchowitz, Vincent Sitzmann  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.27817v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://vera.csail.mit.edu)  
  Keywords: world model, benchmark, efficient, robotics, dynamics  
- **[Tensor Memory: Fixed-Size Recurrent State for Long-Horizon Transformers](https://arxiv.org/abs/2605.27686v1)**  
  Authors: Kabir Swain, Sijie Han, Daniel Karl I. Weidele, Mauro Martino, Antonio Torralba  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.27686v1.pdf)  
  Keywords: efficient, dynamics, benchmark  
- **[What-If World: A Causal Benchmark for General World Models in Embodied Scenarios](https://arxiv.org/abs/2605.27589v1)**  
  Authors: Kunlin Cai, Rui Song, Jinghuai Zhang, Kaiyuan Zhang, Pranav Bodapati, Alicia Yu, Fnu Suya, Mohammad Rostami, Jiaqi Ma, Yuan Tian  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.27589v1.pdf)  
  Keywords: world model, benchmark, video generation, physics, world simulator, dit, simulation, action-conditioned, physical  

### Text-to-Video Generation

- **[OSP-Next: Efficient High-Quality Video Generation with Sparse Sequence Parallelism, HiF8 Quantization, and Reinforcement Learning](https://arxiv.org/abs/2605.28691v1)**  
  Authors: Yunyang Ge, Xianyi He, Zezhong Zhang, Bin Lin, Bin Zhu, Xinhua Cheng, Li Yuan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28691v1.pdf)  
  Keywords: diffusion transformer, architecture, video generation, text-to-video, efficient, dit  
- **[Sketch2Motion: Text-driven 2D Sketch to 3D Animation via Diffusion-guided Skeleton Optimization](https://arxiv.org/abs/2605.28394v1)**  
  Authors: Gaurav Rai, Ojaswa Sharma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28394v1.pdf)  
  Keywords: distillation, diffusion model, text-to-video, physics, video diffusion, dit, physical  
- **[Proprio: Latent Self-Scoring and Inference-Time Refinement for Physically Plausible Video Generation](https://arxiv.org/abs/2605.28230v1)**  
  Authors: Mariam Hassan, Kaouther Messaoud, Wuyang Li, Alexandre Alahi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28230v1.pdf)  
  Keywords: benchmark, video generation, image-to-video, evaluation, text-to-video, physics, dynamics, physical  
- **[Refining Multidimensional Video Reward Models via Disentangled Influence Functions](https://arxiv.org/abs/2605.28203v1)**  
  Authors: Muyao Wang, Zeke Xie, Hideki Nakayama  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28203v1.pdf)  
  Keywords: evaluation, text-to-video, efficient, t2v  
- **[PARE: Pruning and Adaptive Routing for Efficient Video Generation](https://arxiv.org/abs/2605.27336v1)**  
  Authors: Yutong Wang, Yunke Wang, Tianfan Xue, Yu Qiao, Yaohui Wang, Xinyuan Chen, Chang Xu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.27336v1.pdf)  
  Keywords: distillation, diffusion transformer, architecture, denoising, acceleration, video generation, image-to-video, text-to-video, video diffusion, efficient, dit  
- **[Tail-Aware HiFloat4: W4A4 Post-Training Quantization for Wan2.2](https://arxiv.org/abs/2605.26628v1)**  
  Authors: Zhanfeng Feng, Shuai Guo, Xin Di, Long Peng, Yang Cao, Zhengjun Zha  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.26628v1.pdf)  
  Keywords: text-to-video, dit, video generation  
- **[Paris 2.0: A Decentralized Diffusion Model for Video Generation](https://arxiv.org/abs/2605.26064v2)**  
  Authors: Ali Rouzbayani, Bidhan Roy, Marcos Villagra, Zhiying Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.26064v2.pdf)  
  Keywords: text-to-video, video generation, diffusion model  
- **[Where Concept Erasure Should Occur: Concept-Layer Alignment in Text-to-Video Diffusion Models](https://arxiv.org/abs/2605.25941v1)**  
  Authors: Yiwei Xie, Ping Liu, Zheng Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25941v1.pdf)  
  Keywords: diffusion transformer, diffusion model, text-to-video, video diffusion, concept  
- **[DrawVideo: Generating Long Video from Storyboard Keyframe Sketches](https://arxiv.org/abs/2605.23508v1)**  
  Authors: Chuanzhi Xu, Huiqi Liang, Bang Shi, Huiming Zhang, Yifan Xiao, Guangcheng Lin, Haodong Chen, Qiang Qu, Zhicheng Lu, Weidong Cai  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.23508v1.pdf)  
  Keywords: controllable, long video, identity, video generation, layout, text-to-video, style, dynamics  
- **[RE-TRIANGLE: Does TRIANGLE Enable Multimodal Alignment Beyond Cosine Similarity in Retrieval?](https://arxiv.org/abs/2605.27436v1)**  
  Authors: Arijit Ghosh, Aritra Bandyopadhyay, Chiranjeev Bindra, Jingfen Qiao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.27436v1.pdf) | [![GitHub](https://img.shields.io/github/stars/ARIJIT00171/RE-TRIANGLE?style=social)](https://github.com/ARIJIT00171/RE-TRIANGLE)  
  Keywords: text-to-video, dit  

### Video Editing

- **[DeltaCam: Differential Intrinsic Camera Modeling for Video Generation](https://arxiv.org/abs/2605.25266v1)**  
  Authors: Debabrata Mandal, Zhihan Peng, Yujie Wang, Praneeth Chakravarthula  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25266v1.pdf)  
  Keywords: controllable, dynamics, video generation, video-to-video, video style transfer, video diffusion, style, dit  
- **[Geo-Align: Video Generation Alignment via Metric Geometry Reward](https://arxiv.org/abs/2605.23903v1)**  
  Authors: Zizun Li, Haoyu Guo, Runzhe Teng, Chunhua Shen, Tong He  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.23903v1.pdf)  
  Keywords: camera control, video generation, video-to-video, dit, physical  
- **[SimInsert: Seamless Video Object Insertion via Regional Sparse Attention Fusion](https://arxiv.org/abs/2605.23245v1)**  
  Authors: Xinyu Chen, Yuyi Qian, Jiang Lin, Shenyi Wang, Gao Wang, Zhiqiu Zhang, Jizhi Zhang, Mingjie Wang, Qiang Tang, Qian Wang, Song Wu, Zili Yi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.23245v1.pdf)  
  Keywords: video editing, denoising, trajectory, interactive, diffusion model, image-to-video, video diffusion, efficient, dit  
- **[StreamGVE: Training-Free Video Editing via Few-Step Streaming Video Generation](https://arxiv.org/abs/2605.21466v1)**  
  Authors: Guanlong Jiao, Chenyangguang Zhang, Jia Jun Cheng Xian, Zewei Zhang, Renjie Liao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.21466v1.pdf)  
  Keywords: streaming, video editing, dit, video generation  
- **[Preserve, Reveal, Expand: Faithful 4D Video Editing with Region-Aware Conditioning](https://arxiv.org/abs/2605.20961v1)**  
  Authors: Zhangchi Hu, Wenzhang Sun, Xiangchen Yin, Jiahui Yuan, Chunfeng Wang, Hao Li, Kun Zhan, Xiaoyan Sun  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20961v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://ricepastem.github.io/PREX-Open)  
  Keywords: video editing, benchmark, diffusion model, evaluation, video diffusion, dit  
- **[What Semantics Survive the Connector? Diagnosing VLM-to-DiT Alignment in Video Editing](https://arxiv.org/abs/2605.20795v1)**  
  Authors: Hangyu Lin, Chao Wen, Chengming Xu, Jianxiong Gao, Jiangning Zhang, Xiaobin Hu, Yanwei Fu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20795v1.pdf)  
  Keywords: video editing, architecture, multi-modal, flow matching, evaluation, dit  
- **[Goodbye Drift: Anchored Tree Sampling for Long-Horizon Video-to-Video Generation](https://arxiv.org/abs/2605.20476v1)**  
  Authors: Matthew Bendel, Stephen W. Bailey, Mithilesh Vaidya, Sumukh Badam, Xingzhe He  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20476v1.pdf)  
  Keywords: distillation, autoregressive, outpainting, video generation, video-to-video, t2v, style, dit  
- **[PhyWorld: Physics-Faithful World Model for Video Generation](https://arxiv.org/abs/2605.19242v1)**  
  Authors: Pu Zhao, Juyi Lin, Timothy Rupprecht, Arash Akbari, Chence Yang, Rahul Chowdhury, Elaheh Motamedi, Arman Akbari, Yumei He, Chen Wang, Geng Yuan, Weiwei Chen, Yanzhi Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.19242v1.pdf)  
  Keywords: world model, dynamics, benchmark, flow matching, video generation, video-to-video, physics, world simulator, dit, physical  
- **[Aurora: Unified Video Editing with a Tool-Using Agent](https://arxiv.org/abs/2605.18748v1)**  
  Authors: Yongsheng Yu, Ziyun Zeng, Zhiyuan Xiao, Zhenghong Zhou, Hang Hua, Wei Xiong, Jiebo Luo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.18748v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://yeates.github.io/Aurora-Page)  
  Keywords: video editing, diffusion transformer, benchmark, video diffusion, style, dit  
- **[InstructAV2AV: Instruction-Guided Audio-Video Joint Editing](https://arxiv.org/abs/2605.18467v1)**  
  Authors: Haojie Zheng, Yixin Yang, Siqi Yang, Shuchen Weng, Boxin Shi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.18467v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://hjzheng.net/projects/InstructAV2AV)  
  Keywords: video editing, controllable, video generation, evaluation, dit  

### Video Inpainting & Completion

- **[Full-4D: Generating Full-Scope 4D Scenes from a Single-View Video](https://arxiv.org/abs/2605.25500v1)**  
  Authors: Tingxi Chen, Ke Hao, Yabo Chen, Zhengxue Cheng, Rong Xie, Li Song, Haibin Huang, Chi Zhang, Xuelong Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25500v1.pdf)  
  Keywords: distillation, 4d generation, flow matching, video synthesis, interactive, multi-view video, diffusion model, video diffusion, dit, video interpolation, physical  
- **[CRONOS: Benchmarking Counterfactual Physical Consistency in Video Models](https://arxiv.org/abs/2605.23699v1)**  
  Authors: León Begiristain, Olaf Dünkel, Adam Kortylewski  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.23699v1.pdf)  
  Keywords: world model, video prediction, benchmark, dynamics, evaluation, dit, physical  
- **[GEM-4D: Geometry-Enhanced Video World Models for Robot Manipulation](https://arxiv.org/abs/2605.22882v1)**  
  Authors: Kaichen Zhou, Yuzhen Chen, Fangneng Zhan, Hang Hua, Grace Chen, Xinhai Chang, Ao Qu, Yilun Du, Zhuang Liu, Paul Pu Liang, Mengyu Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.22882v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://anonymous-submission-20.github.io/gem.github.io)  
  Keywords: world model, video prediction, architecture, dynamics, simulation, dit, physical  
- **[Goodbye Drift: Anchored Tree Sampling for Long-Horizon Video-to-Video Generation](https://arxiv.org/abs/2605.20476v1)**  
  Authors: Matthew Bendel, Stephen W. Bailey, Mithilesh Vaidya, Sumukh Badam, Xingzhe He  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20476v1.pdf)  
  Keywords: distillation, autoregressive, outpainting, video generation, video-to-video, t2v, style, dit  
- **[Nano World Models: A Minimalist Implementation of Future Video Prediction](https://arxiv.org/abs/2605.23993v1)**  
  Authors: Siqiao Huang, Partha Kaushik, Michael Chen, Hengkai Pan, Omar Chehab, Fernando Moreno-Pino, Max Simchowitz  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.23993v1.pdf)  
  Keywords: world model, autoregressive, video prediction, architecture, interactive, video generation, evaluation, dit, simulation  
- **[Relit-LiVE: Relight Video by Jointly Learning Environment Video](https://arxiv.org/abs/2605.06658v1)**  
  Authors: Weiqing Xiao, Hong Li, Xiuyu Yang, Houyuan Chen, Wenyi Li, Tianqi Liu, Shaocong Xu, Chongjie Ye, Hao Zhao, Beibei Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.06658v1.pdf) | [![GitHub](https://img.shields.io/github/stars/zhuxing0/Relit-LiVE?style=social)](https://github.com/zhuxing0/Relit-LiVE)  
  Keywords: video prediction, benchmark, diffusion model, streaming, video diffusion, dit, physical  
- **[Quaternion Nonlinear Transform-Induced Nuclear Norm for Low-Rank Tensor Completion](https://arxiv.org/abs/2605.01467v1)**  
  Authors: Biswarup Karmakar, Ratikanta Behera  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.01467v1.pdf)  
  Keywords: efficient, benchmark, video inpainting  
- **[LMGenDrive: Bridging Multimodal Understanding and Generative World Modeling for End-to-End Driving](https://arxiv.org/abs/2604.08719v1)**  
  Authors: Hao Shao, Letian Wang, Yang Zhou, Yuxuan Hu, Zhuofan Zong, Steven L. Waslander, Wei Zhan, Hongsheng Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2604.08719v1.pdf)  
  Keywords: world model, autoregressive, video prediction, benchmark, video generation, autonomous driving  
- **[Novel View Synthesis as Video Completion](https://arxiv.org/abs/2604.08500v1)**  
  Authors: Qi Wu, Khiem Vuong, Minsik Jeon, Srinivasa Narasimhan, Deva Ramanan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2604.08500v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://frame-crafter.github.io)  
  Keywords: benchmark, video completion, diffusion model, video diffusion, novel view  
- **[SEM-ROVER: Semantic Voxel-Guided Diffusion for Large-Scale Driving Scene Generation](https://arxiv.org/abs/2604.06113v1)**  
  Authors: Hiba Dahmani, Nathan Piasco, Moussab Bennehar, Luis Roldão, Dzmitry Tsishkou, Laurent Caraffa, Jean-Philippe Tarel, Roland Brémond  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2604.06113v1.pdf)  
  Keywords: outpainting, dit, diffusion model  

### Video Super-Resolution & Enhancement

*Showing the latest 50 out of 65 papers*

- **[PARE: Pruning and Adaptive Routing for Efficient Video Generation](https://arxiv.org/abs/2605.27336v1)**  
  Authors: Yutong Wang, Yunke Wang, Tianfan Xue, Yu Qiao, Yaohui Wang, Xinyuan Chen, Chang Xu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.27336v1.pdf)  
  Keywords: distillation, diffusion transformer, architecture, denoising, acceleration, video generation, image-to-video, text-to-video, video diffusion, efficient, dit  
- **[Timestep-Aware SVDQuant-GPTQ for W4A4 Quantization of Wan2.2-I2V](https://arxiv.org/abs/2605.27003v1)**  
  Authors: Junhao Wu, Dezhong Yao, Hai Jin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.27003v1.pdf)  
  Keywords: diffusion transformer, benchmark, denoising, trajectory, video diffusion, i2v, dit  
- **[On-Policy Adversarial Flow Distillation for Autoregressive Video Generation](https://arxiv.org/abs/2605.26105v1)**  
  Authors: Yang Luo, Shengju Qian, Xiaohang Tang, Zirui Zhu, Yong Liu, Xin Wang, Yang You  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.26105v1.pdf)  
  Keywords: distillation, autoregressive, architecture, denoising, interactive, video generation, physics, streaming, efficient, dit  
- **[StreamChar: Long-Horizon Streaming Character Audio-Video Generation with Decoupled Orchestration](https://arxiv.org/abs/2605.25659v1)**  
  Authors: Linrui Tian, Qi Wang, Bang Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25659v1.pdf)  
  Keywords: distillation, autoregressive, denoising, identity, video generation, streaming, efficient, audio-driven, dit  
- **[SimInsert: Seamless Video Object Insertion via Regional Sparse Attention Fusion](https://arxiv.org/abs/2605.23245v1)**  
  Authors: Xinyu Chen, Yuyi Qian, Jiang Lin, Shenyi Wang, Gao Wang, Zhiqiu Zhang, Jizhi Zhang, Mingjie Wang, Qiang Tang, Qian Wang, Song Wu, Zili Yi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.23245v1.pdf)  
  Keywords: video editing, denoising, trajectory, interactive, diffusion model, image-to-video, video diffusion, efficient, dit  
- **[Dynamic Video Generation: Shaping Video Generation Across Time and Space](https://arxiv.org/abs/2605.21042v1)**  
  Authors: Shikang Zheng, Jingkai Huang, Jiacheng Liu, Guantao Chen, Lixuan, Yuqi Lin, Peiliang Cai, Linfeng Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.21042v1.pdf)  
  Keywords: distillation, denoising, acceleration, video generation, diffusion model, efficient, dit  
- **[Accelerating Video Inverse Problem Solvers with Autoregressive Diffusion Models](https://arxiv.org/abs/2605.20624v1)**  
  Authors: Taesung Kwon, Jonghyun Park, Hyungjin Chung, Jong Chul Ye  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20624v1.pdf)  
  Keywords: video restoration, autoregressive, diffusion model, streaming, video diffusion  
- **[Rebalancing Reference Frame Dominance to Improve Motion in Image-to-Video Models](https://arxiv.org/abs/2605.19398v2)**  
  Authors: Wooseok Jeon, Seungho Park, Seunghyun Shin, Sangeyl Lee, Hyeonho Jeong, Hae-Gon Jeon  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.19398v2.pdf)  
  Keywords: dynamics, denoising, image-to-video, text-to-video, i2v, dit  
- **[LongLive-2.0: An NVFP4 Parallel Infrastructure for Long Video Generation](https://arxiv.org/abs/2605.18739v2)**  
  Authors: Yukang Chen, Luozhou Wang, Wei Huang, Shuai Yang, Bohan Zhang, Yicheng Xiao, Ruihang Chu, Weian Mao, Qixin Hu, Shaoteng Liu, Yuyang Zhao, Huizi Mao, Ying-Cong Chen, Enze Xie, Xiaojuan Qi, Song Han  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.18739v2.pdf)  
  Keywords: distillation, autoregressive, long video, benchmark, denoising, architecture, interactive, video generation, layout, diffusion model, streaming, efficient  
- **[Spectral Progressive Diffusion for Efficient Image and Video Generation](https://arxiv.org/abs/2605.18736v2)**  
  Authors: Howard Xiao, Brian Chao, Lior Yariv, Gordon Wetzstein  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.18736v2.pdf)  
  Keywords: autoregressive, denoising, acceleration, trajectory, video generation, diffusion model, efficient  

### World Models & Simulation

*Showing the latest 50 out of 122 papers*

- **[Gamma-World: Generative Multi-Agent World Modeling Beyond Two Players](https://arxiv.org/abs/2605.28816v1)**  
  Authors: Fangfu Liu, Kai He, Tianchang Shen, Tianshi Cao, Sanja Fidler, Yueqi Duan, Jun Gao, Igor Gilitschenski, Zian Wang, Xuanchi Ren  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28816v1.pdf)  
  Keywords: controllable, world model, identity, interactive, video generation, dit, efficient, simulation  
- **[Turning Video Models into Generalist Robot Policies](https://arxiv.org/abs/2605.27817v1)**  
  Authors: Sizhe Lester Li, Evan Kim, Xingjian Bai, Tong Zhao, Tao Pang, Max Simchowitz, Vincent Sitzmann  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.27817v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://vera.csail.mit.edu)  
  Keywords: world model, benchmark, efficient, robotics, dynamics  
- **[What-If World: A Causal Benchmark for General World Models in Embodied Scenarios](https://arxiv.org/abs/2605.27589v1)**  
  Authors: Kunlin Cai, Rui Song, Jinghuai Zhang, Kaiyuan Zhang, Pranav Bodapati, Alicia Yu, Fnu Suya, Mohammad Rostami, Jiaqi Ma, Yuan Tian  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.27589v1.pdf)  
  Keywords: world model, benchmark, video generation, physics, world simulator, dit, simulation, action-conditioned, physical  
- **[AnyScene: Towards Highly Controllable Driving Scene Generation at Anywhere and Beyond](https://arxiv.org/abs/2605.26113v1)**  
  Authors: Haiming Zhang, Junfei Zhou, Feng Jiang, Jingzhong Li, Zhenglong Guo, Penglin Dai, Jifeng Dai, Yan Xie, Benjin Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.26113v1.pdf)  
  Keywords: controllable, diffusion transformer, autoregressive, video synthesis, video generation, layout, autonomous driving, dit, simulation  
- **[On-Policy Adversarial Flow Distillation for Autoregressive Video Generation](https://arxiv.org/abs/2605.26105v1)**  
  Authors: Yang Luo, Shengju Qian, Xiaohang Tang, Zirui Zhu, Yong Liu, Xin Wang, Yang You  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.26105v1.pdf)  
  Keywords: distillation, autoregressive, architecture, denoising, interactive, video generation, physics, streaming, efficient, dit  
- **[Full-4D: Generating Full-Scope 4D Scenes from a Single-View Video](https://arxiv.org/abs/2605.25500v1)**  
  Authors: Tingxi Chen, Ke Hao, Yabo Chen, Zhengxue Cheng, Rong Xie, Li Song, Haibin Huang, Chi Zhang, Xuelong Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25500v1.pdf)  
  Keywords: distillation, 4d generation, flow matching, video synthesis, interactive, multi-view video, diffusion model, video diffusion, dit, video interpolation, physical  
- **[Pantheon360: Taming Digital Twin Generation via 3D-Aware 360° Video Diffusion](https://arxiv.org/abs/2605.25449v1)**  
  Authors: Ting-Hsuan Chen, Ying-Huan Chen, Tao Tu, Jie-Ying Lee, Cho-Ying Wu, Fangzhou Lin, Hengyuan Zhang, David Paz, Xinyu Huang, Yuliang Guo, Yu-Lun Liu, Yue Wang, Liu Ren  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25449v1.pdf)  
  Keywords: controllable, temporal consistency, camera control, 3d-aware, trajectory, diffusion model, video generation, video diffusion, simulation  
- **[Toward Native Multimodal Modeling: A Roadmap](https://arxiv.org/abs/2605.25343v1)**  
  Authors: Siyu An, Junru Lu, Junnan Dong, Qiufeng Wang, Yinghui Li, Weizhi Fei, Zichao Yu, Zheng Yuan, Biao Liu, Haopeng Wang, Renzhao Liang, Yixuan Yang, Yunhang Shen, Bo Ke, Keyu Chen, Linhao Luo, Difan Zou, Xiao Huang, Di Yin, Ruizhi Qiao, Xing Sun  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25343v1.pdf)  
  Keywords: evaluation, world model, architecture, video generation  
- **[Teaching Video Generators to Remember: Eliciting Dynamic Memory for Out-of-Sight State Evolution](https://arxiv.org/abs/2605.25333v1)**  
  Authors: Tianshuo Xu, Yichen Xie, Depu Meng, Chensheng Peng, Quentin Herau, Bo Jiang, Yihan Hu, Wei Zhan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25333v1.pdf)  
  Keywords: world model, diffusion transformer, image-to-video, evaluation, video diffusion, dynamics  
- **[X-Foresight: A Joint Vision-Action Causal Forecasting Network via Predictive World Modeling](https://arxiv.org/abs/2605.24892v1)**  
  Authors: Baolu Li, Jingyu Qian, Rui Guo, Yilun Chen, Hanpeng Liu, Yuan Lin, Junhong Zhou, Ruixin Liu, Willow Yang, Yutong Zheng, Zhenli Zhang, Tenglong, Gu, Zhuangzhuang Ding, Pengkun Zheng, Yu Zhang, Xianming Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.24892v1.pdf)  
  Keywords: world model, architecture, efficient, dynamics, physical  



## Classic Papers
- **[Video Diffusion Models](https://arxiv.org/abs/2204.03458)** (NeurIPS 2022)  
  Authors: Jonathan Ho, Tim Salimans, Alexey Gritsenko, William Chan, Mohammad Norouzi, David J. Fleet  
  Keywords: Video Diffusion, Generative Model, Unconditional Video Generation

- **[Align your Latents: High-Resolution Video Synthesis with Latent Diffusion Models](https://arxiv.org/abs/2304.08818)** (CVPR 2023)  
  Authors: Andreas Blattmann, Robin Rombach, Huan Ling, Tim Dockhorn, Seung Wook Kim, Sanja Fidler, Karsten Kreis  
  Keywords: Latent Video Diffusion, Text-to-Video, High-Resolution

- **[Stable Video Diffusion: Scaling Latent Video Diffusion Models to Large Datasets](https://arxiv.org/abs/2311.15127)** (2023)  
  Authors: Andreas Blattmann, Tim Dockhorn, Sumith Kulal, Daniel Menber, Maciej Kilian, Dominik Lorenz, et al.  
  Code: 🔗 [GitHub](https://github.com/Stability-AI/generative-models)  
  Keywords: Image-to-Video, Latent Video Diffusion, Large-Scale Training

- **[Sora: Video Generation Models as World Simulators](https://openai.com/research/video-generation-models-as-world-simulators)** (OpenAI, 2024)  
  Authors: OpenAI  
  Keywords: Text-to-Video, World Simulator, Diffusion Transformer, Long Video

- **[CogVideoX: Text-to-Video Diffusion Models with An Expert Transformer](https://arxiv.org/abs/2408.06072)** (2024)  
  Authors: Zhuoyi Yang, Jiayan Teng, Wendi Zheng, Ming Ding, Shiyu Huang, et al.  
  Code: 🔗 [GitHub](https://github.com/THUDM/CogVideo)  
  Keywords: Text-to-Video, Diffusion Transformer, Expert Transformer

## Open Source Projects
- [CogVideo](https://github.com/THUDM/CogVideo) - Text-to-video generation with CogVideoX series models (Tsinghua & Zhipu AI)
- [Open-Sora](https://github.com/hpcaitech/Open-Sora) - Open-source Sora-like video generation framework
- [Open-Sora-Plan](https://github.com/PKU-YuanGroup/Open-Sora-Plan) - Reproducing Sora with an open-source plan
- [HunyuanVideo](https://github.com/Tencent/HunyuanVideo) - Tencent's large-scale video generation model
- [Wan2.1](https://github.com/Wan-Video/Wan2.1) - Alibaba's open-source video generation model
- [AnimateDiff](https://github.com/guoyww/AnimateDiff) - Animate personalized text-to-image models without specific tuning
- [Stable Video Diffusion](https://github.com/Stability-AI/generative-models) - Stability AI's video generation models
- [ModelScope Text-to-Video](https://github.com/modelscope/modelscope) - ModelScope text-to-video synthesis

## Tutorials & Blogs
- [Video Generation Models as World Simulators](https://openai.com/research/video-generation-models-as-world-simulators) - OpenAI's Sora technical report
- [A Survey on Video Diffusion Models](https://arxiv.org/abs/2310.10647) - Comprehensive survey on video diffusion
- [Diffusion Models: A Comprehensive Survey](https://arxiv.org/abs/2209.00796) - Foundation knowledge on diffusion models

## 📋 Project Features

### 🛠️ Core Features
- **Unified CLI** (`main.py`): Single entry point with `init`, `search`, `suggest`, `export-bib`, `readme` subcommands
- **Interactive Config Wizard**: Guided setup for keywords, domains, time range, and API keys via `python main.py init`
- **Custom Search Keywords**: Configure keywords for title, abstract, or both; with arXiv domain filtering (`cs.CV`, `cs.AI`, `cs.MM`, etc.)
- **Time Range Filtering**: Relative periods (`30d`, `6m`, `1y`, `2y`) or absolute date ranges (`YYYY-MM-DD` to `YYYY-MM-DD`)
- **Smart Link Extraction**: Auto-classifies URLs from abstracts into GitHub, project page, dataset, video, demo, HuggingFace links
- **BibTeX Export**: Fetch BibTeX from arXiv official API; export to `.bib` files with category and date filters
- **LLM Keyword Suggestion**: Input paper titles or arXiv IDs to auto-generate optimized search keywords via OpenAI-compatible API
- **Automated Paper Collection**: Daily automatic crawling with GitHub Actions
- **Intelligent Classification**: Auto-categorize papers into 16 topics (T2V, I2V, Video Editing, Controllable Generation, World Models, etc.)

### 🛠️ Technical Features
- **Robust Error Handling**: Multi-layer retry and fallback strategies ensure stable operation
- **GitHub Actions Integration**: Automated CI/CD workflows for daily updates
- **Multi-type Link Badges**: README entries display PDF, GitHub (with stars), Project, Dataset, Video, Demo, HuggingFace, and Citation badges
- **Detailed Logging**: Comprehensive logging for debugging and monitoring
- **Cross-Platform**: Support for Windows/Linux/macOS

### 📚 Data Output
- **Paper JSON files** (`data/papers_YYYY-MM-DD.json`): Full paper metadata with title, authors, abstract, links, keywords, BibTeX
- **BibTeX files** (`output/*.bib`): Ready-to-use bibliography files for LaTeX
- **Auto-generated README**: Categorized and formatted paper listings

## 🚀 Quick Start

### 1. Install Dependencies

```bash
pip install -r requirements.txt
```

### 2. Interactive Setup (Recommended)

```bash
python main.py init
```

This wizard walks you through:
- Setting search keywords (for title, abstract, or both)
- Selecting arXiv domains (e.g., `cs.CV`, `cs.AI`, `cs.MM`)
- Configuring time range (relative like `6m`/`1y`, or absolute dates)
- Setting max results
- Optionally configuring an OpenAI-compatible API key for keyword suggestion

### 3. Search Papers

```bash
# Search with settings from user_config.json
python main.py search

# Override: fetch 200 papers from the last 6 months, include BibTeX
python main.py search --max-results 200 --recent 6m --bibtex

# Search with absolute date range
python main.py search --date-from 2024-01-01 --date-to 2025-01-01

# Include citation counts from Semantic Scholar
python main.py search --citations
```

### 4. Export BibTeX

```bash
# Export all papers from the latest data file
python main.py export-bib --output output/references.bib

# Export only "Text-to-Video Generation" papers
python main.py export-bib --category "Text-to-Video Generation" --output output/t2v.bib

# Export papers from a specific date range
python main.py export-bib --date-from 2024-06-01 --date-to 2025-01-01 --output output/recent.bib
```

### 5. LLM Keyword Suggestion

```bash
# Generate keywords from paper titles
python main.py suggest --titles "Video Diffusion Models" "Stable Video Diffusion"

# Generate from arXiv IDs (auto-fetches titles)
python main.py suggest --arxiv-ids 2204.03458 2311.15127

# Auto-write suggested keywords to config
python main.py suggest --titles "Sora" "CogVideoX" --apply

# Use a custom API endpoint (e.g., DeepSeek)
python main.py suggest --titles "Paper Title" --base-url https://api.deepseek.com/v1 --api-key sk-xxx --model deepseek-chat
```

### 6. Generate README

```bash
# Basic README
python main.py readme

# Include latest papers section and abstracts
python main.py readme --show-latest --show-abstracts
```

### Configuration File

All settings are stored in `data/user_config.json`:

```json
{
  "search": {
    "keywords": {
      "both_abstract_and_title": ["video diffusion", "video generation", "text-to-video"],
      "abstract_only": ["diffusion model video generation"],
      "title_only": ["video generation", "video diffusion"]
    },
    "domains": ["cs.CV", "cs.AI", "cs.MM"],
    "time_range": {
      "mode": "relative",
      "relative": "1y"
    },
    "max_results": 500
  },
  "api_keys": {
    "openai_api_key": "",
    "openai_base_url": "https://api.openai.com/v1",
    "openai_model": "gpt-4o-mini"
  }
}
```

## Contribution Guidelines
Feel free to submit Pull Requests to improve this list! Please follow these formats:
- Paper entry format: `**[Paper Title](link)** - Brief description`
- Project entry format: `[Project Name](link) - Project description`

## License
[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/) 
