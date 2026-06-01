# Awesome Video Diffusions [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of latest research papers, projects and resources related to Video Diffusion Models and Video Generation. Content is automatically updated daily.

> Last Update: 2026-06-01 04:07:00

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

- [3D-aware Video Generation](#3d-aware-video-generation) (17 papers) - Video generation with 3D awareness, multi-view consistency, and 4D content creation
- [Applications](#applications) (53 papers) - Domain-specific applications of video diffusion models
- [Architecture & Efficiency](#architecture-&-efficiency) (361 papers) - Architectural innovations (DiT, UNet), flow matching, and training/inference efficiency
- [Audio & Multi-modal](#audio-&-multi-modal) (30 papers) - Audio-driven and multi-modal conditioned video generation
- [Controllable Generation](#controllable-generation) (131 papers) - Controllable video generation with motion, camera, pose, or layout guidance
- [Human & Character Animation](#human-&-character-animation) (23 papers) - Human-centric video generation including talking heads, dance, and character animation
- [Image-to-Video Generation](#image-to-video-generation) (41 papers) - Methods for animating still images into videos
- [Long Video Generation](#long-video-generation) (133 papers) - Generating temporally consistent long-form videos beyond short clips
- [Personalization & Customization](#personalization-&-customization) (84 papers) - Personalized video generation with custom subjects, identities, or styles
- [Physical Understanding](#physical-understanding) (150 papers) - Physics-aware video generation and dynamics modeling
- [Surveys & Benchmarks](#surveys-&-benchmarks) (227 papers) - Survey papers, benchmarks, and evaluation metrics for video generation
- [Text-to-Video Generation](#text-to-video-generation) (51 papers) - Foundation models and methods for generating videos from text prompts
- [Video Editing](#video-editing) (30 papers) - Diffusion-based video editing, style transfer, and manipulation
- [Video Inpainting & Completion](#video-inpainting-&-completion) (10 papers) - Video inpainting, completion, outpainting, and temporal prediction
- [Video Super-Resolution & Enhancement](#video-super-resolution-&-enhancement) (69 papers) - Video quality improvement, upscaling, restoration, and frame interpolation
- [World Models & Simulation](#world-models-&-simulation) (121 papers) - Video generation as world simulators and interactive environment generation



## Table of Contents

- [Categorized Papers](#categorized-papers)
- [Classic Papers](#classic-papers)
- [Open Source Projects](#open-source-projects)
- [Applications](#applications)
- [Tutorials & Blogs](#tutorials--blogs)





## Categorized Papers

### 3D-aware Video Generation

- **[Robust Dreamer: Deviation-Aware Latent Gaussian Memory for Action-Controlled AR Video Generation](https://arxiv.org/abs/2605.30855v1)**  
  Authors: Hanlin Chen, Jiaxin Wei, Xibin Song, Yifu Wang, Steve Wang, Hongdong Li, Pan Ji, Gim Hee Lee  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30855v1.pdf)  
  Keywords: autoregressive, interactive, dit, 3d-aware, simulation, video generation, image-to-video, denoising  
- **[Full-4D: Generating Full-Scope 4D Scenes from a Single-View Video](https://arxiv.org/abs/2605.25500v1)**  
  Authors: Tingxi Chen, Ke Hao, Yabo Chen, Zhengxue Cheng, Rong Xie, Li Song, Haibin Huang, Chi Zhang, Xuelong Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25500v1.pdf)  
  Keywords: distillation, multi-view video, video diffusion, video interpolation, flow matching, physical, interactive, dit, 4d generation, diffusion model, video synthesis  
- **[Pantheon360: Taming Digital Twin Generation via 3D-Aware 360° Video Diffusion](https://arxiv.org/abs/2605.25449v1)**  
  Authors: Ting-Hsuan Chen, Ying-Huan Chen, Tao Tu, Jie-Ying Lee, Cho-Ying Wu, Fangzhou Lin, Hengyuan Zhang, David Paz, Xinyu Huang, Yuliang Guo, Yu-Lun Liu, Yue Wang, Liu Ren  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25449v1.pdf)  
  Keywords: camera control, controllable, video diffusion, temporal consistency, 3d-aware, simulation, video generation, diffusion model, trajectory  
- **[SRUG: Shadow-Guided Relightable Urban Scene with Generation Model](https://arxiv.org/abs/2605.24700v3)**  
  Authors: Yonghao Zhao, Zexin Yin, Jian Yang, Beibei Wang, Jin Xie  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.24700v3.pdf)  
  Keywords: novel view, physical, dit, evaluation  
- **[3DPhysVideo: Consistency-Guided Flow SDE for Video Generation via 3D Scene Reconstruction and Physical Simulation](https://arxiv.org/abs/2605.16795v1)**  
  Authors: Hwidong Kim, Yunho Kim, Tae-Kyun Kim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.16795v1.pdf)  
  Keywords: i2v, dynamics, physical, dit, evaluation, physics, novel view, efficient, physical simulation, simulation, video generation, image-to-video, denoising, benchmark  
- **[GTA: Advancing Image-to-3D World Generation via Geometry Then Appearance Video Diffusion](https://arxiv.org/abs/2605.12957v1)**  
  Authors: Hanxin Zhu, Cong Wang, Peiyan Tu, Jiayi Luo, Tianyu He, Xin Jin, Zhibo Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.12957v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://hanxinzhu-lab.github.io/GTA)  
  Keywords: video diffusion, dit, autonomous driving, novel view, diffusion model  
- **[GaitProtector: Impersonation-Driven Gait De-Identification via Training-Free Diffusion Latent Optimization](https://arxiv.org/abs/2605.12431v1)**  
  Authors: Huiran Duan, Qian Zhou, Zhongliang Guo, Junhao Dong, Yuqi Li, Guoying Zhao, Yingli Tian  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.12431v1.pdf)  
  Keywords: identity, dynamics, video diffusion, 3d video, diffusion model, trajectory  
- **[VidSplat: Gaussian Splatting Reconstruction with Geometry-Guided Video Diffusion Priors](https://arxiv.org/abs/2605.11424v1)**  
  Authors: Jimin Tang, Wenyuan Zhang, Junsheng Zhou, Zian Huang, Kanle Shi, Shenkun Xu, Yu-Shen Liu, Zhizhong Han  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.11424v1.pdf)  
  Keywords: video diffusion, 3d consistent, novel view, denoising, benchmark  
- **[LoViF 2026 The First Challenge on Holistic Quality Assessment for 4D World Model (PhyScore)](https://arxiv.org/abs/2605.05187v1)**  
  Authors: Wei Luo, Yiting Lu, Xin Li, Haoran Li, Fengbin Guan, Chen Gao, Xin Jin, Yong Li, Zhibo Chen, Sijing Wu, Kang Fu, Yunhao Li, Ziang Xiao, Huiyu Duan, Jing Liu, Qiang Hu, Xiongkuo Min, Guangtao Zhai, Manxi Sun, Zixuan Guo, Yun Li, Ziyang Chen, Manabu Tsukada, Zhengyang Li, Zhenglin Du, Yi Wen, Licheng Jiao, Fang Liu, Lingling Li, Yiwen Ren, Zhilong Song, Dubing Chen, Yucheng Zhou, Tianyi Yan, Huan Zheng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.05187v1.pdf)  
  Keywords: creative, dynamics, world model, temporal consistency, physical, dit, evaluation, 4d generation, physics, benchmark  
- **[AnyRecon: Arbitrary-View 3D Reconstruction with Video Diffusion Model](https://arxiv.org/abs/2604.19747v1)**  
  Authors: Yutian Chen, Shi Guo, Renbiao Jin, Tianshuo Yang, Xin Cai, Yawen Luo, Mingxin Yang, Mulin Yu, Linning Xu, Tianfan Xue  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2604.19747v1.pdf)  
  Keywords: distillation, video diffusion, dit, novel view, diffusion model  

### Applications

*Showing the latest 50 out of 53 papers*

- **[Foundation VAEs for 3D CT Reconstruction, Augmentation, and Generation](https://arxiv.org/abs/2605.30893v1)**  
  Authors: Qi Chen, Shuhan Ding, Yu Gu, Nan Liu, Jiang Bian, Alan Yuille, Zongwei Zhou, Jingjing Fu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30893v1.pdf) | [![GitHub](https://img.shields.io/github/stars/qic999/Foundation-VAE?style=social)](https://github.com/qic999/Foundation-VAE)  
  Keywords: diffusion model, dit, medical  
- **[DriveWAM: Video Generative Priors Enable Scalable World-Action Modeling for Autonomous Driving](https://arxiv.org/abs/2605.28544v1)**  
  Authors: Chen Shi, Jinrui Xu, Shaoshuai Shi, Kehua Sheng, Bo Zhang, Li Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28544v1.pdf)  
  Keywords: diffusion transformer, architecture, autoregressive, video diffusion, dynamics, physical, autonomous driving, benchmark  
- **[Turning Video Models into Generalist Robot Policies](https://arxiv.org/abs/2605.27817v1)**  
  Authors: Sizhe Lester Li, Evan Kim, Xingjian Bai, Tong Zhao, Tao Pang, Max Simchowitz, Vincent Sitzmann  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.27817v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://vera.csail.mit.edu)  
  Keywords: dynamics, world model, efficient, robotics, benchmark  
- **[AnyScene: Towards Highly Controllable Driving Scene Generation at Anywhere and Beyond](https://arxiv.org/abs/2605.26113v1)**  
  Authors: Haiming Zhang, Junfei Zhou, Feng Jiang, Jingzhong Li, Zhenglong Guo, Penglin Dai, Jifeng Dai, Yan Xie, Benjin Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.26113v1.pdf)  
  Keywords: diffusion transformer, controllable, autoregressive, dit, autonomous driving, simulation, layout, video generation, video synthesis  
- **[DexSIM: Real-time Dexterous Simulation with Unified Causal Video Diffusion](https://arxiv.org/abs/2605.24630v1)**  
  Authors: Adam Lee  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.24630v1.pdf)  
  Keywords: autoregressive, video diffusion, physical, interactive, simulation, robotics, diffusion model, trajectory  
- **[EvalVerse: Pipeline-Aware and Expert-Calibrated Benchmarking for Professional Cinematic Video Generation](https://arxiv.org/abs/2605.23271v1)**  
  Authors: Songlin Yang, Haobin Zhong, Ruilin Zhang, Xiaotong Zhao, Shuai Li, Kai Zheng, Xuyi Yang, Zhe Wang, Zhenchen Tang, Yang Li, Bohai Gu, Zhengwei Peng, Yidan Huang, Mengzhou Luo, Yihang Bo, Dalu Feng, Yujia Zhang, Juntao Ma, Ruiqi Wang, Lvmin Zhang, Yuwei Guo, Frank Guan, Maneesh Agrawala, Hongbo Fu, Alan Zhao, Anyi Rao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.23271v1.pdf)  
  Keywords: film, video generation, evaluation, benchmark  
- **[Cell Phantom Video Generation in Elliptical Fourier Descriptor Domain](https://arxiv.org/abs/2605.22563v1)**  
  Authors: Francesco Benedetto, Roberto Basla, Luca Magri, Giacomo Boracchi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.22563v1.pdf) | [![GitHub](https://img.shields.io/github/stars/FrancescoBenedetto99/efd-cell-video-gen?style=social)](https://github.com/FrancescoBenedetto99/efd-cell-video-gen)  
  Keywords: video generation, medical, efficient  
- **[CogOmniControl: Reasoning-Driven Controllable Video Generation via Creative Intent Cognition](https://arxiv.org/abs/2605.19995v1)**  
  Authors: Hongji Yang, Songlian Li, Yucheng Zhou, Xiaotong Zhao, Alan Zhao, Chengzhong Xu, Jianbing Shen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.19995v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://um-lab.github.io/CogOmniControl)  
  Keywords: controllable, architecture, creative, dit, video generation, diffusion model, benchmark  
- **[CodeBind: Decoupled Representation Learning for Multimodal Alignment with Unified Compositional Codebook](https://arxiv.org/abs/2605.18257v1)**  
  Authors: Zeyu Chen, Jie Li, Kai Han  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.18257v1.pdf)  
  Keywords: robotics, dit  
- **[Xiaomi Auto World Model: A Joint World Model Integrating Reconstruction and Generation for Autonomous Driving](https://arxiv.org/abs/2605.18137v5)**  
  Authors: Lijun Zhou, Hongcheng Luo, Zhenxin Zhu, Cheng Chi, Mingfei Tu, Kaixin Xiong, Lei Gong, Zhanqian Wu, Zehan Zhang, Fangzhen Li, Hao Li, Yingying Shen, Jiale He, Haohui Zhu, Shan Zhao, Kai Wang, Zhiwei Zhan, Yuechuan Pu, Kaiyuan Tan, Ruiling Yang, Xianqi Wang, Tianyi Yan, Jiawei Zhou, Lei Zhang, Jingyang Zhao, Xi Zhou, Chitian Sun, Chenming Wu, Jiong Deng, Hongwei Xie, Ming Lu, Kun Ma, Long Chen, Guang Chen, Hangjun Ye, Bing Wang, Haiyang Sun  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.18137v5.pdf)  
  Keywords: distillation, architecture, world model, autonomous driving, simulation, video generation, denoising  

### Architecture & Efficiency

*Showing the latest 50 out of 361 papers*

- **[Lumos-Nexus: Efficient Frequency Bridging with Homogeneous Latent Space for Video Unified Models](https://arxiv.org/abs/2605.31603v1)**  
  Authors: Jiazheng Xing, Hangjie Yuan, Lingling Cai, Xinyu Liu, Yujie Wei, Fei Du, Hai Ci, Tao Feng, Jiasheng Tang, Weihua Chen, Fan Wang, Yong Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.31603v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://jiazheng-xing.github.io/nexus-lumos-home)  
  Keywords: video generation, efficient, video synthesis, benchmark  
- **[Learning Global Motion with Compact Gaussians for Feed-Forward 4D Reconstruction](https://arxiv.org/abs/2605.31595v1)**  
  Authors: Mungyeom Kim, Minkyeong Jeon, Honggyu An, Jaewoo Jung, Hyuna Ko, Jisang Han, Hyeonseo Yu, Donghwan Shin, Sunghwan Hong, Takuya Narihira, Kazumi Fukuda, Yuki Mitsufuji, Seungryong Kim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.31595v1.pdf)  
  Keywords: diffusion model, dit, video diffusion  
- **[TunerDiT: Training-free Progressive Steering of Diffusion Transformer for Multi-Event Video Generation](https://arxiv.org/abs/2605.31590v1)**  
  Authors: Ruotong Liao, Guowen Huang, Qing Cheng, Guangyao Zhai, Lei Zhang, Xun Xiao, Thomas Seidl, Daniel Cremers, Volker Tresp  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.31590v1.pdf)  
  Keywords: t2v, diffusion transformer, video diffusion, text-to-video, dit, layout, video generation, denoising, trajectory, benchmark  
- **[DecMem: Towards Minute-Long Consistent World Generation with Decoupled Memory](https://arxiv.org/abs/2605.31336v1)**  
  Authors: Zhenhao Yang, Xiaoshi Wu, Zhengyao Lv, Xiaoyu Shi, Xintao Wang, Pengfei Wan, Kun Gai, Kwan-Yee K. Wong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.31336v1.pdf)  
  Keywords: long video, controllable, architecture, world model, temporal consistency, efficient, video generation  
- **[Vanilla ViT for Automotive Point Cloud Semantic Segmentation](https://arxiv.org/abs/2605.31177v1)**  
  Authors: Gilles Puy, Nermin Samet, Alexandre Boulch, Spyros Gidaris, Tuan-Hung VU, Renaud Marlet  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.31177v1.pdf) | [![GitHub](https://img.shields.io/github/stars/valeoai/VaViT?style=social)](https://github.com/valeoai/VaViT)  
  Keywords: architecture, evaluation  
- **[Foundation VAEs for 3D CT Reconstruction, Augmentation, and Generation](https://arxiv.org/abs/2605.30893v1)**  
  Authors: Qi Chen, Shuhan Ding, Yu Gu, Nan Liu, Jiang Bian, Alan Yuille, Zongwei Zhou, Jingjing Fu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30893v1.pdf) | [![GitHub](https://img.shields.io/github/stars/qic999/Foundation-VAE?style=social)](https://github.com/qic999/Foundation-VAE)  
  Keywords: diffusion model, dit, medical  
- **[Robust Dreamer: Deviation-Aware Latent Gaussian Memory for Action-Controlled AR Video Generation](https://arxiv.org/abs/2605.30855v1)**  
  Authors: Hanlin Chen, Jiaxin Wei, Xibin Song, Yifu Wang, Steve Wang, Hongdong Li, Pan Ji, Gim Hee Lee  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30855v1.pdf)  
  Keywords: autoregressive, interactive, dit, 3d-aware, simulation, video generation, image-to-video, denoising  
- **[CameraNoise: Enabling Faithful Camera Control in Video Diffusion through Geometry-Flow-Guided Noise Warping](https://arxiv.org/abs/2605.30774v1)**  
  Authors: Haoyu Zhao, Jiaxi Gu, Haoran Chen, Qingping Zheng, Yeying Jin, Hongyi Yang, Junqi Cheng, Yuang Zhang, Zenghui Lu, Huan Yu, Jie Jiang, Peng Shu, Zuxuan Wu, Yu-Gang Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30774v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://gulucaptain.github.io/CameraNoise)  
  Keywords: camera control, dynamics, video diffusion, dit, trajectory  
- **[DTG-Restore: Training-Free Diffusion Refinement for Generative Video Super-Resolution](https://arxiv.org/abs/2605.30431v1)**  
  Authors: Hidir Yesiltepe, Koutilya PNVR, Gaurav Pathak, Navaneeth Bodla, Bharat Singh, Pinar Yanardag, Jinrong Xie  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30431v1.pdf)  
  Keywords: video diffusion, text-to-video, dit, evaluation, super-resolution, diffusion model, benchmark  
- **[AdaState: Self-Evolving Anchors for Streaming Video Generation](https://arxiv.org/abs/2605.30349v1)**  
  Authors: Yusuf Dalva, Pinar Yanardag  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30349v1.pdf)  
  Keywords: denoising, autoregressive, video diffusion, dynamics, streaming, dit, video generation, diffusion model  

### Audio & Multi-modal

- **[LongCat-Video-Avatar 1.5 Technical Report](https://arxiv.org/abs/2605.26486v1)**  
  Authors: Meituan LongCat Team, Xunliang Cai, Meng Cheng, Feng Gao, Zhe Kong, Jiamu Li, Le Li, Weiheng Li, Hongyu Liu, Shuai Tan, Xiaoming Wei, Tianyu Yang, Yong Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.26486v1.pdf)  
  Keywords: audio-driven, distillation, identity, dit, evaluation, video generation, avatar, benchmark  
- **[StreamChar: Long-Horizon Streaming Character Audio-Video Generation with Decoupled Orchestration](https://arxiv.org/abs/2605.25659v1)**  
  Authors: Linrui Tian, Qi Wang, Bang Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25659v1.pdf)  
  Keywords: audio-driven, distillation, identity, autoregressive, streaming, dit, efficient, video generation, denoising  
- **[Test-Time Self-Adaptive Conditioning for Stable Audio-Driven Talking-Head Generation](https://arxiv.org/abs/2605.25488v1)**  
  Authors: Zhicheng Zhang, Lei Wang, Yu Zhang, Yongsheng Gao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25488v1.pdf)  
  Keywords: identity, dynamics, video generation, dit, audio-driven, benchmark  
- **[AVBench: Human-Aligned and Automated Evaluation Benchmark for Audio-Video Generative Models](https://arxiv.org/abs/2605.24652v1)**  
  Authors: Jialiang Yang, Bin Xia, Ruihang Chu, Dingdong Wang, Wanke Xia, Zhun Mou, Tianyang Zhong, Yiting Zhao, Wenming Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.24652v1.pdf)  
  Keywords: dit, evaluation, style, sound, benchmark  
- **[What Semantics Survive the Connector? Diagnosing VLM-to-DiT Alignment in Video Editing](https://arxiv.org/abs/2605.20795v1)**  
  Authors: Hangyu Lin, Chao Wen, Chengming Xu, Jianxiong Gao, Jiangning Zhang, Xiaobin Hu, Yanwei Fu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20795v1.pdf)  
  Keywords: architecture, flow matching, video editing, dit, evaluation, multi-modal  
- **[Sound Sparks Motion: Audio and Text Tuning for Video Editing](https://arxiv.org/abs/2605.15307v1)**  
  Authors: AmirHossein Naghi Razlighi, Aryan Mikaeili, Ali Mahdavi-Amiri, Daniel Cohen-Or, Yiorgos Chrysanthou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.15307v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://amirhossein-razlighi.github.io/Sound_Sparks_Motion)  
  Keywords: video editing, dit, motion control, video generation, sound  
- **[OmniNFT: Modality-wise Omni Diffusion Reinforcement for Joint Audio-Video Generation](https://arxiv.org/abs/2605.12480v1)**  
  Authors: Guohui Zhang, XiaoXiao Ma, Jie Huang, Hang Xu, Hu Yu, Siming Fu, Yuming Li, Zeyue Xue, Lin Song, Haoyang Huang, Nan Duan, Feng Zhao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.12480v1.pdf)  
  Keywords: video generation, multi-modal, dit, efficient  
- **[AllocMV: Optimal Resource Allocation for Music Video Generation via Structured Persistent State](https://arxiv.org/abs/2605.10723v1)**  
  Authors: Huimin Wang, Leilei Ouyang, Chang Xia, Yongqi Kang, Yu Fu, Yuqi Ouyang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.10723v1.pdf)  
  Keywords: music video, video generation, dit, video synthesis  
- **[Omni-DeepSearch: A Benchmark for Audio-Driven Omni-Modal Deep Search](https://arxiv.org/abs/2605.08762v1)**  
  Authors: Tao Yu, yiming ding, Shenghua Chai, Minghui Zhang, Zhongtian Luo, Xinming Wang, Xinlong Chen, Zhaolu Kang, Junhao Gong, Yuxuan Zhou, Haopeng Jin, Zhiqing Cui, Jiabing Yang, YiFan Zhang, Hongzhu Yi, Zheqi He, Xi Yang, Yan Huang, Liang Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.08762v1.pdf)  
  Keywords: audio-driven, benchmark  
- **[Unison: Harmonizing Motion, Speech, and Sound for Human-Centric Audio-Video Generation](https://arxiv.org/abs/2605.08729v1)**  
  Authors: Shihao Cheng, Jiaxu Zhang, Quanyue Song, Shansong Liu, Zhizhi Guo, Xiaolei Zhang, Chi Zhang, Xuelong Li, Zhigang Tu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.08729v1.pdf)  
  Keywords: video generation, sound, denoising, dit  

### Controllable Generation

*Showing the latest 50 out of 131 papers*

- **[TunerDiT: Training-free Progressive Steering of Diffusion Transformer for Multi-Event Video Generation](https://arxiv.org/abs/2605.31590v1)**  
  Authors: Ruotong Liao, Guowen Huang, Qing Cheng, Guangyao Zhai, Lei Zhang, Xun Xiao, Thomas Seidl, Daniel Cremers, Volker Tresp  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.31590v1.pdf)  
  Keywords: t2v, diffusion transformer, video diffusion, text-to-video, dit, layout, video generation, denoising, trajectory, benchmark  
- **[DecMem: Towards Minute-Long Consistent World Generation with Decoupled Memory](https://arxiv.org/abs/2605.31336v1)**  
  Authors: Zhenhao Yang, Xiaoshi Wu, Zhengyao Lv, Xiaoyu Shi, Xintao Wang, Pengfei Wan, Kun Gai, Kwan-Yee K. Wong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.31336v1.pdf)  
  Keywords: long video, controllable, architecture, world model, temporal consistency, efficient, video generation  
- **[CameraNoise: Enabling Faithful Camera Control in Video Diffusion through Geometry-Flow-Guided Noise Warping](https://arxiv.org/abs/2605.30774v1)**  
  Authors: Haoyu Zhao, Jiaxi Gu, Haoran Chen, Qingping Zheng, Yeying Jin, Hongyi Yang, Junqi Cheng, Yuang Zhang, Zenghui Lu, Huan Yu, Jie Jiang, Peng Shu, Zuxuan Wu, Yu-Gang Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30774v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://gulucaptain.github.io/CameraNoise)  
  Keywords: camera control, dynamics, video diffusion, dit, trajectory  
- **[VideoMLA: Low-Rank Latent KV Cache for Minute-Scale Autoregressive Video Diffusion](https://arxiv.org/abs/2605.30351v1)**  
  Authors: Hidir Yesiltepe, Jiazhen Hu, Tuna Han Salih Meral, Adil Kaan Akan, Kaan Oktay, Hoda Eldardiry, Pinar Yanardag  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30351v1.pdf)  
  Keywords: layout, streaming, autoregressive, video diffusion  
- **[minWM: A Full-Stack Open-Source Framework for Real-Time Interactive Video World Models](https://arxiv.org/abs/2605.30263v1)**  
  Authors: Min Zhao, Hongzhou Zhu, Bokai Yan, Zihan Zhou, Yimin Chen, Wenqiang Sun, Kaiwen Zheng, Guande He, Xiao Yang, Chongxuan Li, Fan Bao, Jun Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30263v1.pdf) | [![GitHub](https://img.shields.io/github/stars/shengshu-ai/minWM?style=social)](https://github.com/shengshu-ai/minWM)  
  Keywords: t2v, i2v, camera control, controllable, architecture, autoregressive, video diffusion, world model, distillation, streaming, interactive, dit, style, video generation, diffusion model, trajectory  
- **[Native Audio-Visual Alignment for Generation](https://arxiv.org/abs/2605.30073v1)**  
  Authors: Longbin Ji, Guan Wang, Xuan Wei, Chenye Yang, Xiangrui Liu, Zhenyu Zhang, Shuohuan Wang, Yu Sun, Jingzhou He  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30073v1.pdf)  
  Keywords: controllable, architecture, dit, video generation, denoising  
- **[Gamma-World: Generative Multi-Agent World Modeling Beyond Two Players](https://arxiv.org/abs/2605.28816v1)**  
  Authors: Fangfu Liu, Kai He, Tianchang Shen, Tianshi Cao, Sanja Fidler, Yueqi Duan, Jun Gao, Igor Gilitschenski, Zian Wang, Xuanchi Ren  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28816v1.pdf)  
  Keywords: controllable, identity, world model, interactive, dit, efficient, simulation, video generation  
- **[CogPortrait: Fine-Grained Eye-Region Control in Portrait Animation via Hierarchical Agent Planning](https://arxiv.org/abs/2605.28056v1)**  
  Authors: He Feng, Yongjia Ma, Donglin Di, Lei Fan, Tonghua Su  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28056v1.pdf)  
  Keywords: identity, dynamics, dit, motion control, video generation, benchmark  
- **[Timestep-Aware SVDQuant-GPTQ for W4A4 Quantization of Wan2.2-I2V](https://arxiv.org/abs/2605.27003v1)**  
  Authors: Junhao Wu, Dezhong Yao, Hai Jin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.27003v1.pdf)  
  Keywords: diffusion transformer, i2v, video diffusion, dit, denoising, trajectory, benchmark  
- **[E$^3$C: Video Generation with 3D Environmental Memory and Ego-Exo Human Pose Control](https://arxiv.org/abs/2605.26316v1)**  
  Authors: Qiao Gu, Lingni Ma, Adam W Harley, Richard Newcombe, Florian Shkurti, Julian Straub  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.26316v1.pdf)  
  Keywords: controllable, dynamics, video diffusion, physical, dit, video generation, video synthesis  

### Human & Character Animation

- **[Archon: A Unified Multimodal Model for Holistic Digital Human Generation](https://arxiv.org/abs/2605.30311v1)**  
  Authors: Chong Bao, Shichen Liu, Lijun Yu, David Futschik, Stylianos Moschoglou, Shefali Srivastava, Ziqian Bai, Feitong Tan, Guofeng Zhang, Zhaopeng Cui, Sean Fanello, Yinda Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30311v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://zju3dv.github.io/archon)  
  Keywords: dynamics, autoregressive, video diffusion, efficient, avatar  
- **[LongCat-Video-Avatar 1.5 Technical Report](https://arxiv.org/abs/2605.26486v1)**  
  Authors: Meituan LongCat Team, Xunliang Cai, Meng Cheng, Feng Gao, Zhe Kong, Jiamu Li, Le Li, Weiheng Li, Hongyu Liu, Shuai Tan, Xiaoming Wei, Tianyu Yang, Yong Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.26486v1.pdf)  
  Keywords: audio-driven, distillation, identity, dit, evaluation, video generation, avatar, benchmark  
- **[RoMo: A Large-Scale, Richly Organized Dataset and Semantic Taxonomy for Human Motion Generation](https://arxiv.org/abs/2605.26241v1)**  
  Authors: Jiahao Zhang, Joseph Liu, Young-Yoon Lee, Seonghyeon Moon, Victor Zordan, Guy Tevet, Karen Liu, Stephen Gould, Oren Jacob, Haomiao Jiang, Mubbasir Kapadia, Yizhak Ben-Shabat  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.26241v1.pdf)  
  Keywords: human motion, evaluation  
- **[iTryOn: Mastering Interactive Video Virtual Try-On with Spatial-Semantic Guidance](https://arxiv.org/abs/2605.21431v1)**  
  Authors: Jun Zheng, Zhengze Xu, Mengting Chen, Jing Wang, Jinsong Lan, Xiaoyong Zhu, Kaifu Zhang, Bo Zheng, Xiaodan Liang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.21431v1.pdf)  
  Keywords: diffusion transformer, controllable, dynamics, video diffusion, virtual try-on, temporal consistency, interactive, dit, benchmark  
- **[EverAnimate: Minute-Scale Human Animation via Latent Flow Restoration](https://arxiv.org/abs/2605.15042v1)**  
  Authors: Wuyang Li, Yang Gao, Mariam Hassan, Lan Feng, Wentao Pan, Po-Chien Luan, Alexandre Alahi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.15042v1.pdf)  
  Keywords: identity, flow matching, human motion, long-form, efficient, video generation, human animation  
- **[PhyMotion: Structured 3D Motion Reward for Physics-Grounded Human Video Generation](https://arxiv.org/abs/2605.14269v1)**  
  Authors: Yidong Huang, Zun Wang, Han Lin, Dong-Ki Kim, Shayegan Omidshafiei, Jaehong Yoon, Jaemin Cho, Yue Zhang, Mohit Bansal  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.14269v1.pdf)  
  Keywords: autoregressive, dynamics, physical, human motion, physics, evaluation, video generation  
- **[SocialDirector: Training-Free Social Interaction Control for Multi-Person Video Generation](https://arxiv.org/abs/2605.10079v1)**  
  Authors: Liangyang Ouyang, Ruicong Liu, Caixin Kang, Yifei Huang, Yoichi Sato  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.10079v1.pdf)  
  Keywords: dynamics, evaluation, gesture, robotics, film, video generation  
- **[MoCoTalk: Multi-Conditional Diffusion with Adaptive Router for Controllable Talking Head Generation](https://arxiv.org/abs/2605.08050v1)**  
  Authors: Xinyan Ye, Jiankang Deng, Abbas Edalat  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.08050v1.pdf)  
  Keywords: controllable, identity, dynamics, video diffusion, dit, talking head  
- **[Omni-Fake: Benchmarking Unified Multimodal Social Media Deepfake Detection](https://arxiv.org/abs/2605.01638v1)**  
  Authors: Tianxiao Li, Zhenglin Huang, Haiquan Wen, Yiwei He, Xinze Li, Bingyu Zhu, Wuhui Duan, Congang Chen, Zeyu Fu, Yi Dong, Baoyuan Wu, Jason Li, Guangliang Cheng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.01638v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://tianxiao1201.github.io/omni-fake-project-page)  
  Keywords: dit, talking head, benchmark  
- **[Generate Your Talking Avatar from Video Reference](https://arxiv.org/abs/2604.27918v1)**  
  Authors: Zujin Guo, Zhenhui Ye, Yi Ren, Yuanming Li, Ce Chen, Zhibin Hong, Chen Change Loy  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2604.27918v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://www.heygen.com/research)  
  Keywords: identity, dit, avatar, image-to-video, benchmark  

### Image-to-Video Generation

- **[Robust Dreamer: Deviation-Aware Latent Gaussian Memory for Action-Controlled AR Video Generation](https://arxiv.org/abs/2605.30855v1)**  
  Authors: Hanlin Chen, Jiaxin Wei, Xibin Song, Yifu Wang, Steve Wang, Hongdong Li, Pan Ji, Gim Hee Lee  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30855v1.pdf)  
  Keywords: autoregressive, interactive, dit, 3d-aware, simulation, video generation, image-to-video, denoising  
- **[minWM: A Full-Stack Open-Source Framework for Real-Time Interactive Video World Models](https://arxiv.org/abs/2605.30263v1)**  
  Authors: Min Zhao, Hongzhou Zhu, Bokai Yan, Zihan Zhou, Yimin Chen, Wenqiang Sun, Kaiwen Zheng, Guande He, Xiao Yang, Chongxuan Li, Fan Bao, Jun Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30263v1.pdf) | [![GitHub](https://img.shields.io/github/stars/shengshu-ai/minWM?style=social)](https://github.com/shengshu-ai/minWM)  
  Keywords: t2v, i2v, camera control, controllable, architecture, autoregressive, video diffusion, world model, distillation, streaming, interactive, dit, style, video generation, diffusion model, trajectory  
- **[LiveSVG: Zero-Shot SVG Animation via Video Generation](https://arxiv.org/abs/2605.30174v1)**  
  Authors: Matan Levy, Ran Margolin, Bar Cavia, Dvir Samuel, Yael Pritch, Shmuel Peleg, Alex Rav Acha, Ariel Shamir, Dani Lischinski  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30174v1.pdf)  
  Keywords: distillation, video diffusion, dit, evaluation, video generation, image-to-video, diffusion model, benchmark  
- **[Proprio: Latent Self-Scoring and Inference-Time Refinement for Physically Plausible Video Generation](https://arxiv.org/abs/2605.28230v1)**  
  Authors: Mariam Hassan, Kaouther Messaoud, Wuyang Li, Alexandre Alahi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28230v1.pdf)  
  Keywords: dynamics, physical, text-to-video, evaluation, physics, video generation, image-to-video, benchmark  
- **[VidPrism: Heterogeneous Mixture of Experts for Image-to-Video Transfer](https://arxiv.org/abs/2605.28229v1)**  
  Authors: Rui Lin, Chuanming Wang, Huadong Ma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28229v1.pdf) | [![GitHub](https://img.shields.io/github/stars/Lrrrr549/VidPrism.git?style=social)](https://github.com/Lrrrr549/VidPrism.git)  
  Keywords: efficient, image-to-video, benchmark  
- **[PARE: Pruning and Adaptive Routing for Efficient Video Generation](https://arxiv.org/abs/2605.27336v1)**  
  Authors: Yutong Wang, Yunke Wang, Tianfan Xue, Yu Qiao, Yaohui Wang, Xinyuan Chen, Chang Xu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.27336v1.pdf)  
  Keywords: diffusion transformer, distillation, acceleration, architecture, video diffusion, text-to-video, dit, efficient, video generation, image-to-video, denoising  
- **[Timestep-Aware SVDQuant-GPTQ for W4A4 Quantization of Wan2.2-I2V](https://arxiv.org/abs/2605.27003v1)**  
  Authors: Junhao Wu, Dezhong Yao, Hai Jin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.27003v1.pdf)  
  Keywords: diffusion transformer, i2v, video diffusion, dit, denoising, trajectory, benchmark  
- **[Teaching Video Generators to Remember: Eliciting Dynamic Memory for Out-of-Sight State Evolution](https://arxiv.org/abs/2605.25333v1)**  
  Authors: Tianshuo Xu, Yichen Xie, Depu Meng, Chensheng Peng, Quentin Herau, Bo Jiang, Yihan Hu, Wei Zhan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25333v1.pdf)  
  Keywords: diffusion transformer, dynamics, video diffusion, world model, evaluation, image-to-video  
- **[SimInsert: Seamless Video Object Insertion via Regional Sparse Attention Fusion](https://arxiv.org/abs/2605.23245v1)**  
  Authors: Xinyu Chen, Yuyi Qian, Jiang Lin, Shenyi Wang, Gao Wang, Zhiqiu Zhang, Jizhi Zhang, Mingjie Wang, Qiang Tang, Qian Wang, Song Wu, Zili Yi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.23245v1.pdf)  
  Keywords: denoising, video diffusion, video editing, interactive, dit, efficient, image-to-video, diffusion model, trajectory  
- **[MotiMotion: Motion-Controlled Video Generation with Visual Reasoning](https://arxiv.org/abs/2605.22818v1)**  
  Authors: Lee Hsin-Ying, Hanwen Jiang, Yiqun Mei, Jing Shi, Ming-Hsuan Yang, Zhixin Shu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.22818v1.pdf)  
  Keywords: evaluation, motion control, video generation, image-to-video, benchmark  

### Long Video Generation

*Showing the latest 50 out of 133 papers*

- **[DecMem: Towards Minute-Long Consistent World Generation with Decoupled Memory](https://arxiv.org/abs/2605.31336v1)**  
  Authors: Zhenhao Yang, Xiaoshi Wu, Zhengyao Lv, Xiaoyu Shi, Xintao Wang, Pengfei Wan, Kun Gai, Kwan-Yee K. Wong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.31336v1.pdf)  
  Keywords: long video, controllable, architecture, world model, temporal consistency, efficient, video generation  
- **[LVSA: Training-Free Sparse Attention for Long Video Diffusion](https://arxiv.org/abs/2605.31057v1)**  
  Authors: Gael Glorian, Ioannis Lamprou, Zhen Zhang, Yujie Yuan, Hongsheng Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.31057v1.pdf)  
  Keywords: long video, diffusion transformer, video diffusion  
- **[SlotMemory: Object-Centric KV Memory for Streaming Long-Video Generation](https://arxiv.org/abs/2605.31033v1)**  
  Authors: Weijia Dou, Hui Li, Jiahao Cui, Lei Zhou, Jingdong Wang, Siyu Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.31033v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://tj12323.github.io/SlotMemory)  
  Keywords: t2v, identity, video diffusion, streaming, interactive, long-form, video generation, video synthesis  
- **[Robust Dreamer: Deviation-Aware Latent Gaussian Memory for Action-Controlled AR Video Generation](https://arxiv.org/abs/2605.30855v1)**  
  Authors: Hanlin Chen, Jiaxin Wei, Xibin Song, Yifu Wang, Steve Wang, Hongdong Li, Pan Ji, Gim Hee Lee  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30855v1.pdf)  
  Keywords: autoregressive, interactive, dit, 3d-aware, simulation, video generation, image-to-video, denoising  
- **[OmniMem: Scalable and Adaptive Memory Retrieval for Long Video Generation](https://arxiv.org/abs/2605.30519v1)**  
  Authors: Lin Zhao, Yushu Wu, Yifan Gong, Yanzhi Wang, Pu Zhao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30519v1.pdf)  
  Keywords: long video, video generation, autoregressive  
- **[VideoMLA: Low-Rank Latent KV Cache for Minute-Scale Autoregressive Video Diffusion](https://arxiv.org/abs/2605.30351v1)**  
  Authors: Hidir Yesiltepe, Jiazhen Hu, Tuna Han Salih Meral, Adil Kaan Akan, Kaan Oktay, Hoda Eldardiry, Pinar Yanardag  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30351v1.pdf)  
  Keywords: layout, streaming, autoregressive, video diffusion  
- **[AdaState: Self-Evolving Anchors for Streaming Video Generation](https://arxiv.org/abs/2605.30349v1)**  
  Authors: Yusuf Dalva, Pinar Yanardag  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30349v1.pdf)  
  Keywords: denoising, autoregressive, video diffusion, dynamics, streaming, dit, video generation, diffusion model  
- **[Veda: Scalable Video Diffusion via Distilled Sparse Attention](https://arxiv.org/abs/2605.30325v1)**  
  Authors: Shihao Han, Hao Yang, Xinting Hu, Xiaofeng Mei, Yi Jiang, Xiaojuan Qi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30325v1.pdf)  
  Keywords: t2v, long video, diffusion transformer, video diffusion, efficient, acceleration, diffusion model  
- **[VPG: Visual Prefix Guidance for Autoregressive Image and Video Generation](https://arxiv.org/abs/2605.30317v1)**  
  Authors: Xinyao Liao, Qiyuan He, Yicong Li, Jiayin Zhu, Xiaoye Qu, Wei Wei, Angela Yao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30317v1.pdf)  
  Keywords: autoregressive, dit, text-to-video, video generation, benchmark  
- **[Archon: A Unified Multimodal Model for Holistic Digital Human Generation](https://arxiv.org/abs/2605.30311v1)**  
  Authors: Chong Bao, Shichen Liu, Lijun Yu, David Futschik, Stylianos Moschoglou, Shefali Srivastava, Ziqian Bai, Feitong Tan, Guofeng Zhang, Zhaopeng Cui, Sean Fanello, Yinda Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30311v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://zju3dv.github.io/archon)  
  Keywords: dynamics, autoregressive, video diffusion, efficient, avatar  

### Personalization & Customization

*Showing the latest 50 out of 84 papers*

- **[SlotMemory: Object-Centric KV Memory for Streaming Long-Video Generation](https://arxiv.org/abs/2605.31033v1)**  
  Authors: Weijia Dou, Hui Li, Jiahao Cui, Lei Zhou, Jingdong Wang, Siyu Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.31033v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://tj12323.github.io/SlotMemory)  
  Keywords: t2v, identity, video diffusion, streaming, interactive, long-form, video generation, video synthesis  
- **[minWM: A Full-Stack Open-Source Framework for Real-Time Interactive Video World Models](https://arxiv.org/abs/2605.30263v1)**  
  Authors: Min Zhao, Hongzhou Zhu, Bokai Yan, Zihan Zhou, Yimin Chen, Wenqiang Sun, Kaiwen Zheng, Guande He, Xiao Yang, Chongxuan Li, Fan Bao, Jun Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30263v1.pdf) | [![GitHub](https://img.shields.io/github/stars/shengshu-ai/minWM?style=social)](https://github.com/shengshu-ai/minWM)  
  Keywords: t2v, i2v, camera control, controllable, architecture, autoregressive, video diffusion, world model, distillation, streaming, interactive, dit, style, video generation, diffusion model, trajectory  
- **[SGMD: Score Gradient Matching Distillation for Few-Step Video Diffusion Distillation](https://arxiv.org/abs/2605.30116v1)**  
  Authors: Zhuguanyu Wu, Ruihao Gong, Yang Yong, Yushi Huang, Xiangyu Fan, Lei Yang, Dahua Lin, Xianglong Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30116v1.pdf) | [![GitHub](https://img.shields.io/github/stars/ModelTC/LightX2V?style=social)](https://github.com/ModelTC/LightX2V)  
  Keywords: distillation, dynamics, video diffusion, temporal consistency, style, diffusion model  
- **[KGEdit: Ambiguity-Aware Knowledge Graphs for Training-Free Precise Video Generation and Editing](https://arxiv.org/abs/2605.29509v1)**  
  Authors: Mingshu Cai, Miao Zhang, Chenghe Yang, Yixuan Li, Osamu Yoshie, Yuya Ieiri  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.29509v1.pdf)  
  Keywords: t2v, diffusion transformer, denoising, identity, temporal consistency, text-to-video, dit, video generation, diffusion model, concept  
- **[Gamma-World: Generative Multi-Agent World Modeling Beyond Two Players](https://arxiv.org/abs/2605.28816v1)**  
  Authors: Fangfu Liu, Kai He, Tianchang Shen, Tianshi Cao, Sanja Fidler, Yueqi Duan, Jun Gao, Igor Gilitschenski, Zian Wang, Xuanchi Ren  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28816v1.pdf)  
  Keywords: controllable, identity, world model, interactive, dit, efficient, simulation, video generation  
- **[Which Pretraining Paradigm Better Serves Spatial Intelligence? An Empirical Comparison of Vision-Language and Video Generation Models](https://arxiv.org/abs/2605.28132v1)**  
  Authors: Haozhan Shen, Tiancheng Zhao, Kangjia Zhao, Jianwei Yin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28132v1.pdf) | [![GitHub](https://img.shields.io/github/stars/om-ai-lab/Probing-VLM-VGM?style=social)](https://github.com/om-ai-lab/Probing-VLM-VGM)  
  Keywords: video generation, physical, concept  
- **[CogPortrait: Fine-Grained Eye-Region Control in Portrait Animation via Hierarchical Agent Planning](https://arxiv.org/abs/2605.28056v1)**  
  Authors: He Feng, Yongjia Ma, Donglin Di, Lei Fan, Tonghua Su  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28056v1.pdf)  
  Keywords: identity, dynamics, dit, motion control, video generation, benchmark  
- **[PlayClass: Automated Play Behaviour Classification in Poultry](https://arxiv.org/abs/2605.27304v1)**  
  Authors: Prince Ravi Leow, Neil Scheidwasser, Rebecca Oscarsson, Per Jensen, Samir Bhatt, David Alejandro Duchêne  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.27304v1.pdf)  
  Keywords: identity  
- **[ReCA: Multi-Shot Long Video Extrapolation via Recursive Context Allocation](https://arxiv.org/abs/2605.26525v1)**  
  Authors: Akide Liu, Jinbo Xing, Chaojie Mao, Ye Li, Zeyu Zhang, Yefei He, Weijie Wang, Zihan Wang, Yu Liu, Gholamreza Haffari, Bohan Zhuang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.26525v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://reca.vmv.re)  
  Keywords: long video, video generation, identity, benchmark  
- **[LongCat-Video-Avatar 1.5 Technical Report](https://arxiv.org/abs/2605.26486v1)**  
  Authors: Meituan LongCat Team, Xunliang Cai, Meng Cheng, Feng Gao, Zhe Kong, Jiamu Li, Le Li, Weiheng Li, Hongyu Liu, Shuai Tan, Xiaoming Wei, Tianyu Yang, Yong Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.26486v1.pdf)  
  Keywords: audio-driven, distillation, identity, dit, evaluation, video generation, avatar, benchmark  

### Physical Understanding

*Showing the latest 50 out of 150 papers*

- **[CameraNoise: Enabling Faithful Camera Control in Video Diffusion through Geometry-Flow-Guided Noise Warping](https://arxiv.org/abs/2605.30774v1)**  
  Authors: Haoyu Zhao, Jiaxi Gu, Haoran Chen, Qingping Zheng, Yeying Jin, Hongyi Yang, Junqi Cheng, Yuang Zhang, Zenghui Lu, Huan Yu, Jie Jiang, Peng Shu, Zuxuan Wu, Yu-Gang Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30774v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://gulucaptain.github.io/CameraNoise)  
  Keywords: camera control, dynamics, video diffusion, dit, trajectory  
- **[AdaState: Self-Evolving Anchors for Streaming Video Generation](https://arxiv.org/abs/2605.30349v1)**  
  Authors: Yusuf Dalva, Pinar Yanardag  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30349v1.pdf)  
  Keywords: denoising, autoregressive, video diffusion, dynamics, streaming, dit, video generation, diffusion model  
- **[Archon: A Unified Multimodal Model for Holistic Digital Human Generation](https://arxiv.org/abs/2605.30311v1)**  
  Authors: Chong Bao, Shichen Liu, Lijun Yu, David Futschik, Stylianos Moschoglou, Shefali Srivastava, Ziqian Bai, Feitong Tan, Guofeng Zhang, Zhaopeng Cui, Sean Fanello, Yinda Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30311v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://zju3dv.github.io/archon)  
  Keywords: dynamics, autoregressive, video diffusion, efficient, avatar  
- **[SGMD: Score Gradient Matching Distillation for Few-Step Video Diffusion Distillation](https://arxiv.org/abs/2605.30116v1)**  
  Authors: Zhuguanyu Wu, Ruihao Gong, Yang Yong, Yushi Huang, Xiangyu Fan, Lei Yang, Dahua Lin, Xianglong Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30116v1.pdf) | [![GitHub](https://img.shields.io/github/stars/ModelTC/LightX2V?style=social)](https://github.com/ModelTC/LightX2V)  
  Keywords: distillation, dynamics, video diffusion, temporal consistency, style, diffusion model  
- **[HarmoVid: Relightful Video Portrait Harmonization](https://arxiv.org/abs/2605.28811v1)**  
  Authors: Jun Myeong Choi, Jae Shin Yoon, Luchao Qi, Roni Sengupta, Joon-Young Lee  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28811v1.pdf)  
  Keywords: physical, diffusion model, dit, video diffusion  
- **[DriveWAM: Video Generative Priors Enable Scalable World-Action Modeling for Autonomous Driving](https://arxiv.org/abs/2605.28544v1)**  
  Authors: Chen Shi, Jinrui Xu, Shaoshuai Shi, Kehua Sheng, Bo Zhang, Li Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28544v1.pdf)  
  Keywords: diffusion transformer, architecture, autoregressive, video diffusion, dynamics, physical, autonomous driving, benchmark  
- **[Sketch2Motion: Text-driven 2D Sketch to 3D Animation via Diffusion-guided Skeleton Optimization](https://arxiv.org/abs/2605.28394v1)**  
  Authors: Gaurav Rai, Ojaswa Sharma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28394v1.pdf)  
  Keywords: distillation, video diffusion, physical, dit, text-to-video, physics, diffusion model  
- **[Proprio: Latent Self-Scoring and Inference-Time Refinement for Physically Plausible Video Generation](https://arxiv.org/abs/2605.28230v1)**  
  Authors: Mariam Hassan, Kaouther Messaoud, Wuyang Li, Alexandre Alahi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28230v1.pdf)  
  Keywords: dynamics, physical, text-to-video, evaluation, physics, video generation, image-to-video, benchmark  
- **[Which Pretraining Paradigm Better Serves Spatial Intelligence? An Empirical Comparison of Vision-Language and Video Generation Models](https://arxiv.org/abs/2605.28132v1)**  
  Authors: Haozhan Shen, Tiancheng Zhao, Kangjia Zhao, Jianwei Yin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28132v1.pdf) | [![GitHub](https://img.shields.io/github/stars/om-ai-lab/Probing-VLM-VGM?style=social)](https://github.com/om-ai-lab/Probing-VLM-VGM)  
  Keywords: video generation, physical, concept  
- **[CogPortrait: Fine-Grained Eye-Region Control in Portrait Animation via Hierarchical Agent Planning](https://arxiv.org/abs/2605.28056v1)**  
  Authors: He Feng, Yongjia Ma, Donglin Di, Lei Fan, Tonghua Su  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28056v1.pdf)  
  Keywords: identity, dynamics, dit, motion control, video generation, benchmark  

### Surveys & Benchmarks

*Showing the latest 50 out of 227 papers*

- **[Lumos-Nexus: Efficient Frequency Bridging with Homogeneous Latent Space for Video Unified Models](https://arxiv.org/abs/2605.31603v1)**  
  Authors: Jiazheng Xing, Hangjie Yuan, Lingling Cai, Xinyu Liu, Yujie Wei, Fei Du, Hai Ci, Tao Feng, Jiasheng Tang, Weihua Chen, Fan Wang, Yong Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.31603v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://jiazheng-xing.github.io/nexus-lumos-home)  
  Keywords: video generation, efficient, video synthesis, benchmark  
- **[TunerDiT: Training-free Progressive Steering of Diffusion Transformer for Multi-Event Video Generation](https://arxiv.org/abs/2605.31590v1)**  
  Authors: Ruotong Liao, Guowen Huang, Qing Cheng, Guangyao Zhai, Lei Zhang, Xun Xiao, Thomas Seidl, Daniel Cremers, Volker Tresp  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.31590v1.pdf)  
  Keywords: t2v, diffusion transformer, video diffusion, text-to-video, dit, layout, video generation, denoising, trajectory, benchmark  
- **[Vanilla ViT for Automotive Point Cloud Semantic Segmentation](https://arxiv.org/abs/2605.31177v1)**  
  Authors: Gilles Puy, Nermin Samet, Alexandre Boulch, Spyros Gidaris, Tuan-Hung VU, Renaud Marlet  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.31177v1.pdf) | [![GitHub](https://img.shields.io/github/stars/valeoai/VaViT?style=social)](https://github.com/valeoai/VaViT)  
  Keywords: architecture, evaluation  
- **[DTG-Restore: Training-Free Diffusion Refinement for Generative Video Super-Resolution](https://arxiv.org/abs/2605.30431v1)**  
  Authors: Hidir Yesiltepe, Koutilya PNVR, Gaurav Pathak, Navaneeth Bodla, Bharat Singh, Pinar Yanardag, Jinrong Xie  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30431v1.pdf)  
  Keywords: video diffusion, text-to-video, dit, evaluation, super-resolution, diffusion model, benchmark  
- **[YoCausal: How Far is Video Generation from World Model? A Causality Perspective](https://arxiv.org/abs/2605.30346v1)**  
  Authors: You-Zhe Xie, Yu-Hsuan Li, Jie-Ying Lee, Kaipeng Zhang, Yu-Lun Liu, Zhixiang Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30346v1.pdf)  
  Keywords: denoising, video diffusion, world model, evaluation, video generation, diffusion model, benchmark  
- **[VPG: Visual Prefix Guidance for Autoregressive Image and Video Generation](https://arxiv.org/abs/2605.30317v1)**  
  Authors: Xinyao Liao, Qiyuan He, Yicong Li, Jiayin Zhu, Xiaoye Qu, Wei Wei, Angela Yao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30317v1.pdf)  
  Keywords: autoregressive, dit, text-to-video, video generation, benchmark  
- **[LiveSVG: Zero-Shot SVG Animation via Video Generation](https://arxiv.org/abs/2605.30174v1)**  
  Authors: Matan Levy, Ran Margolin, Bar Cavia, Dvir Samuel, Yael Pritch, Shmuel Peleg, Alex Rav Acha, Ariel Shamir, Dani Lischinski  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30174v1.pdf)  
  Keywords: distillation, video diffusion, dit, evaluation, video generation, image-to-video, diffusion model, benchmark  
- **[DirectorBench: Diagnosing Long-Form Video Generation with Personalized Multi-Agent Evaluation](https://arxiv.org/abs/2605.30090v1)**  
  Authors: Jiamin Chen, Qianben Chen, Jiawen Zhang, Yidi Wu, Yuchen Li, Xiaokun Zhang, Wangchunshu Zhou, Chen Ma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30090v1.pdf)  
  Keywords: temporal consistency, evaluation, long-form, video generation, benchmark  
- **[DMC-CF: Dynamic Multimodal CounterFactual QA benchmark for Causal Reasoning](https://arxiv.org/abs/2605.29339v1)**  
  Authors: Junzhe Zhang, Huixuan Zhang, Guirong Wang, Xingyao Zhang, Pei Liu, Lin Qu, Hu Wei, Xiaojun Wan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.29339v1.pdf)  
  Keywords: evaluation, dit, benchmark  
- **[DriveWAM: Video Generative Priors Enable Scalable World-Action Modeling for Autonomous Driving](https://arxiv.org/abs/2605.28544v1)**  
  Authors: Chen Shi, Jinrui Xu, Shaoshuai Shi, Kehua Sheng, Bo Zhang, Li Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28544v1.pdf)  
  Keywords: diffusion transformer, architecture, autoregressive, video diffusion, dynamics, physical, autonomous driving, benchmark  

### Text-to-Video Generation

*Showing the latest 50 out of 51 papers*

- **[TunerDiT: Training-free Progressive Steering of Diffusion Transformer for Multi-Event Video Generation](https://arxiv.org/abs/2605.31590v1)**  
  Authors: Ruotong Liao, Guowen Huang, Qing Cheng, Guangyao Zhai, Lei Zhang, Xun Xiao, Thomas Seidl, Daniel Cremers, Volker Tresp  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.31590v1.pdf)  
  Keywords: t2v, diffusion transformer, video diffusion, text-to-video, dit, layout, video generation, denoising, trajectory, benchmark  
- **[SlotMemory: Object-Centric KV Memory for Streaming Long-Video Generation](https://arxiv.org/abs/2605.31033v1)**  
  Authors: Weijia Dou, Hui Li, Jiahao Cui, Lei Zhou, Jingdong Wang, Siyu Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.31033v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://tj12323.github.io/SlotMemory)  
  Keywords: t2v, identity, video diffusion, streaming, interactive, long-form, video generation, video synthesis  
- **[DTG-Restore: Training-Free Diffusion Refinement for Generative Video Super-Resolution](https://arxiv.org/abs/2605.30431v1)**  
  Authors: Hidir Yesiltepe, Koutilya PNVR, Gaurav Pathak, Navaneeth Bodla, Bharat Singh, Pinar Yanardag, Jinrong Xie  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30431v1.pdf)  
  Keywords: video diffusion, text-to-video, dit, evaluation, super-resolution, diffusion model, benchmark  
- **[Veda: Scalable Video Diffusion via Distilled Sparse Attention](https://arxiv.org/abs/2605.30325v1)**  
  Authors: Shihao Han, Hao Yang, Xinting Hu, Xiaofeng Mei, Yi Jiang, Xiaojuan Qi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30325v1.pdf)  
  Keywords: t2v, long video, diffusion transformer, video diffusion, efficient, acceleration, diffusion model  
- **[VPG: Visual Prefix Guidance for Autoregressive Image and Video Generation](https://arxiv.org/abs/2605.30317v1)**  
  Authors: Xinyao Liao, Qiyuan He, Yicong Li, Jiayin Zhu, Xiaoye Qu, Wei Wei, Angela Yao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30317v1.pdf)  
  Keywords: autoregressive, dit, text-to-video, video generation, benchmark  
- **[minWM: A Full-Stack Open-Source Framework for Real-Time Interactive Video World Models](https://arxiv.org/abs/2605.30263v1)**  
  Authors: Min Zhao, Hongzhou Zhu, Bokai Yan, Zihan Zhou, Yimin Chen, Wenqiang Sun, Kaiwen Zheng, Guande He, Xiao Yang, Chongxuan Li, Fan Bao, Jun Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30263v1.pdf) | [![GitHub](https://img.shields.io/github/stars/shengshu-ai/minWM?style=social)](https://github.com/shengshu-ai/minWM)  
  Keywords: t2v, i2v, camera control, controllable, architecture, autoregressive, video diffusion, world model, distillation, streaming, interactive, dit, style, video generation, diffusion model, trajectory  
- **[KGEdit: Ambiguity-Aware Knowledge Graphs for Training-Free Precise Video Generation and Editing](https://arxiv.org/abs/2605.29509v1)**  
  Authors: Mingshu Cai, Miao Zhang, Chenghe Yang, Yixuan Li, Osamu Yoshie, Yuya Ieiri  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.29509v1.pdf)  
  Keywords: t2v, diffusion transformer, denoising, identity, temporal consistency, text-to-video, dit, video generation, diffusion model, concept  
- **[OSP-Next: Efficient High-Quality Video Generation with Sparse Sequence Parallelism, HiF8 Quantization, and Reinforcement Learning](https://arxiv.org/abs/2605.28691v1)**  
  Authors: Yunyang Ge, Xianyi He, Zezhong Zhang, Bin Lin, Bin Zhu, Xinhua Cheng, Li Yuan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28691v1.pdf)  
  Keywords: diffusion transformer, architecture, text-to-video, dit, efficient, video generation  
- **[Sketch2Motion: Text-driven 2D Sketch to 3D Animation via Diffusion-guided Skeleton Optimization](https://arxiv.org/abs/2605.28394v1)**  
  Authors: Gaurav Rai, Ojaswa Sharma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28394v1.pdf)  
  Keywords: distillation, video diffusion, physical, dit, text-to-video, physics, diffusion model  
- **[Proprio: Latent Self-Scoring and Inference-Time Refinement for Physically Plausible Video Generation](https://arxiv.org/abs/2605.28230v1)**  
  Authors: Mariam Hassan, Kaouther Messaoud, Wuyang Li, Alexandre Alahi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28230v1.pdf)  
  Keywords: dynamics, physical, text-to-video, evaluation, physics, video generation, image-to-video, benchmark  

### Video Editing

- **[DeltaCam: Differential Intrinsic Camera Modeling for Video Generation](https://arxiv.org/abs/2605.25266v1)**  
  Authors: Debabrata Mandal, Zhihan Peng, Yujie Wang, Praneeth Chakravarthula  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25266v1.pdf)  
  Keywords: video-to-video, controllable, dynamics, video style transfer, video diffusion, dit, style, video generation  
- **[Geo-Align: Video Generation Alignment via Metric Geometry Reward](https://arxiv.org/abs/2605.23903v1)**  
  Authors: Zizun Li, Haoyu Guo, Runzhe Teng, Chunhua Shen, Tong He  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.23903v1.pdf)  
  Keywords: video-to-video, camera control, physical, dit, video generation  
- **[SimInsert: Seamless Video Object Insertion via Regional Sparse Attention Fusion](https://arxiv.org/abs/2605.23245v1)**  
  Authors: Xinyu Chen, Yuyi Qian, Jiang Lin, Shenyi Wang, Gao Wang, Zhiqiu Zhang, Jizhi Zhang, Mingjie Wang, Qiang Tang, Qian Wang, Song Wu, Zili Yi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.23245v1.pdf)  
  Keywords: denoising, video diffusion, video editing, interactive, dit, efficient, image-to-video, diffusion model, trajectory  
- **[StreamGVE: Training-Free Video Editing via Few-Step Streaming Video Generation](https://arxiv.org/abs/2605.21466v1)**  
  Authors: Guanlong Jiao, Chenyangguang Zhang, Jia Jun Cheng Xian, Zewei Zhang, Renjie Liao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.21466v1.pdf)  
  Keywords: video generation, streaming, dit, video editing  
- **[Preserve, Reveal, Expand: Faithful 4D Video Editing with Region-Aware Conditioning](https://arxiv.org/abs/2605.20961v1)**  
  Authors: Zhangchi Hu, Wenzhang Sun, Xiangchen Yin, Jiahui Yuan, Chunfeng Wang, Hao Li, Kun Zhan, Xiaoyan Sun  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20961v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://ricepastem.github.io/PREX-Open)  
  Keywords: video diffusion, video editing, dit, evaluation, diffusion model, benchmark  
- **[What Semantics Survive the Connector? Diagnosing VLM-to-DiT Alignment in Video Editing](https://arxiv.org/abs/2605.20795v1)**  
  Authors: Hangyu Lin, Chao Wen, Chengming Xu, Jianxiong Gao, Jiangning Zhang, Xiaobin Hu, Yanwei Fu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20795v1.pdf)  
  Keywords: architecture, flow matching, video editing, dit, evaluation, multi-modal  
- **[Goodbye Drift: Anchored Tree Sampling for Long-Horizon Video-to-Video Generation](https://arxiv.org/abs/2605.20476v1)**  
  Authors: Matthew Bendel, Stephen W. Bailey, Mithilesh Vaidya, Sumukh Badam, Xingzhe He  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20476v1.pdf)  
  Keywords: t2v, video-to-video, distillation, outpainting, autoregressive, dit, style, video generation  
- **[PhyWorld: Physics-Faithful World Model for Video Generation](https://arxiv.org/abs/2605.19242v1)**  
  Authors: Pu Zhao, Juyi Lin, Timothy Rupprecht, Arash Akbari, Chence Yang, Rahul Chowdhury, Elaheh Motamedi, Arman Akbari, Yumei He, Chen Wang, Geng Yuan, Weiwei Chen, Yanzhi Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.19242v1.pdf)  
  Keywords: video-to-video, world simulator, dynamics, world model, flow matching, physical, dit, physics, video generation, benchmark  
- **[Aurora: Unified Video Editing with a Tool-Using Agent](https://arxiv.org/abs/2605.18748v1)**  
  Authors: Yongsheng Yu, Ziyun Zeng, Zhiyuan Xiao, Zhenghong Zhou, Hang Hua, Wei Xiong, Jiebo Luo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.18748v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://yeates.github.io/Aurora-Page)  
  Keywords: diffusion transformer, video diffusion, video editing, dit, style, benchmark  
- **[InstructAV2AV: Instruction-Guided Audio-Video Joint Editing](https://arxiv.org/abs/2605.18467v1)**  
  Authors: Haojie Zheng, Yixin Yang, Siqi Yang, Shuchen Weng, Boxin Shi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.18467v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://hjzheng.net/projects/InstructAV2AV)  
  Keywords: controllable, video editing, dit, evaluation, video generation  

### Video Inpainting & Completion

- **[Full-4D: Generating Full-Scope 4D Scenes from a Single-View Video](https://arxiv.org/abs/2605.25500v1)**  
  Authors: Tingxi Chen, Ke Hao, Yabo Chen, Zhengxue Cheng, Rong Xie, Li Song, Haibin Huang, Chi Zhang, Xuelong Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25500v1.pdf)  
  Keywords: distillation, multi-view video, video diffusion, video interpolation, flow matching, physical, interactive, dit, 4d generation, diffusion model, video synthesis  
- **[CRONOS: Benchmarking Counterfactual Physical Consistency in Video Models](https://arxiv.org/abs/2605.23699v1)**  
  Authors: León Begiristain, Olaf Dünkel, Adam Kortylewski  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.23699v1.pdf)  
  Keywords: dynamics, world model, physical, dit, evaluation, video prediction, benchmark  
- **[GEM-4D: Geometry-Enhanced Video World Models for Robot Manipulation](https://arxiv.org/abs/2605.22882v2)**  
  Authors: Kaichen Zhou, Yuzhen Chen, Fangneng Zhan, Hang Hua, Grace Chen, Xinhai Chang, Ao Qu, Yilun Du, Zhuang Liu, Paul Pu Liang, Mengyu Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.22882v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://gem-4d.github.io)  
  Keywords: architecture, dynamics, world model, physical, dit, simulation, video prediction  
- **[Goodbye Drift: Anchored Tree Sampling for Long-Horizon Video-to-Video Generation](https://arxiv.org/abs/2605.20476v1)**  
  Authors: Matthew Bendel, Stephen W. Bailey, Mithilesh Vaidya, Sumukh Badam, Xingzhe He  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20476v1.pdf)  
  Keywords: t2v, video-to-video, distillation, outpainting, autoregressive, dit, style, video generation  
- **[Nano World Models: A Minimalist Implementation of Future Video Prediction](https://arxiv.org/abs/2605.23993v2)**  
  Authors: Siqiao Huang, Partha Kaushik, Michael Chen, Hengkai Pan, Kaiwen Geng, Omar Chehab, Fernando Moreno-Pino, Max Simchowitz  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.23993v2.pdf)  
  Keywords: architecture, autoregressive, world model, interactive, dit, evaluation, simulation, video prediction, video generation  
- **[Relit-LiVE: Relight Video by Jointly Learning Environment Video](https://arxiv.org/abs/2605.06658v1)**  
  Authors: Weiqing Xiao, Hong Li, Xiuyu Yang, Houyuan Chen, Wenyi Li, Tianqi Liu, Shaocong Xu, Chongjie Ye, Hao Zhao, Beibei Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.06658v1.pdf) | [![GitHub](https://img.shields.io/github/stars/zhuxing0/Relit-LiVE?style=social)](https://github.com/zhuxing0/Relit-LiVE)  
  Keywords: video diffusion, physical, streaming, dit, video prediction, diffusion model, benchmark  
- **[Quaternion Nonlinear Transform-Induced Nuclear Norm for Low-Rank Tensor Completion](https://arxiv.org/abs/2605.01467v1)**  
  Authors: Biswarup Karmakar, Ratikanta Behera  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.01467v1.pdf)  
  Keywords: efficient, video inpainting, benchmark  
- **[LMGenDrive: Bridging Multimodal Understanding and Generative World Modeling for End-to-End Driving](https://arxiv.org/abs/2604.08719v1)**  
  Authors: Hao Shao, Letian Wang, Yang Zhou, Yuxuan Hu, Zhuofan Zong, Steven L. Waslander, Wei Zhan, Hongsheng Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2604.08719v1.pdf)  
  Keywords: autoregressive, world model, autonomous driving, video prediction, video generation, benchmark  
- **[Novel View Synthesis as Video Completion](https://arxiv.org/abs/2604.08500v1)**  
  Authors: Qi Wu, Khiem Vuong, Minsik Jeon, Srinivasa Narasimhan, Deva Ramanan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2604.08500v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://frame-crafter.github.io)  
  Keywords: video diffusion, novel view, diffusion model, video completion, benchmark  
- **[SEM-ROVER: Semantic Voxel-Guided Diffusion for Large-Scale Driving Scene Generation](https://arxiv.org/abs/2604.06113v1)**  
  Authors: Hiba Dahmani, Nathan Piasco, Moussab Bennehar, Luis Roldão, Dzmitry Tsishkou, Laurent Caraffa, Jean-Philippe Tarel, Roland Brémond  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2604.06113v1.pdf)  
  Keywords: outpainting, diffusion model, dit  

### Video Super-Resolution & Enhancement

*Showing the latest 50 out of 69 papers*

- **[TunerDiT: Training-free Progressive Steering of Diffusion Transformer for Multi-Event Video Generation](https://arxiv.org/abs/2605.31590v1)**  
  Authors: Ruotong Liao, Guowen Huang, Qing Cheng, Guangyao Zhai, Lei Zhang, Xun Xiao, Thomas Seidl, Daniel Cremers, Volker Tresp  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.31590v1.pdf)  
  Keywords: t2v, diffusion transformer, video diffusion, text-to-video, dit, layout, video generation, denoising, trajectory, benchmark  
- **[Robust Dreamer: Deviation-Aware Latent Gaussian Memory for Action-Controlled AR Video Generation](https://arxiv.org/abs/2605.30855v1)**  
  Authors: Hanlin Chen, Jiaxin Wei, Xibin Song, Yifu Wang, Steve Wang, Hongdong Li, Pan Ji, Gim Hee Lee  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30855v1.pdf)  
  Keywords: autoregressive, interactive, dit, 3d-aware, simulation, video generation, image-to-video, denoising  
- **[DTG-Restore: Training-Free Diffusion Refinement for Generative Video Super-Resolution](https://arxiv.org/abs/2605.30431v1)**  
  Authors: Hidir Yesiltepe, Koutilya PNVR, Gaurav Pathak, Navaneeth Bodla, Bharat Singh, Pinar Yanardag, Jinrong Xie  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30431v1.pdf)  
  Keywords: video diffusion, text-to-video, dit, evaluation, super-resolution, diffusion model, benchmark  
- **[AdaState: Self-Evolving Anchors for Streaming Video Generation](https://arxiv.org/abs/2605.30349v1)**  
  Authors: Yusuf Dalva, Pinar Yanardag  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30349v1.pdf)  
  Keywords: denoising, autoregressive, video diffusion, dynamics, streaming, dit, video generation, diffusion model  
- **[YoCausal: How Far is Video Generation from World Model? A Causality Perspective](https://arxiv.org/abs/2605.30346v1)**  
  Authors: You-Zhe Xie, Yu-Hsuan Li, Jie-Ying Lee, Kaipeng Zhang, Yu-Lun Liu, Zhixiang Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30346v1.pdf)  
  Keywords: denoising, video diffusion, world model, evaluation, video generation, diffusion model, benchmark  
- **[Native Audio-Visual Alignment for Generation](https://arxiv.org/abs/2605.30073v1)**  
  Authors: Longbin Ji, Guan Wang, Xuan Wei, Chenye Yang, Xiangrui Liu, Zhenyu Zhang, Shuohuan Wang, Yu Sun, Jingzhou He  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30073v1.pdf)  
  Keywords: controllable, architecture, dit, video generation, denoising  
- **[KGEdit: Ambiguity-Aware Knowledge Graphs for Training-Free Precise Video Generation and Editing](https://arxiv.org/abs/2605.29509v1)**  
  Authors: Mingshu Cai, Miao Zhang, Chenghe Yang, Yixuan Li, Osamu Yoshie, Yuya Ieiri  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.29509v1.pdf)  
  Keywords: t2v, diffusion transformer, denoising, identity, temporal consistency, text-to-video, dit, video generation, diffusion model, concept  
- **[PARE: Pruning and Adaptive Routing for Efficient Video Generation](https://arxiv.org/abs/2605.27336v1)**  
  Authors: Yutong Wang, Yunke Wang, Tianfan Xue, Yu Qiao, Yaohui Wang, Xinyuan Chen, Chang Xu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.27336v1.pdf)  
  Keywords: diffusion transformer, distillation, acceleration, architecture, video diffusion, text-to-video, dit, efficient, video generation, image-to-video, denoising  
- **[Timestep-Aware SVDQuant-GPTQ for W4A4 Quantization of Wan2.2-I2V](https://arxiv.org/abs/2605.27003v1)**  
  Authors: Junhao Wu, Dezhong Yao, Hai Jin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.27003v1.pdf)  
  Keywords: diffusion transformer, i2v, video diffusion, dit, denoising, trajectory, benchmark  
- **[On-Policy Adversarial Flow Distillation for Autoregressive Video Generation](https://arxiv.org/abs/2605.26105v1)**  
  Authors: Yang Luo, Shengju Qian, Xiaohang Tang, Zirui Zhu, Yong Liu, Xin Wang, Yang You  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.26105v1.pdf)  
  Keywords: distillation, architecture, autoregressive, streaming, interactive, dit, physics, efficient, video generation, denoising  

### World Models & Simulation

*Showing the latest 50 out of 121 papers*

- **[DecMem: Towards Minute-Long Consistent World Generation with Decoupled Memory](https://arxiv.org/abs/2605.31336v1)**  
  Authors: Zhenhao Yang, Xiaoshi Wu, Zhengyao Lv, Xiaoyu Shi, Xintao Wang, Pengfei Wan, Kun Gai, Kwan-Yee K. Wong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.31336v1.pdf)  
  Keywords: long video, controllable, architecture, world model, temporal consistency, efficient, video generation  
- **[SlotMemory: Object-Centric KV Memory for Streaming Long-Video Generation](https://arxiv.org/abs/2605.31033v1)**  
  Authors: Weijia Dou, Hui Li, Jiahao Cui, Lei Zhou, Jingdong Wang, Siyu Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.31033v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://tj12323.github.io/SlotMemory)  
  Keywords: t2v, identity, video diffusion, streaming, interactive, long-form, video generation, video synthesis  
- **[Robust Dreamer: Deviation-Aware Latent Gaussian Memory for Action-Controlled AR Video Generation](https://arxiv.org/abs/2605.30855v1)**  
  Authors: Hanlin Chen, Jiaxin Wei, Xibin Song, Yifu Wang, Steve Wang, Hongdong Li, Pan Ji, Gim Hee Lee  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30855v1.pdf)  
  Keywords: autoregressive, interactive, dit, 3d-aware, simulation, video generation, image-to-video, denoising  
- **[YoCausal: How Far is Video Generation from World Model? A Causality Perspective](https://arxiv.org/abs/2605.30346v1)**  
  Authors: You-Zhe Xie, Yu-Hsuan Li, Jie-Ying Lee, Kaipeng Zhang, Yu-Lun Liu, Zhixiang Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30346v1.pdf)  
  Keywords: denoising, video diffusion, world model, evaluation, video generation, diffusion model, benchmark  
- **[minWM: A Full-Stack Open-Source Framework for Real-Time Interactive Video World Models](https://arxiv.org/abs/2605.30263v1)**  
  Authors: Min Zhao, Hongzhou Zhu, Bokai Yan, Zihan Zhou, Yimin Chen, Wenqiang Sun, Kaiwen Zheng, Guande He, Xiao Yang, Chongxuan Li, Fan Bao, Jun Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30263v1.pdf) | [![GitHub](https://img.shields.io/github/stars/shengshu-ai/minWM?style=social)](https://github.com/shengshu-ai/minWM)  
  Keywords: t2v, i2v, camera control, controllable, architecture, autoregressive, video diffusion, world model, distillation, streaming, interactive, dit, style, video generation, diffusion model, trajectory  
- **[Gamma-World: Generative Multi-Agent World Modeling Beyond Two Players](https://arxiv.org/abs/2605.28816v1)**  
  Authors: Fangfu Liu, Kai He, Tianchang Shen, Tianshi Cao, Sanja Fidler, Yueqi Duan, Jun Gao, Igor Gilitschenski, Zian Wang, Xuanchi Ren  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28816v1.pdf)  
  Keywords: controllable, identity, world model, interactive, dit, efficient, simulation, video generation  
- **[Turning Video Models into Generalist Robot Policies](https://arxiv.org/abs/2605.27817v1)**  
  Authors: Sizhe Lester Li, Evan Kim, Xingjian Bai, Tong Zhao, Tao Pang, Max Simchowitz, Vincent Sitzmann  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.27817v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://vera.csail.mit.edu)  
  Keywords: dynamics, world model, efficient, robotics, benchmark  
- **[What-If World: A Causal Benchmark for General World Models in Embodied Scenarios](https://arxiv.org/abs/2605.27589v1)**  
  Authors: Kunlin Cai, Rui Song, Jinghuai Zhang, Kaiyuan Zhang, Pranav Bodapati, Alicia Yu, Fnu Suya, Mohammad Rostami, Jiaqi Ma, Yuan Tian  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.27589v1.pdf)  
  Keywords: world simulator, world model, physical, action-conditioned, dit, physics, simulation, video generation, benchmark  
- **[AnyScene: Towards Highly Controllable Driving Scene Generation at Anywhere and Beyond](https://arxiv.org/abs/2605.26113v1)**  
  Authors: Haiming Zhang, Junfei Zhou, Feng Jiang, Jingzhong Li, Zhenglong Guo, Penglin Dai, Jifeng Dai, Yan Xie, Benjin Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.26113v1.pdf)  
  Keywords: diffusion transformer, controllable, autoregressive, dit, autonomous driving, simulation, layout, video generation, video synthesis  
- **[On-Policy Adversarial Flow Distillation for Autoregressive Video Generation](https://arxiv.org/abs/2605.26105v1)**  
  Authors: Yang Luo, Shengju Qian, Xiaohang Tang, Zirui Zhu, Yong Liu, Xin Wang, Yang You  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.26105v1.pdf)  
  Keywords: distillation, architecture, autoregressive, streaming, interactive, dit, physics, efficient, video generation, denoising  



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
