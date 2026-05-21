# Awesome Video Diffusions [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of latest research papers, projects and resources related to Video Diffusion Models and Video Generation. Content is automatically updated daily.

> Last Update: 2026-05-21 03:43:11

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

- [3D-aware Video Generation](#3d-aware-video-generation) (20 papers) - Video generation with 3D awareness, multi-view consistency, and 4D content creation
- [Applications](#applications) (55 papers) - Domain-specific applications of video diffusion models
- [Architecture & Efficiency](#architecture-&-efficiency) (359 papers) - Architectural innovations (DiT, UNet), flow matching, and training/inference efficiency
- [Audio & Multi-modal](#audio-&-multi-modal) (33 papers) - Audio-driven and multi-modal conditioned video generation
- [Controllable Generation](#controllable-generation) (130 papers) - Controllable video generation with motion, camera, pose, or layout guidance
- [Human & Character Animation](#human-&-character-animation) (25 papers) - Human-centric video generation including talking heads, dance, and character animation
- [Image-to-Video Generation](#image-to-video-generation) (39 papers) - Methods for animating still images into videos
- [Long Video Generation](#long-video-generation) (125 papers) - Generating temporally consistent long-form videos beyond short clips
- [Personalization & Customization](#personalization-&-customization) (83 papers) - Personalized video generation with custom subjects, identities, or styles
- [Physical Understanding](#physical-understanding) (150 papers) - Physics-aware video generation and dynamics modeling
- [Surveys & Benchmarks](#surveys-&-benchmarks) (228 papers) - Survey papers, benchmarks, and evaluation metrics for video generation
- [Text-to-Video Generation](#text-to-video-generation) (43 papers) - Foundation models and methods for generating videos from text prompts
- [Video Editing](#video-editing) (33 papers) - Diffusion-based video editing, style transfer, and manipulation
- [Video Inpainting & Completion](#video-inpainting-&-completion) (7 papers) - Video inpainting, completion, outpainting, and temporal prediction
- [Video Super-Resolution & Enhancement](#video-super-resolution-&-enhancement) (72 papers) - Video quality improvement, upscaling, restoration, and frame interpolation
- [World Models & Simulation](#world-models-&-simulation) (118 papers) - Video generation as world simulators and interactive environment generation



## Table of Contents

- [Categorized Papers](#categorized-papers)
- [Classic Papers](#classic-papers)
- [Open Source Projects](#open-source-projects)
- [Applications](#applications)
- [Tutorials & Blogs](#tutorials--blogs)





## Categorized Papers

### 3D-aware Video Generation

- **[3DPhysVideo: Consistency-Guided Flow SDE for Video Generation via 3D Scene Reconstruction and Physical Simulation](https://arxiv.org/abs/2605.16795v1)**  
  Authors: Hwidong Kim, Yunho Kim, Tae-Kyun Kim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.16795v1.pdf)  
  Keywords: dynamics, denoising, simulation, efficient, video generation, physical, evaluation, physical simulation, novel view, benchmark, physics, image-to-video, i2v, dit  
- **[GTA: Advancing Image-to-3D World Generation via Geometry Then Appearance Video Diffusion](https://arxiv.org/abs/2605.12957v1)**  
  Authors: Hanxin Zhu, Cong Wang, Peiyan Tu, Jiayi Luo, Tianyu He, Xin Jin, Zhibo Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.12957v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://hanxinzhu-lab.github.io/GTA)  
  Keywords: video diffusion, diffusion model, novel view, autonomous driving, dit  
- **[GaitProtector: Impersonation-Driven Gait De-Identification via Training-Free Diffusion Latent Optimization](https://arxiv.org/abs/2605.12431v1)**  
  Authors: Huiran Duan, Qian Zhou, Zhongliang Guo, Junhao Dong, Yuqi Li, Guoying Zhao, Yingli Tian  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.12431v1.pdf)  
  Keywords: dynamics, identity, video diffusion, trajectory, diffusion model, 3d video  
- **[VidSplat: Gaussian Splatting Reconstruction with Geometry-Guided Video Diffusion Priors](https://arxiv.org/abs/2605.11424v1)**  
  Authors: Jimin Tang, Wenyuan Zhang, Junsheng Zhou, Zian Huang, Kanle Shi, Shenkun Xu, Yu-Shen Liu, Zhizhong Han  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.11424v1.pdf)  
  Keywords: video diffusion, denoising, novel view, benchmark, 3d consistent  
- **[LoViF 2026 The First Challenge on Holistic Quality Assessment for 4D World Model (PhyScore)](https://arxiv.org/abs/2605.05187v1)**  
  Authors: Wei Luo, Yiting Lu, Xin Li, Haoran Li, Fengbin Guan, Chen Gao, Xin Jin, Yong Li, Zhibo Chen, Sijing Wu, Kang Fu, Yunhao Li, Ziang Xiao, Huiyu Duan, Jing Liu, Qiang Hu, Xiongkuo Min, Guangtao Zhai, Manxi Sun, Zixuan Guo, Yun Li, Ziyang Chen, Manabu Tsukada, Zhengyang Li, Zhenglin Du, Yi Wen, Licheng Jiao, Fang Liu, Lingling Li, Yiwen Ren, Zhilong Song, Dubing Chen, Yucheng Zhou, Tianyi Yan, Huan Zheng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.05187v1.pdf)  
  Keywords: dynamics, world model, physical, evaluation, benchmark, creative, 4d generation, physics, temporal consistency, dit  
- **[AnyRecon: Arbitrary-View 3D Reconstruction with Video Diffusion Model](https://arxiv.org/abs/2604.19747v1)**  
  Authors: Yutian Chen, Shi Guo, Renbiao Jin, Tianshuo Yang, Xin Cai, Yawen Luo, Mingxin Yang, Mulin Yu, Linning Xu, Tianfan Xue  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2604.19747v1.pdf)  
  Keywords: video diffusion, diffusion model, novel view, distillation, dit  
- **[MultiWorld: Scalable Multi-Agent Multi-View Video World Models](https://arxiv.org/abs/2604.18564v2)**  
  Authors: Haoyu Wu, Jiwen Yu, Yingtian Zou, Xihui Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2604.18564v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://multi-world.github.io)  
  Keywords: dynamics, world model, video generation, multi-view video, action-conditioned, dit  
- **[ArtifactWorld: Scaling 3D Gaussian Splatting Artifact Restoration via Video Generation Models](https://arxiv.org/abs/2604.12251v1)**  
  Authors: Xinliang Wang, Yifeng Shi, Zhenyu Wu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2604.12251v1.pdf)  
  Keywords: video diffusion, novel view, video generation  
- **[Rays as Pixels: Learning A Joint Distribution of Videos and Camera Trajectories](https://arxiv.org/abs/2604.09429v3)**  
  Authors: Wonbong Jang, Shikun Liu, Soubhik Sanyal, Juan Camilo Perez, Kam Woh Ng, Sanskar Agrawal, Juan-Manuel Perez-Rua, Yiannis Douratsos, Tao Xiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2604.09429v3.pdf)  
  Keywords: video diffusion, video generation, trajectory, diffusion model, novel view, dit  
- **[Novel View Synthesis as Video Completion](https://arxiv.org/abs/2604.08500v1)**  
  Authors: Qi Wu, Khiem Vuong, Minsik Jeon, Srinivasa Narasimhan, Deva Ramanan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2604.08500v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://frame-crafter.github.io)  
  Keywords: video diffusion, diffusion model, benchmark, novel view, video completion  

### Applications

*Showing the latest 50 out of 55 papers*

- **[CogOmniControl: Reasoning-Driven Controllable Video Generation via Creative Intent Cognition](https://arxiv.org/abs/2605.19995v1)**  
  Authors: Hongji Yang, Songlian Li, Yucheng Zhou, Xiaotong Zhao, Alan Zhao, Chengzhong Xu, Jianbing Shen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.19995v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://um-lab.github.io/CogOmniControl)  
  Keywords: video generation, architecture, diffusion model, benchmark, creative, dit, controllable  
- **[CodeBind: Decoupled Representation Learning for Multimodal Alignment with Unified Compositional Codebook](https://arxiv.org/abs/2605.18257v1)**  
  Authors: Zeyu Chen, Jie Li, Kai Han  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.18257v1.pdf)  
  Keywords: robotics, dit  
- **[Xiaomi EV World Model: A Joint World Model Integrating Reconstruction and Generation for Autonomous Driving](https://arxiv.org/abs/2605.18137v2)**  
  Authors: Lijun Zhou, Hongcheng Luo, Zhenxin Zhu, Cheng Chi, Mingfei Tu, Kaixin Xiong, Lei Gong, Zhanqian Wu, Zehan Zhang, Fangzhen Li, Hao Li, Yingying Shen, Jiale He, Haohui Zhu, Shan Zhao, Kai Wang, Zhiwei Zhan, Yuechuan Pu, Kaiyuan Tan, Ruiling Yang, Xianqi Wang, Tianyi Yan, Jiawei Zhou, Lei Zhang, Jingyang Zhao, Xi Zhou, Chitian Sun, Chenming Wu, Jiong Deng, Hongwei Xie, Ming Lu, Kun Ma, Long Chen, Guang Chen, Hangjun Ye, Bing Wang, Haiyang Sun  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.18137v2.pdf)  
  Keywords: denoising, simulation, world model, architecture, video generation, distillation, autonomous driving  
- **[Soap2Soap: Long Cinematic Video Remaking via Multi-Agent Collaboration](https://arxiv.org/abs/2605.17423v1)**  
  Authors: Yiren Song, Huilin Zhong, Kevin Qinghong Lin, Haofan Wang, Mike Zheng Shou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.17423v1.pdf)  
  Keywords: identity, video generation, video synthesis, film, video-to-video, dit  
- **[DriveCtrl: Conditioned Sim-to-Real Driving Video Generation](https://arxiv.org/abs/2605.15116v1)**  
  Authors: Haonan Zhao, Yiting Wang, Jingkun Chen, Valentina Donzella, Thomas Bashford-Rogers, Kurt Debattista  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.15116v1.pdf)  
  Keywords: dynamics, simulation, style, autonomous driving, video generation, video synthesis, evaluation, layout, temporal consistency, depth-guided, dit, controllable  
- **[Generating HDR Video from SDR Video](https://arxiv.org/abs/2605.14703v1)**  
  Authors: SaiKiran Tedla, Francesco Banterle, Trevor Canham, Karanpreet Raja, David B. Lindell, Kiriakos N. Kutulakos, Jiacheng Li, Feiran Li, Daisuke Iso  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.14703v1.pdf)  
  Keywords: film, video synthesis, evaluation  
- **[GTA: Advancing Image-to-3D World Generation via Geometry Then Appearance Video Diffusion](https://arxiv.org/abs/2605.12957v1)**  
  Authors: Hanxin Zhu, Cong Wang, Peiyan Tu, Jiayi Luo, Tianyu He, Xin Jin, Zhibo Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.12957v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://hanxinzhu-lab.github.io/GTA)  
  Keywords: video diffusion, diffusion model, novel view, autonomous driving, dit  
- **[Images in Sentences: Scaling Interleaved Instructions for Unified Visual Generation](https://arxiv.org/abs/2605.12305v1)**  
  Authors: Yabo Zhang, Kunchang Li, Dewei Zhou, Xinyu Huang, Xun Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.12305v1.pdf)  
  Keywords: evaluation, creative, dit  
- **[TIE: Time Interval Encoding for Video Generation over Events](https://arxiv.org/abs/2605.10543v1)**  
  Authors: Zhilei Shu, Shangwen Zhu, Zihang Liang, Xiaofan Li, Qianyu Peng, Xinyu Cui, Bo Ye, Yiming Li, Fan Cheng, Jian Zhao, Yang Cao, Zheng-Jun Zha, Ruili Feng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.10543v1.pdf) | [![GitHub](https://img.shields.io/github/stars/MatrixTeam-AI/TIE?style=social)](https://github.com/MatrixTeam-AI/TIE)  
  Keywords: efficient, interactive, style, video generation, trajectory, robotics, dit, diffusion transformer  
- **[SocialDirector: Training-Free Social Interaction Control for Multi-Person Video Generation](https://arxiv.org/abs/2605.10079v1)**  
  Authors: Liangyang Ouyang, Ruicong Liu, Caixin Kang, Yifei Huang, Yoichi Sato  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.10079v1.pdf)  
  Keywords: dynamics, video generation, evaluation, robotics, film, gesture  

### Architecture & Efficiency

*Showing the latest 50 out of 359 papers*

- **[StreamGVE: Training-Free Video Editing via Few-Step Streaming Video Generation](https://arxiv.org/abs/2605.21466v1)**  
  Authors: Guanlong Jiao, Chenyangguang Zhang, Jia Jun Cheng Xian, Zewei Zhang, Renjie Liao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.21466v1.pdf)  
  Keywords: streaming, video editing, dit, video generation  
- **[iTryOn: Mastering Interactive Video Virtual Try-On with Spatial-Semantic Guidance](https://arxiv.org/abs/2605.21431v1)**  
  Authors: Jun Zheng, Zhengze Xu, Mengting Chen, Jing Wang, Jinsong Lan, Xiaoyong Zhu, Kaifu Zhang, Bo Zheng, Xiaodan Liang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.21431v1.pdf)  
  Keywords: dynamics, video diffusion, interactive, diffusion transformer, benchmark, virtual try-on, temporal consistency, dit, controllable  
- **[Q-ARVD: Quantizing Autoregressive Video Diffusion Models](https://arxiv.org/abs/2605.21072v1)**  
  Authors: Siao Tang, Xinyin Ma, Gongfan Fang, Xingyi Yang, Xinchao Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.21072v1.pdf)  
  Keywords: autoregressive, video diffusion, interactive, video generation, world model, architecture, diffusion model, streaming, diffusion transformer  
- **[Dynamic Video Generation: Shaping Video Generation Across Time and Space](https://arxiv.org/abs/2605.21042v1)**  
  Authors: Shikang Zheng, Jingkai Huang, Jiacheng Liu, Guantao Chen, Lixuan, Yuqi Lin, Peiliang Cai, Linfeng Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.21042v1.pdf)  
  Keywords: efficient, acceleration, denoising, video generation, diffusion model, distillation, dit  
- **[Preserve, Reveal, Expand: Faithful 4D Video Editing with Region-Aware Conditioning](https://arxiv.org/abs/2605.20961v1)**  
  Authors: Zhangchi Hu, Wenzhang Sun, Xiangchen Yin, Jiahui Yuan, Chunfeng Wang, Hao Li, Kun Zhan, Xiaoyan Sun  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20961v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://ricepastem.github.io/PREX-Open)  
  Keywords: video diffusion, evaluation, diffusion model, benchmark, video editing, dit  
- **[FlowLong: Inference-time Long Video Generation via Manifold-constrained Tweedie Matching](https://arxiv.org/abs/2605.20910v1)**  
  Authors: Jangho Park, Geon Yeong Park, Gihyun Kwon, Jong Chul Ye  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20910v1.pdf)  
  Keywords: long video, video diffusion, autoregressive, video generation, architecture, diffusion model, temporal consistency, dit  
- **[What Semantics Survive the Connector? Diagnosing VLM-to-DiT Alignment in Video Editing](https://arxiv.org/abs/2605.20795v1)**  
  Authors: Hangyu Lin, Chao Wen, Chengming Xu, Jianxiong Gao, Jiangning Zhang, Xiaobin Hu, Yanwei Fu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20795v1.pdf)  
  Keywords: architecture, evaluation, multi-modal, video editing, flow matching, dit  
- **[RoPeSLR: 3D RoPE-driven Sparse-LowRank Attention for Efficient Diffusion Transformers](https://arxiv.org/abs/2605.20659v1)**  
  Authors: Yuxi Liu, Zekun Zhang, Yixiang Cai, Renjia Deng, Yutong He, Kun Yuan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20659v1.pdf)  
  Keywords: long video, efficient, video generation, evaluation, dit, diffusion transformer  
- **[Goodbye Drift: Anchored Tree Sampling for Long-Horizon Video-to-Video Generation](https://arxiv.org/abs/2605.20476v1)**  
  Authors: Matthew Bendel, Stephen W. Bailey, Mithilesh Vaidya, Sumukh Badam, Xingzhe He  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20476v1.pdf)  
  Keywords: autoregressive, style, video generation, outpainting, t2v, distillation, video-to-video, dit  
- **[Tiny-Engram: Trigger-Indexed Concept Tables for Generative Vision](https://arxiv.org/abs/2605.20309v1)**  
  Authors: Runyuan Cai, Yiming Wang, Yu Lin, Xiaodong Zeng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20309v1.pdf)  
  Keywords: identity, video diffusion, video generation, concept, personalization, dit  

### Audio & Multi-modal

- **[What Semantics Survive the Connector? Diagnosing VLM-to-DiT Alignment in Video Editing](https://arxiv.org/abs/2605.20795v1)**  
  Authors: Hangyu Lin, Chao Wen, Chengming Xu, Jianxiong Gao, Jiangning Zhang, Xiaobin Hu, Yanwei Fu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20795v1.pdf)  
  Keywords: architecture, evaluation, multi-modal, video editing, flow matching, dit  
- **[Sound Sparks Motion: Audio and Text Tuning for Video Editing](https://arxiv.org/abs/2605.15307v1)**  
  Authors: AmirHossein Naghi Razlighi, Aryan Mikaeili, Ali Mahdavi-Amiri, Daniel Cohen-Or, Yiorgos Chrysanthou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.15307v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://amirhossein-razlighi.github.io/Sound_Sparks_Motion)  
  Keywords: motion control, video generation, sound, video editing, dit  
- **[OmniNFT: Modality-wise Omni Diffusion Reinforcement for Joint Audio-Video Generation](https://arxiv.org/abs/2605.12480v1)**  
  Authors: Guohui Zhang, XiaoXiao Ma, Jie Huang, Hang Xu, Hu Yu, Siming Fu, Yuming Li, Zeyue Xue, Lin Song, Haoyang Huang, Nan Duan, Feng Zhao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.12480v1.pdf)  
  Keywords: multi-modal, efficient, dit, video generation  
- **[AllocMV: Optimal Resource Allocation for Music Video Generation via Structured Persistent State](https://arxiv.org/abs/2605.10723v1)**  
  Authors: Huimin Wang, Leilei Ouyang, Chang Xia, Yongqi Kang, Yu Fu, Yuqi Ouyang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.10723v1.pdf)  
  Keywords: video synthesis, dit, music video, video generation  
- **[Omni-DeepSearch: A Benchmark for Audio-Driven Omni-Modal Deep Search](https://arxiv.org/abs/2605.08762v1)**  
  Authors: Tao Yu, yiming ding, Shenghua Chai, Minghui Zhang, Zhongtian Luo, Xinming Wang, Xinlong Chen, Zhaolu Kang, Junhao Gong, Yuxuan Zhou, Haopeng Jin, Zhiqing Cui, Jiabing Yang, YiFan Zhang, Hongzhu Yi, Zheqi He, Xi Yang, Yan Huang, Liang Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.08762v1.pdf)  
  Keywords: audio-driven, benchmark  
- **[Unison: Harmonizing Motion, Speech, and Sound for Human-Centric Audio-Video Generation](https://arxiv.org/abs/2605.08729v1)**  
  Authors: Shihao Cheng, Jiaxu Zhang, Quanyue Song, Shansong Liu, Zhizhi Guo, Xiaolei Zhang, Chi Zhang, Xuelong Li, Zhigang Tu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.08729v1.pdf)  
  Keywords: sound, denoising, dit, video generation  
- **[Do Joint Audio-Video Generation Models Understand Physics?](https://arxiv.org/abs/2605.07061v1)**  
  Authors: Zijun Cui, Xiulong Liu, Hao Fang, Mingwei Xu, Jiageng Liu, Zexin Xu, Weiguo Pian, Shijian Deng, Feiyu Du, Chenming Ge, Yapeng Tian  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.07061v1.pdf)  
  Keywords: dynamics, style, video generation, physical, sound, benchmark, physics  
- **[Audio-Visual Intelligence in Large Foundation Models](https://arxiv.org/abs/2605.04045v1)**  
  Authors: You Qin, Kai Liu, Shengqiong Wu, Kai Wang, Shijian Deng, Yapeng Tian, Junbin Xiao, Yazhou Xing, Yinghao Ma, Bobo Li, Roger Zimmermann, Lei Cui, Furu Wei, Jiebo Luo, Hao Fei  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.04045v1.pdf)  
  Keywords: autoregressive, architecture, video synthesis, evaluation, sound, benchmark, survey, audio-driven, dit, controllable  
- **[Divide and Conquer: Decoupled Representation Alignment for Multimodal World Models](https://arxiv.org/abs/2605.01896v1)**  
  Authors: Junyuan Xiao, Dingkang Liang, Xin Zhou, Yixuan Ye, Tongtong Su, Guangmo Yi, Bin Xia, Qiang Lyu, Shurui Shi, Jun Huang, Jianlou Si, Wenming Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.01896v1.pdf)  
  Keywords: world model, diffusion model, multi-modal, video generation  
- **[Lucid-XR: An Extended-Reality Data Engine for Robotic Manipulation](https://arxiv.org/abs/2605.00244v1)**  
  Authors: Yajvan Ravan, Adam Rashid, Alan Yu, Kai McClennen, Gio Huh, Kevin Yang, Zhutian Yang, Qinxi Yu, Xiaolong Wang, Phillip Isola, Ge Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.00244v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://lucidxr.github.io)  
  Keywords: simulation, video generation, evaluation, multi-modal, physics  

### Controllable Generation

*Showing the latest 50 out of 130 papers*

- **[iTryOn: Mastering Interactive Video Virtual Try-On with Spatial-Semantic Guidance](https://arxiv.org/abs/2605.21431v1)**  
  Authors: Jun Zheng, Zhengze Xu, Mengting Chen, Jing Wang, Jinsong Lan, Xiaoyong Zhu, Kaifu Zhang, Bo Zheng, Xiaodan Liang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.21431v1.pdf)  
  Keywords: dynamics, video diffusion, interactive, diffusion transformer, benchmark, virtual try-on, temporal consistency, dit, controllable  
- **[CogOmniControl: Reasoning-Driven Controllable Video Generation via Creative Intent Cognition](https://arxiv.org/abs/2605.19995v1)**  
  Authors: Hongji Yang, Songlian Li, Yucheng Zhou, Xiaotong Zhao, Alan Zhao, Chengzhong Xu, Jianbing Shen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.19995v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://um-lab.github.io/CogOmniControl)  
  Keywords: video generation, architecture, diffusion model, benchmark, creative, dit, controllable  
- **[Aero-World: Action-Conditioned Aerial Video Generation from Inertial Controls](https://arxiv.org/abs/2605.19728v1)**  
  Authors: Abdul Mohaimen Al Radi, Kunyang Li, Yuzhang Shang, Mubarak Shah, Yu Tian  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.19728v1.pdf)  
  Keywords: video diffusion, simulation, action-conditioned, acceleration, video generation, physical, evaluation, trajectory, diffusion model, benchmark, physics, image-to-video, controllable, dit, diffusion transformer  
- **[Efficient Long-Context Modeling in Diffusion Language Models via Block Approximate Sparse Attention](https://arxiv.org/abs/2605.19726v1)**  
  Authors: Wenhu Zhang, Yiming Wu, Huanyu Wang, Yaoyang Liu, Huanzhang Dou, Senqiao Yang, Sitong Wu, Hanbin Zhao, Jiaya Jia  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.19726v1.pdf)  
  Keywords: efficient, autoregressive, acceleration, video generation, dit, controllable  
- **[TelePhysics: Physics-Grounded Multi-Object Scene Generation from a Single Image with Real-Time Interaction](https://arxiv.org/abs/2605.20290v1)**  
  Authors: Xin Zhang, Yabo Chen, Yijie Fang, Wanying Qu, Haibin Huang, Chi Zhang, Feng Xu, Xuelong Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20290v1.pdf) | [![GitHub](https://img.shields.io/github/stars/xinzhang007/TelePhysics?style=social)](https://github.com/xinzhang007/TelePhysics)  
  Keywords: simulation, interactive, video generation, physical, video synthesis, physics, controllable  
- **[LMM-Track4D: Eliciting 4D Dynamic Reasoning in LMMs via Trajectory-Grounded Dialogue](https://arxiv.org/abs/2605.19390v1)**  
  Authors: Chaoyue Li, Yongxue Xu, Jie Feng, Jiayu Ding  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.19390v1.pdf) | [![GitHub](https://img.shields.io/github/stars/mikubaka88/LMM-Track4D?style=social)](https://github.com/mikubaka88/LMM-Track4D)  
  Keywords: trajectory, evaluation, streaming, benchmark  
- **[PRISM: A Benchmark for Programmatic Spatial-Temporal Reasoning](https://arxiv.org/abs/2605.19382v1)**  
  Authors: Qiran Zhang, Yuheng Wang, Runde Yang, Lin Wu, Jingru Fan, Shu Yao, Jie Zhang, Tianle Zhou, Huatao Li, Ruijie Shi, Yihan Li, Chen Qian  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.19382v1.pdf)  
  Keywords: style, video generation, evaluation, diffusion model, benchmark, layout  
- **[LongLive-2.0: An NVFP4 Parallel Infrastructure for Long Video Generation](https://arxiv.org/abs/2605.18739v2)**  
  Authors: Yukang Chen, Luozhou Wang, Wei Huang, Shuai Yang, Bohan Zhang, Yicheng Xiao, Ruihang Chu, Weian Mao, Qixin Hu, Shaoteng Liu, Yuyang Zhao, Huizi Mao, Ying-Cong Chen, Enze Xie, Xiaojuan Qi, Song Han  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.18739v2.pdf)  
  Keywords: long video, autoregressive, denoising, interactive, efficient, video generation, architecture, diffusion model, benchmark, layout, distillation, streaming  
- **[Spectral Progressive Diffusion for Efficient Image and Video Generation](https://arxiv.org/abs/2605.18736v2)**  
  Authors: Howard Xiao, Brian Chao, Lior Yariv, Gordon Wetzstein  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.18736v2.pdf)  
  Keywords: autoregressive, denoising, efficient, acceleration, video generation, trajectory, diffusion model  
- **[InstructAV2AV: Instruction-Guided Audio-Video Joint Editing](https://arxiv.org/abs/2605.18467v1)**  
  Authors: Haojie Zheng, Yixin Yang, Siqi Yang, Shuchen Weng, Boxin Shi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.18467v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://hjzheng.net/projects/InstructAV2AV)  
  Keywords: video generation, evaluation, video editing, dit, controllable  

### Human & Character Animation

- **[iTryOn: Mastering Interactive Video Virtual Try-On with Spatial-Semantic Guidance](https://arxiv.org/abs/2605.21431v1)**  
  Authors: Jun Zheng, Zhengze Xu, Mengting Chen, Jing Wang, Jinsong Lan, Xiaoyong Zhu, Kaifu Zhang, Bo Zheng, Xiaodan Liang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.21431v1.pdf)  
  Keywords: dynamics, video diffusion, interactive, diffusion transformer, benchmark, virtual try-on, temporal consistency, dit, controllable  
- **[EverAnimate: Minute-Scale Human Animation via Latent Flow Restoration](https://arxiv.org/abs/2605.15042v1)**  
  Authors: Wuyang Li, Yang Gao, Mariam Hassan, Lan Feng, Wentao Pan, Po-Chien Luan, Alexandre Alahi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.15042v1.pdf)  
  Keywords: identity, efficient, human animation, video generation, human motion, long-form, flow matching  
- **[PhyMotion: Structured 3D Motion Reward for Physics-Grounded Human Video Generation](https://arxiv.org/abs/2605.14269v1)**  
  Authors: Yidong Huang, Zun Wang, Han Lin, Dong-Ki Kim, Shayegan Omidshafiei, Jaehong Yoon, Jaemin Cho, Yue Zhang, Mohit Bansal  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.14269v1.pdf)  
  Keywords: dynamics, autoregressive, video generation, physical, evaluation, human motion, physics  
- **[SocialDirector: Training-Free Social Interaction Control for Multi-Person Video Generation](https://arxiv.org/abs/2605.10079v1)**  
  Authors: Liangyang Ouyang, Ruicong Liu, Caixin Kang, Yifei Huang, Yoichi Sato  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.10079v1.pdf)  
  Keywords: dynamics, video generation, evaluation, robotics, film, gesture  
- **[MoCoTalk: Multi-Conditional Diffusion with Adaptive Router for Controllable Talking Head Generation](https://arxiv.org/abs/2605.08050v1)**  
  Authors: Xinyan Ye, Jiankang Deng, Abbas Edalat  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.08050v1.pdf)  
  Keywords: dynamics, identity, video diffusion, talking head, dit, controllable  
- **[Omni-Fake: Benchmarking Unified Multimodal Social Media Deepfake Detection](https://arxiv.org/abs/2605.01638v1)**  
  Authors: Tianxiao Li, Zhenglin Huang, Haiquan Wen, Yiwei He, Xinze Li, Bingyu Zhu, Wuhui Duan, Congang Chen, Zeyu Fu, Yi Dong, Baoyuan Wu, Jason Li, Guangliang Cheng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.01638v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://tianxiao1201.github.io/omni-fake-project-page)  
  Keywords: benchmark, dit, talking head  
- **[Generate Your Talking Avatar from Video Reference](https://arxiv.org/abs/2604.27918v1)**  
  Authors: Zujin Guo, Zhenhui Ye, Yi Ren, Yuanming Li, Ce Chen, Zhibin Hong, Chen Change Loy  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2604.27918v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://www.heygen.com/research)  
  Keywords: identity, benchmark, image-to-video, avatar, dit  
- **[HuM-Eval: A Coarse-to-Fine Framework for Human-Centric Video Evaluation](https://arxiv.org/abs/2604.25361v1)**  
  Authors: Bingzi Zhang, Kaisi Guan, Ruihua Song  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2604.25361v1.pdf)  
  Keywords: text-to-video, video generation, evaluation, benchmark, human motion  
- **[Talker-T2AV: Joint Talking Audio-Video Generation with Autoregressive Diffusion Modeling](https://arxiv.org/abs/2604.23586v1)**  
  Authors: Zhen Ye, Xu Tan, Aoxiong Yin, Hongzhan Lin, Guangyan Zhang, Peiwen Sun, Yiming Li, Chi-Min Chan, Wei Ye, Shikun Zhang, Wei Xue  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2604.23586v1.pdf)  
  Keywords: autoregressive, denoising, video generation, talking head, diffusion model, benchmark, diffusion transformer  
- **[EAD-Net: Emotion-Aware Talking Head Generation with Spatial Refinement and Temporal Coherence](https://arxiv.org/abs/2604.23325v1)**  
  Authors: Yahui Li, Yinfeng Yu, Liejun Wang, Shengjie Shen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2604.23325v1.pdf)  
  Keywords: long video, talking head, video generation, multi-modal, temporal consistency, dit  

### Image-to-Video Generation

- **[Aero-World: Action-Conditioned Aerial Video Generation from Inertial Controls](https://arxiv.org/abs/2605.19728v1)**  
  Authors: Abdul Mohaimen Al Radi, Kunyang Li, Yuzhang Shang, Mubarak Shah, Yu Tian  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.19728v1.pdf)  
  Keywords: video diffusion, simulation, action-conditioned, acceleration, video generation, physical, evaluation, trajectory, diffusion model, benchmark, physics, image-to-video, controllable, dit, diffusion transformer  
- **[Rebalancing Reference Frame Dominance to Improve Motion in Image-to-Video Models](https://arxiv.org/abs/2605.19398v2)**  
  Authors: Wooseok Jeon, Seungho Park, Seunghyun Shin, Sangeyl Lee, Hyeonho Jeong, Hae-Gon Jeon  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.19398v2.pdf)  
  Keywords: dynamics, denoising, text-to-video, image-to-video, i2v, dit  
- **[Image-to-Video Diffusion: From Foundations to Open Frontiers](https://arxiv.org/abs/2605.17248v1)**  
  Authors: Xianlong Wang, Wenbo Pan, Shijia Zhou, Ke Li, Yuqi Wang, Zeyu Ye, Hangtao Zhang, Leo Yu Zhang, Xiaohua Jia  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.17248v1.pdf)  
  Keywords: identity, video diffusion, video generation, architecture, evaluation, image-to-video, i2v, dit  
- **[3DPhysVideo: Consistency-Guided Flow SDE for Video Generation via 3D Scene Reconstruction and Physical Simulation](https://arxiv.org/abs/2605.16795v1)**  
  Authors: Hwidong Kim, Yunho Kim, Tae-Kyun Kim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.16795v1.pdf)  
  Keywords: dynamics, denoising, simulation, efficient, video generation, physical, evaluation, physical simulation, novel view, benchmark, physics, image-to-video, i2v, dit  
- **[FashionChameleon: Towards Real-Time and Interactive Human-Garment Video Customization](https://arxiv.org/abs/2605.15824v1)**  
  Authors: Quanjian Song, Yefeng Shen, Mengting Chen, Hao Sun, Jinsong Lan, Xiaoyong Zhu, Bo Zheng, Liujuan Cao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.15824v1.pdf)  
  Keywords: autoregressive, interactive, video generation, distillation, image-to-video, streaming, customization  
- **[RefDecoder: Enhancing Visual Generation with Conditional Video Decoding](https://arxiv.org/abs/2605.15196v1)**  
  Authors: Xiang Fan, Yuheng Wang, Bohan Fang, Zhongzheng Ren, Ranjay Krishna  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.15196v1.pdf)  
  Keywords: denoising, style, video generation, diffusion model, benchmark, video editing, i2v, dit  
- **[MechVerse: Evaluating Physical Motion Consistency in Video Generation Models](https://arxiv.org/abs/2605.14843v1)**  
  Authors: Rahul Jain, Mayank Patel, Asim Unmesh, Karthik Ramani  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.14843v1.pdf)  
  Keywords: video generation, physical, benchmark, image-to-video, dit  
- **[Video Reconstruction using Diffusion-based Image-to-Video Generation with Trajectory Guidance](https://arxiv.org/abs/2605.16420v1)**  
  Authors: Stelio Bompai, Ioannis Kontopoulos, Giannis Spiliopoulos, Dimitris Zissis, Konstantinos Tserpes  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.16420v1.pdf)  
  Keywords: video diffusion, video generation, trajectory, diffusion model, benchmark, image-to-video, i2v, dit  
- **[Improving Human Image Animation via Semantic Representation Alignment](https://arxiv.org/abs/2605.10523v1)**  
  Authors: Chang Liu, Mengting Chen, Yixuan Huang, Haoning Wu, Chen Ju, Shuai Xiao, Jinsong Lan, Yanfeng Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.10523v1.pdf)  
  Keywords: identity, long video, video generation, diffusion model, image animation, image-to-video, dit  
- **[Progressive Photorealistic Simplification](https://arxiv.org/abs/2605.10409v1)**  
  Authors: Adi Rosenthal, Dana Berman, Yedid Hoshen, Ariel Shamir  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.10409v1.pdf)  
  Keywords: image-to-video, interactive, dit, video generation  

### Long Video Generation

*Showing the latest 50 out of 125 papers*

- **[StreamGVE: Training-Free Video Editing via Few-Step Streaming Video Generation](https://arxiv.org/abs/2605.21466v1)**  
  Authors: Guanlong Jiao, Chenyangguang Zhang, Jia Jun Cheng Xian, Zewei Zhang, Renjie Liao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.21466v1.pdf)  
  Keywords: streaming, video editing, dit, video generation  
- **[iTryOn: Mastering Interactive Video Virtual Try-On with Spatial-Semantic Guidance](https://arxiv.org/abs/2605.21431v1)**  
  Authors: Jun Zheng, Zhengze Xu, Mengting Chen, Jing Wang, Jinsong Lan, Xiaoyong Zhu, Kaifu Zhang, Bo Zheng, Xiaodan Liang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.21431v1.pdf)  
  Keywords: dynamics, video diffusion, interactive, diffusion transformer, benchmark, virtual try-on, temporal consistency, dit, controllable  
- **[Q-ARVD: Quantizing Autoregressive Video Diffusion Models](https://arxiv.org/abs/2605.21072v1)**  
  Authors: Siao Tang, Xinyin Ma, Gongfan Fang, Xingyi Yang, Xinchao Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.21072v1.pdf)  
  Keywords: autoregressive, video diffusion, interactive, video generation, world model, architecture, diffusion model, streaming, diffusion transformer  
- **[DySink: Dynamic Frame Sinks for Autoregressive Long Video Generation](https://arxiv.org/abs/2605.21028v1)**  
  Authors: Bo Ye, Xinyu Cui, Jian Zhao, Tong Wei, Min-Ling Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.21028v1.pdf) | [![GitHub](https://img.shields.io/github/stars/yebo0216best/DySink?style=social)](https://github.com/yebo0216best/DySink)  
  Keywords: streaming, long video, autoregressive, video generation  
- **[FlowLong: Inference-time Long Video Generation via Manifold-constrained Tweedie Matching](https://arxiv.org/abs/2605.20910v1)**  
  Authors: Jangho Park, Geon Yeong Park, Gihyun Kwon, Jong Chul Ye  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20910v1.pdf)  
  Keywords: long video, video diffusion, autoregressive, video generation, architecture, diffusion model, temporal consistency, dit  
- **[RoPeSLR: 3D RoPE-driven Sparse-LowRank Attention for Efficient Diffusion Transformers](https://arxiv.org/abs/2605.20659v1)**  
  Authors: Yuxi Liu, Zekun Zhang, Yixiang Cai, Renjia Deng, Yutong He, Kun Yuan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20659v1.pdf)  
  Keywords: long video, efficient, video generation, evaluation, dit, diffusion transformer  
- **[Accelerating Video Inverse Problem Solvers with Autoregressive Diffusion Models](https://arxiv.org/abs/2605.20624v1)**  
  Authors: Taesung Kwon, Jonghyun Park, Hyungjin Chung, Jong Chul Ye  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20624v1.pdf)  
  Keywords: autoregressive, video diffusion, diffusion model, video restoration, streaming  
- **[Goodbye Drift: Anchored Tree Sampling for Long-Horizon Video-to-Video Generation](https://arxiv.org/abs/2605.20476v1)**  
  Authors: Matthew Bendel, Stephen W. Bailey, Mithilesh Vaidya, Sumukh Badam, Xingzhe He  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20476v1.pdf)  
  Keywords: autoregressive, style, video generation, outpainting, t2v, distillation, video-to-video, dit  
- **[Efficient Long-Context Modeling in Diffusion Language Models via Block Approximate Sparse Attention](https://arxiv.org/abs/2605.19726v1)**  
  Authors: Wenhu Zhang, Yiming Wu, Huanyu Wang, Yaoyang Liu, Huanzhang Dou, Senqiao Yang, Sitong Wu, Hanbin Zhao, Jiaya Jia  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.19726v1.pdf)  
  Keywords: efficient, autoregressive, acceleration, video generation, dit, controllable  
- **[LMM-Track4D: Eliciting 4D Dynamic Reasoning in LMMs via Trajectory-Grounded Dialogue](https://arxiv.org/abs/2605.19390v1)**  
  Authors: Chaoyue Li, Yongxue Xu, Jie Feng, Jiayu Ding  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.19390v1.pdf) | [![GitHub](https://img.shields.io/github/stars/mikubaka88/LMM-Track4D?style=social)](https://github.com/mikubaka88/LMM-Track4D)  
  Keywords: trajectory, evaluation, streaming, benchmark  

### Personalization & Customization

*Showing the latest 50 out of 83 papers*

- **[Goodbye Drift: Anchored Tree Sampling for Long-Horizon Video-to-Video Generation](https://arxiv.org/abs/2605.20476v1)**  
  Authors: Matthew Bendel, Stephen W. Bailey, Mithilesh Vaidya, Sumukh Badam, Xingzhe He  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20476v1.pdf)  
  Keywords: autoregressive, style, video generation, outpainting, t2v, distillation, video-to-video, dit  
- **[Tiny-Engram: Trigger-Indexed Concept Tables for Generative Vision](https://arxiv.org/abs/2605.20309v1)**  
  Authors: Runyuan Cai, Yiming Wang, Yu Lin, Xiaodong Zeng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20309v1.pdf)  
  Keywords: identity, video diffusion, video generation, concept, personalization, dit  
- **[PRISM: A Benchmark for Programmatic Spatial-Temporal Reasoning](https://arxiv.org/abs/2605.19382v1)**  
  Authors: Qiran Zhang, Yuheng Wang, Runde Yang, Lin Wu, Jingru Fan, Shu Yao, Jie Zhang, Tianle Zhou, Huatao Li, Ruijie Shi, Yihan Li, Chen Qian  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.19382v1.pdf)  
  Keywords: style, video generation, evaluation, diffusion model, benchmark, layout  
- **[Artifact-Bench: Evaluating MLLMs on Detecting and Assessing the Artifacts of AI-Generated Videos](https://arxiv.org/abs/2605.18984v1)**  
  Authors: Yuqi Tang, Yang Shi, Zhuoran Zhang, Qixun Wang, Xuehai Bai, Yue Ding, Ruizhe Chen, Bohan Zeng, Xinlong Chen, Xuanyu Zhu, Bozhou Li, Yuran Wang, Yifan Dai, Chengzhuo Tong, Xinyu Liu, Yiyan Ji, Yujie Wei, Yuhao Dong, Shilin Yan, Fengxiang Wang, Yi-Fan Zhang, Haotian Wang, Yuanxing Zhang, Pengfei Wan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.18984v1.pdf)  
  Keywords: evaluation, benchmark, style  
- **[Aurora: Unified Video Editing with a Tool-Using Agent](https://arxiv.org/abs/2605.18748v1)**  
  Authors: Yongsheng Yu, Ziyun Zeng, Zhiyuan Xiao, Zhenghong Zhou, Hang Hua, Wei Xiong, Jiebo Luo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.18748v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://yeates.github.io/Aurora-Page)  
  Keywords: video diffusion, style, benchmark, video editing, dit, diffusion transformer  
- **[Advancing Narrative Long Video Generation via Training-Free Identity-Aware Memory](https://arxiv.org/abs/2605.18733v1)**  
  Authors: Jinzhuo Liu, Jiangning Zhang, Wencan Jiang, Yabiao Wang, Dingkang Liang, Zhucun Xue, Ran Yi, Yong Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.18733v1.pdf)  
  Keywords: identity, long video, autoregressive, efficient, acceleration, video generation, evaluation, benchmark, streaming, dit  
- **[GeoFlow: Enforcing Implicit Geometric Consistency in Video Generation](https://arxiv.org/abs/2605.18365v1)**  
  Authors: Jan Ackermann, Shengqu Cai, Boyang Deng, Zhengfei Kuang, Songyou Peng, Gordon Wetzstein  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.18365v1.pdf)  
  Keywords: identity, video diffusion, text-to-video, video generation, physical, diffusion model  
- **[Omni-Customizer: End-to-End MultiModal Customization for Joint Audio-Video Generation](https://arxiv.org/abs/2605.17488v1)**  
  Authors: Yuheng Chen, Qingdong He, Teng Hu, Yuji Wang, Yabiao Wang, Lizhuang Ma, Jiangning Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.17488v1.pdf)  
  Keywords: architecture, identity, customization, video generation  
- **[Soap2Soap: Long Cinematic Video Remaking via Multi-Agent Collaboration](https://arxiv.org/abs/2605.17423v1)**  
  Authors: Yiren Song, Huilin Zhong, Kevin Qinghong Lin, Haofan Wang, Mike Zheng Shou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.17423v1.pdf)  
  Keywords: identity, video generation, video synthesis, film, video-to-video, dit  
- **[Image-to-Video Diffusion: From Foundations to Open Frontiers](https://arxiv.org/abs/2605.17248v1)**  
  Authors: Xianlong Wang, Wenbo Pan, Shijia Zhou, Ke Li, Yuqi Wang, Zeyu Ye, Hangtao Zhang, Leo Yu Zhang, Xiaohua Jia  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.17248v1.pdf)  
  Keywords: identity, video diffusion, video generation, architecture, evaluation, image-to-video, i2v, dit  

### Physical Understanding

*Showing the latest 50 out of 150 papers*

- **[iTryOn: Mastering Interactive Video Virtual Try-On with Spatial-Semantic Guidance](https://arxiv.org/abs/2605.21431v1)**  
  Authors: Jun Zheng, Zhengze Xu, Mengting Chen, Jing Wang, Jinsong Lan, Xiaoyong Zhu, Kaifu Zhang, Bo Zheng, Xiaodan Liang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.21431v1.pdf)  
  Keywords: dynamics, video diffusion, interactive, diffusion transformer, benchmark, virtual try-on, temporal consistency, dit, controllable  
- **[Aero-World: Action-Conditioned Aerial Video Generation from Inertial Controls](https://arxiv.org/abs/2605.19728v1)**  
  Authors: Abdul Mohaimen Al Radi, Kunyang Li, Yuzhang Shang, Mubarak Shah, Yu Tian  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.19728v1.pdf)  
  Keywords: video diffusion, simulation, action-conditioned, acceleration, video generation, physical, evaluation, trajectory, diffusion model, benchmark, physics, image-to-video, controllable, dit, diffusion transformer  
- **[TelePhysics: Physics-Grounded Multi-Object Scene Generation from a Single Image with Real-Time Interaction](https://arxiv.org/abs/2605.20290v1)**  
  Authors: Xin Zhang, Yabo Chen, Yijie Fang, Wanying Qu, Haibin Huang, Chi Zhang, Feng Xu, Xuelong Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20290v1.pdf) | [![GitHub](https://img.shields.io/github/stars/xinzhang007/TelePhysics?style=social)](https://github.com/xinzhang007/TelePhysics)  
  Keywords: simulation, interactive, video generation, physical, video synthesis, physics, controllable  
- **[Rebalancing Reference Frame Dominance to Improve Motion in Image-to-Video Models](https://arxiv.org/abs/2605.19398v2)**  
  Authors: Wooseok Jeon, Seungho Park, Seunghyun Shin, Sangeyl Lee, Hyeonho Jeong, Hae-Gon Jeon  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.19398v2.pdf)  
  Keywords: dynamics, denoising, text-to-video, image-to-video, i2v, dit  
- **[PhyWorld: Physics-Faithful World Model for Video Generation](https://arxiv.org/abs/2605.19242v1)**  
  Authors: Pu Zhao, Juyi Lin, Timothy Rupprecht, Arash Akbari, Chence Yang, Rahul Chowdhury, Elaheh Motamedi, Arman Akbari, Yumei He, Chen Wang, Geng Yuan, Weiwei Chen, Yanzhi Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.19242v1.pdf)  
  Keywords: dynamics, world model, video generation, physical, benchmark, world simulator, physics, video-to-video, flow matching, dit  
- **[WorldString: Actionable World Representation](https://arxiv.org/abs/2605.18743v2)**  
  Authors: Kunqi Xu, Jitao Li, Jianglong Ye, Tianshu Tang, Isabella Liu, Sifei Liu, Xueyan Zou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.18743v2.pdf)  
  Keywords: dynamics, world model, architecture, physical, video generation  
- **[NEWTON: Agentic Planning for Physically Grounded Video Generation](https://arxiv.org/abs/2605.18396v2)**  
  Authors: Yuxiang Feng, Juncheng Wang, Chao Xu, Yijie Qian, Huihan Wang, Wenlong Hou, Yang Liu, Baigui Sun, Yong Liu, Shujun Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.18396v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://Newton026.github.io/newton)  
  Keywords: dynamics, physics-aware, video generation, physical, physics, dit  
- **[GeoFlow: Enforcing Implicit Geometric Consistency in Video Generation](https://arxiv.org/abs/2605.18365v1)**  
  Authors: Jan Ackermann, Shengqu Cai, Boyang Deng, Zhengfei Kuang, Songyou Peng, Gordon Wetzstein  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.18365v1.pdf)  
  Keywords: identity, video diffusion, text-to-video, video generation, physical, diffusion model  
- **[EgoInteract: Synthetic Egocentric Videos Generation for Interaction Understanding and Anticipation](https://arxiv.org/abs/2605.18214v1)**  
  Authors: Rosario Leonardi, Francesco Ragusa, Daniele Materia, Alessandro Passanisi, James Fort, Jakob Engel, Giovanni Maria Farinella  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.18214v1.pdf)  
  Keywords: dynamics, simulation, video generation, benchmark, controllable  
- **[3DPhysVideo: Consistency-Guided Flow SDE for Video Generation via 3D Scene Reconstruction and Physical Simulation](https://arxiv.org/abs/2605.16795v1)**  
  Authors: Hwidong Kim, Yunho Kim, Tae-Kyun Kim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.16795v1.pdf)  
  Keywords: dynamics, denoising, simulation, efficient, video generation, physical, evaluation, physical simulation, novel view, benchmark, physics, image-to-video, i2v, dit  

### Surveys & Benchmarks

*Showing the latest 50 out of 228 papers*

- **[iTryOn: Mastering Interactive Video Virtual Try-On with Spatial-Semantic Guidance](https://arxiv.org/abs/2605.21431v1)**  
  Authors: Jun Zheng, Zhengze Xu, Mengting Chen, Jing Wang, Jinsong Lan, Xiaoyong Zhu, Kaifu Zhang, Bo Zheng, Xiaodan Liang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.21431v1.pdf)  
  Keywords: dynamics, video diffusion, interactive, diffusion transformer, benchmark, virtual try-on, temporal consistency, dit, controllable  
- **[Preserve, Reveal, Expand: Faithful 4D Video Editing with Region-Aware Conditioning](https://arxiv.org/abs/2605.20961v1)**  
  Authors: Zhangchi Hu, Wenzhang Sun, Xiangchen Yin, Jiahui Yuan, Chunfeng Wang, Hao Li, Kun Zhan, Xiaoyan Sun  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20961v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://ricepastem.github.io/PREX-Open)  
  Keywords: video diffusion, evaluation, diffusion model, benchmark, video editing, dit  
- **[VSCD: Video-based Scene Change Detection in Unaligned Scenes](https://arxiv.org/abs/2605.20821v1)**  
  Authors: Jiae Yoon, Ue-Hwan Kim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20821v1.pdf)  
  Keywords: simulation, benchmark  
- **[What Semantics Survive the Connector? Diagnosing VLM-to-DiT Alignment in Video Editing](https://arxiv.org/abs/2605.20795v1)**  
  Authors: Hangyu Lin, Chao Wen, Chengming Xu, Jianxiong Gao, Jiangning Zhang, Xiaobin Hu, Yanwei Fu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20795v1.pdf)  
  Keywords: architecture, evaluation, multi-modal, video editing, flow matching, dit  
- **[RoPeSLR: 3D RoPE-driven Sparse-LowRank Attention for Efficient Diffusion Transformers](https://arxiv.org/abs/2605.20659v1)**  
  Authors: Yuxi Liu, Zekun Zhang, Yixiang Cai, Renjia Deng, Yutong He, Kun Yuan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20659v1.pdf)  
  Keywords: long video, efficient, video generation, evaluation, dit, diffusion transformer  
- **[MSAVBench: Towards Comprehensive and Reliable Evaluation of Multi-Shot Audio-Video Generation](https://arxiv.org/abs/2605.20183v1)**  
  Authors: Yujie Wei, Yujin Han, Zhekai Chen, Yongming Li, Kaixun Jiang, Zhihang Liu, Quanhao Li, Zhiwu Qing, Xiang Wang, Zhen Xing, Ruihang Chu, Lingyi Hong, Yefei He, Junjie Zhou, Junqiu Yu, Yang Shi, Difan Zou, Kai Zhu, Shiwei Zhang, Yingya Zhang, Yu Liu, Xihui Liu, Hongming Shan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20183v1.pdf)  
  Keywords: evaluation, benchmark, video generation  
- **[CogOmniControl: Reasoning-Driven Controllable Video Generation via Creative Intent Cognition](https://arxiv.org/abs/2605.19995v1)**  
  Authors: Hongji Yang, Songlian Li, Yucheng Zhou, Xiaotong Zhao, Alan Zhao, Chengzhong Xu, Jianbing Shen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.19995v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://um-lab.github.io/CogOmniControl)  
  Keywords: video generation, architecture, diffusion model, benchmark, creative, dit, controllable  
- **[Aero-World: Action-Conditioned Aerial Video Generation from Inertial Controls](https://arxiv.org/abs/2605.19728v1)**  
  Authors: Abdul Mohaimen Al Radi, Kunyang Li, Yuzhang Shang, Mubarak Shah, Yu Tian  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.19728v1.pdf)  
  Keywords: video diffusion, simulation, action-conditioned, acceleration, video generation, physical, evaluation, trajectory, diffusion model, benchmark, physics, image-to-video, controllable, dit, diffusion transformer  
- **[LMM-Track4D: Eliciting 4D Dynamic Reasoning in LMMs via Trajectory-Grounded Dialogue](https://arxiv.org/abs/2605.19390v1)**  
  Authors: Chaoyue Li, Yongxue Xu, Jie Feng, Jiayu Ding  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.19390v1.pdf) | [![GitHub](https://img.shields.io/github/stars/mikubaka88/LMM-Track4D?style=social)](https://github.com/mikubaka88/LMM-Track4D)  
  Keywords: trajectory, evaluation, streaming, benchmark  
- **[PRISM: A Benchmark for Programmatic Spatial-Temporal Reasoning](https://arxiv.org/abs/2605.19382v1)**  
  Authors: Qiran Zhang, Yuheng Wang, Runde Yang, Lin Wu, Jingru Fan, Shu Yao, Jie Zhang, Tianle Zhou, Huatao Li, Ruijie Shi, Yihan Li, Chen Qian  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.19382v1.pdf)  
  Keywords: style, video generation, evaluation, diffusion model, benchmark, layout  

### Text-to-Video Generation

- **[Goodbye Drift: Anchored Tree Sampling for Long-Horizon Video-to-Video Generation](https://arxiv.org/abs/2605.20476v1)**  
  Authors: Matthew Bendel, Stephen W. Bailey, Mithilesh Vaidya, Sumukh Badam, Xingzhe He  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20476v1.pdf)  
  Keywords: autoregressive, style, video generation, outpainting, t2v, distillation, video-to-video, dit  
- **[Rebalancing Reference Frame Dominance to Improve Motion in Image-to-Video Models](https://arxiv.org/abs/2605.19398v2)**  
  Authors: Wooseok Jeon, Seungho Park, Seunghyun Shin, Sangeyl Lee, Hyeonho Jeong, Hae-Gon Jeon  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.19398v2.pdf)  
  Keywords: dynamics, denoising, text-to-video, image-to-video, i2v, dit  
- **[GeoFlow: Enforcing Implicit Geometric Consistency in Video Generation](https://arxiv.org/abs/2605.18365v1)**  
  Authors: Jan Ackermann, Shengqu Cai, Boyang Deng, Zhengfei Kuang, Songyou Peng, Gordon Wetzstein  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.18365v1.pdf)  
  Keywords: identity, video diffusion, text-to-video, video generation, physical, diffusion model  
- **[StreamingEffect: Real-Time Human-Centric Video Effect Generation](https://arxiv.org/abs/2605.17019v1)**  
  Authors: Yiren Song, Cheng Liu, Yuxin Jiang, Mike Zheng Shou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.17019v1.pdf)  
  Keywords: identity, autoregressive, efficient, text-to-video, interactive, video generation, acceleration, architecture, distillation, video editing, video-to-video, temporal consistency, streaming, dit  
- **[Accelerating Rectified Flow Models via Trajectory-Aware Caching](https://arxiv.org/abs/2605.16789v1)**  
  Authors: Xiao Liu, Kai Liu, Naiyang Guan, Hongliang Lu, Zhixin Wang, Zhikai Chen, Renjing Pei, Yulun Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.16789v1.pdf)  
  Keywords: rectified flow, acceleration, text-to-video, video generation, trajectory, evaluation, dit  
- **[MAVEN A Multi-Agent Framework for Multicultural Text-to-Video Generation](https://arxiv.org/abs/2605.16716v1)**  
  Authors: Shuowei Li, Yuming Zhao, Parth Bhalerao, Oana Ignat  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.16716v1.pdf) | [![GitHub](https://img.shields.io/github/stars/AIM-SCU/CRAFT?style=social)](https://github.com/AIM-SCU/CRAFT)  
  Keywords: text-to-video, video generation, evaluation, t2v, benchmark, temporal consistency  
- **[Compositional Video Generation via Inference-Time Guidance](https://arxiv.org/abs/2605.14988v1)**  
  Authors: Ariel Shaulov, Eitan Shaar, Amit Edenzon, Gal Chechik, Lior Wolf  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.14988v1.pdf)  
  Keywords: video diffusion, denoising, text-to-video, video generation, architecture, trajectory, concept, diffusion model, benchmark, layout  
- **[TeDiO: Temporal Diagonal Optimization for Training-Free Coherent Video Diffusion](https://arxiv.org/abs/2605.14136v1)**  
  Authors: Nurislam Tursynbek, Zhiqiang Lao, Heather Yu, Gedas Bertasius, Marc Niethammer  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.14136v1.pdf)  
  Keywords: dynamics, video diffusion, efficient, text-to-video, video generation, diffusion model, temporal consistency, diffusion transformer  
- **[Not All Tokens Need 40 Steps: Heterogeneous Step Allocation in Diffusion Transformers for Efficient Video Generation](https://arxiv.org/abs/2605.06892v1)**  
  Authors: Ernie Chu, Vishal M. Patel  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.06892v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://ernestchu.github.io/hsa)  
  Keywords: dynamics, denoising, efficient, text-to-video, acceleration, video generation, evaluation, t2v, image-to-video, flow matching, i2v, dit, diffusion transformer  
- **[FaithfulFaces: Pose-Faithful Facial Identity Preservation for Text-to-Video Generation](https://arxiv.org/abs/2605.04702v1)**  
  Authors: Yuanzhi Wang, Xuhua Ren, Jiaxiang Cheng, Bing Ma, Kai Yu, Sen Liang, Wenyue Li, Tianxiang Zheng, Qinglin Lu, Zhen Cui  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.04702v1.pdf)  
  Keywords: identity, t2v, text-to-video, video generation  

### Video Editing

- **[StreamGVE: Training-Free Video Editing via Few-Step Streaming Video Generation](https://arxiv.org/abs/2605.21466v1)**  
  Authors: Guanlong Jiao, Chenyangguang Zhang, Jia Jun Cheng Xian, Zewei Zhang, Renjie Liao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.21466v1.pdf)  
  Keywords: streaming, video editing, dit, video generation  
- **[Preserve, Reveal, Expand: Faithful 4D Video Editing with Region-Aware Conditioning](https://arxiv.org/abs/2605.20961v1)**  
  Authors: Zhangchi Hu, Wenzhang Sun, Xiangchen Yin, Jiahui Yuan, Chunfeng Wang, Hao Li, Kun Zhan, Xiaoyan Sun  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20961v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://ricepastem.github.io/PREX-Open)  
  Keywords: video diffusion, evaluation, diffusion model, benchmark, video editing, dit  
- **[What Semantics Survive the Connector? Diagnosing VLM-to-DiT Alignment in Video Editing](https://arxiv.org/abs/2605.20795v1)**  
  Authors: Hangyu Lin, Chao Wen, Chengming Xu, Jianxiong Gao, Jiangning Zhang, Xiaobin Hu, Yanwei Fu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20795v1.pdf)  
  Keywords: architecture, evaluation, multi-modal, video editing, flow matching, dit  
- **[Goodbye Drift: Anchored Tree Sampling for Long-Horizon Video-to-Video Generation](https://arxiv.org/abs/2605.20476v1)**  
  Authors: Matthew Bendel, Stephen W. Bailey, Mithilesh Vaidya, Sumukh Badam, Xingzhe He  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20476v1.pdf)  
  Keywords: autoregressive, style, video generation, outpainting, t2v, distillation, video-to-video, dit  
- **[PhyWorld: Physics-Faithful World Model for Video Generation](https://arxiv.org/abs/2605.19242v1)**  
  Authors: Pu Zhao, Juyi Lin, Timothy Rupprecht, Arash Akbari, Chence Yang, Rahul Chowdhury, Elaheh Motamedi, Arman Akbari, Yumei He, Chen Wang, Geng Yuan, Weiwei Chen, Yanzhi Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.19242v1.pdf)  
  Keywords: dynamics, world model, video generation, physical, benchmark, world simulator, physics, video-to-video, flow matching, dit  
- **[Aurora: Unified Video Editing with a Tool-Using Agent](https://arxiv.org/abs/2605.18748v1)**  
  Authors: Yongsheng Yu, Ziyun Zeng, Zhiyuan Xiao, Zhenghong Zhou, Hang Hua, Wei Xiong, Jiebo Luo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.18748v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://yeates.github.io/Aurora-Page)  
  Keywords: video diffusion, style, benchmark, video editing, dit, diffusion transformer  
- **[InstructAV2AV: Instruction-Guided Audio-Video Joint Editing](https://arxiv.org/abs/2605.18467v1)**  
  Authors: Haojie Zheng, Yixin Yang, Siqi Yang, Shuchen Weng, Boxin Shi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.18467v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://hjzheng.net/projects/InstructAV2AV)  
  Keywords: video generation, evaluation, video editing, dit, controllable  
- **[Soap2Soap: Long Cinematic Video Remaking via Multi-Agent Collaboration](https://arxiv.org/abs/2605.17423v1)**  
  Authors: Yiren Song, Huilin Zhong, Kevin Qinghong Lin, Haofan Wang, Mike Zheng Shou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.17423v1.pdf)  
  Keywords: identity, video generation, video synthesis, film, video-to-video, dit  
- **[StreamingEffect: Real-Time Human-Centric Video Effect Generation](https://arxiv.org/abs/2605.17019v1)**  
  Authors: Yiren Song, Cheng Liu, Yuxin Jiang, Mike Zheng Shou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.17019v1.pdf)  
  Keywords: identity, autoregressive, efficient, text-to-video, interactive, video generation, acceleration, architecture, distillation, video editing, video-to-video, temporal consistency, streaming, dit  
- **[SWoMo: Neuro-Symbolic World Model for Cataract Surgery Simulation](https://arxiv.org/abs/2605.16530v2)**  
  Authors: Ssharvien Kumar Sivakumar, Akwele Johnson, Anirudh Dhingra, Yannik Frisch, Ghazal Ghazaei, Anirban Mukhopadhyay  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.16530v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://ssharvienkumar.github.io/SWoMo)  
  Keywords: dynamics, video diffusion, simulation, style, world model, physical, diffusion model, video style transfer, dit  

### Video Inpainting & Completion

- **[Goodbye Drift: Anchored Tree Sampling for Long-Horizon Video-to-Video Generation](https://arxiv.org/abs/2605.20476v1)**  
  Authors: Matthew Bendel, Stephen W. Bailey, Mithilesh Vaidya, Sumukh Badam, Xingzhe He  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20476v1.pdf)  
  Keywords: autoregressive, style, video generation, outpainting, t2v, distillation, video-to-video, dit  
- **[Relit-LiVE: Relight Video by Jointly Learning Environment Video](https://arxiv.org/abs/2605.06658v1)**  
  Authors: Weiqing Xiao, Hong Li, Xiuyu Yang, Houyuan Chen, Wenyi Li, Tianqi Liu, Shaocong Xu, Chongjie Ye, Hao Zhao, Beibei Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.06658v1.pdf) | [![GitHub](https://img.shields.io/github/stars/zhuxing0/Relit-LiVE?style=social)](https://github.com/zhuxing0/Relit-LiVE)  
  Keywords: video diffusion, video prediction, physical, diffusion model, benchmark, streaming, dit  
- **[Quaternion Nonlinear Transform-Induced Nuclear Norm for Low-Rank Tensor Completion](https://arxiv.org/abs/2605.01467v1)**  
  Authors: Biswarup Karmakar, Ratikanta Behera  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.01467v1.pdf)  
  Keywords: efficient, benchmark, video inpainting  
- **[LMGenDrive: Bridging Multimodal Understanding and Generative World Modeling for End-to-End Driving](https://arxiv.org/abs/2604.08719v1)**  
  Authors: Hao Shao, Letian Wang, Yang Zhou, Yuxuan Hu, Zhuofan Zong, Steven L. Waslander, Wei Zhan, Hongsheng Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2604.08719v1.pdf)  
  Keywords: autoregressive, video prediction, world model, video generation, benchmark, autonomous driving  
- **[Novel View Synthesis as Video Completion](https://arxiv.org/abs/2604.08500v1)**  
  Authors: Qi Wu, Khiem Vuong, Minsik Jeon, Srinivasa Narasimhan, Deva Ramanan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2604.08500v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://frame-crafter.github.io)  
  Keywords: video diffusion, diffusion model, benchmark, novel view, video completion  
- **[SEM-ROVER: Semantic Voxel-Guided Diffusion for Large-Scale Driving Scene Generation](https://arxiv.org/abs/2604.06113v1)**  
  Authors: Hiba Dahmani, Nathan Piasco, Moussab Bennehar, Luis Roldão, Dzmitry Tsishkou, Laurent Caraffa, Jean-Philippe Tarel, Roland Brémond  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2604.06113v1.pdf)  
  Keywords: outpainting, diffusion model, dit  
- **[ChopGrad: Pixel-Wise Losses for Latent Video Diffusion via Truncated Backpropagation](https://arxiv.org/abs/2603.17812v2)**  
  Authors: Dmitriy Rivkin, Parker Ewen, Lili Gao, Julian Ost, Stefanie Walz, Rasika Kangutkar, Mario Bijelic, Felix Heide  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2603.17812v2.pdf)  
  Keywords: video diffusion, efficient, video generation, video enhancement, diffusion model, latent video, video inpainting, super-resolution, dit  

### Video Super-Resolution & Enhancement

*Showing the latest 50 out of 72 papers*

- **[Dynamic Video Generation: Shaping Video Generation Across Time and Space](https://arxiv.org/abs/2605.21042v1)**  
  Authors: Shikang Zheng, Jingkai Huang, Jiacheng Liu, Guantao Chen, Lixuan, Yuqi Lin, Peiliang Cai, Linfeng Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.21042v1.pdf)  
  Keywords: efficient, acceleration, denoising, video generation, diffusion model, distillation, dit  
- **[Accelerating Video Inverse Problem Solvers with Autoregressive Diffusion Models](https://arxiv.org/abs/2605.20624v1)**  
  Authors: Taesung Kwon, Jonghyun Park, Hyungjin Chung, Jong Chul Ye  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20624v1.pdf)  
  Keywords: autoregressive, video diffusion, diffusion model, video restoration, streaming  
- **[Rebalancing Reference Frame Dominance to Improve Motion in Image-to-Video Models](https://arxiv.org/abs/2605.19398v2)**  
  Authors: Wooseok Jeon, Seungho Park, Seunghyun Shin, Sangeyl Lee, Hyeonho Jeong, Hae-Gon Jeon  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.19398v2.pdf)  
  Keywords: dynamics, denoising, text-to-video, image-to-video, i2v, dit  
- **[LongLive-2.0: An NVFP4 Parallel Infrastructure for Long Video Generation](https://arxiv.org/abs/2605.18739v2)**  
  Authors: Yukang Chen, Luozhou Wang, Wei Huang, Shuai Yang, Bohan Zhang, Yicheng Xiao, Ruihang Chu, Weian Mao, Qixin Hu, Shaoteng Liu, Yuyang Zhao, Huizi Mao, Ying-Cong Chen, Enze Xie, Xiaojuan Qi, Song Han  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.18739v2.pdf)  
  Keywords: long video, autoregressive, denoising, interactive, efficient, video generation, architecture, diffusion model, benchmark, layout, distillation, streaming  
- **[Spectral Progressive Diffusion for Efficient Image and Video Generation](https://arxiv.org/abs/2605.18736v2)**  
  Authors: Howard Xiao, Brian Chao, Lior Yariv, Gordon Wetzstein  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.18736v2.pdf)  
  Keywords: autoregressive, denoising, efficient, acceleration, video generation, trajectory, diffusion model  
- **[Xiaomi EV World Model: A Joint World Model Integrating Reconstruction and Generation for Autonomous Driving](https://arxiv.org/abs/2605.18137v2)**  
  Authors: Lijun Zhou, Hongcheng Luo, Zhenxin Zhu, Cheng Chi, Mingfei Tu, Kaixin Xiong, Lei Gong, Zhanqian Wu, Zehan Zhang, Fangzhen Li, Hao Li, Yingying Shen, Jiale He, Haohui Zhu, Shan Zhao, Kai Wang, Zhiwei Zhan, Yuechuan Pu, Kaiyuan Tan, Ruiling Yang, Xianqi Wang, Tianyi Yan, Jiawei Zhou, Lei Zhang, Jingyang Zhao, Xi Zhou, Chitian Sun, Chenming Wu, Jiong Deng, Hongwei Xie, Ming Lu, Kun Ma, Long Chen, Guang Chen, Hangjun Ye, Bing Wang, Haiyang Sun  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.18137v2.pdf)  
  Keywords: denoising, simulation, world model, architecture, video generation, distillation, autonomous driving  
- **[SpecSem-Net: Integrating Spectral and Semantic Features for Robust AI-generated Video Detection](https://arxiv.org/abs/2605.17311v1)**  
  Authors: Zixi Wei, Huixuaun Zhang, Xiaojun Wan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.17311v1.pdf)  
  Keywords: denoising, benchmark, dit  
- **[3DPhysVideo: Consistency-Guided Flow SDE for Video Generation via 3D Scene Reconstruction and Physical Simulation](https://arxiv.org/abs/2605.16795v1)**  
  Authors: Hwidong Kim, Yunho Kim, Tae-Kyun Kim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.16795v1.pdf)  
  Keywords: dynamics, denoising, simulation, efficient, video generation, physical, evaluation, physical simulation, novel view, benchmark, physics, image-to-video, i2v, dit  
- **[AtlasVid: Efficient Ultra-High-Resolution Long Video Generation via Decoupled Global-Local Modeling](https://arxiv.org/abs/2605.16649v1)**  
  Authors: Ziyang Mai, Yuyao Zhang, Yu-Wing Tai  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.16649v1.pdf)  
  Keywords: long video, video diffusion, autoregressive, denoising, efficient, video generation, video synthesis, diffusion model  
- **[Video Models Can Reason with Verifiable Rewards](https://arxiv.org/abs/2605.15458v1)**  
  Authors: Tinghui Zhu, Sheng Zhang, James Y. Huang, Selena Song, Xiaofei Wen, Yuankai Li, Hoifung Poon, Muhao Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.15458v1.pdf)  
  Keywords: video diffusion, denoising, efficient, video generation, diffusion model, benchmark  

### World Models & Simulation

*Showing the latest 50 out of 118 papers*

- **[iTryOn: Mastering Interactive Video Virtual Try-On with Spatial-Semantic Guidance](https://arxiv.org/abs/2605.21431v1)**  
  Authors: Jun Zheng, Zhengze Xu, Mengting Chen, Jing Wang, Jinsong Lan, Xiaoyong Zhu, Kaifu Zhang, Bo Zheng, Xiaodan Liang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.21431v1.pdf)  
  Keywords: dynamics, video diffusion, interactive, diffusion transformer, benchmark, virtual try-on, temporal consistency, dit, controllable  
- **[Q-ARVD: Quantizing Autoregressive Video Diffusion Models](https://arxiv.org/abs/2605.21072v1)**  
  Authors: Siao Tang, Xinyin Ma, Gongfan Fang, Xingyi Yang, Xinchao Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.21072v1.pdf)  
  Keywords: autoregressive, video diffusion, interactive, video generation, world model, architecture, diffusion model, streaming, diffusion transformer  
- **[VSCD: Video-based Scene Change Detection in Unaligned Scenes](https://arxiv.org/abs/2605.20821v1)**  
  Authors: Jiae Yoon, Ue-Hwan Kim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20821v1.pdf)  
  Keywords: simulation, benchmark  
- **[Aero-World: Action-Conditioned Aerial Video Generation from Inertial Controls](https://arxiv.org/abs/2605.19728v1)**  
  Authors: Abdul Mohaimen Al Radi, Kunyang Li, Yuzhang Shang, Mubarak Shah, Yu Tian  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.19728v1.pdf)  
  Keywords: video diffusion, simulation, action-conditioned, acceleration, video generation, physical, evaluation, trajectory, diffusion model, benchmark, physics, image-to-video, controllable, dit, diffusion transformer  
- **[TelePhysics: Physics-Grounded Multi-Object Scene Generation from a Single Image with Real-Time Interaction](https://arxiv.org/abs/2605.20290v1)**  
  Authors: Xin Zhang, Yabo Chen, Yijie Fang, Wanying Qu, Haibin Huang, Chi Zhang, Feng Xu, Xuelong Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20290v1.pdf) | [![GitHub](https://img.shields.io/github/stars/xinzhang007/TelePhysics?style=social)](https://github.com/xinzhang007/TelePhysics)  
  Keywords: simulation, interactive, video generation, physical, video synthesis, physics, controllable  
- **[SWEET: Sparse World Modeling with Image Editing for Embodied Task Execution](https://arxiv.org/abs/2605.19319v1)**  
  Authors: Yiren Song, Yihan Wang, Xiyao Deng, Zhuoran Yan, Mike Zheng Shou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.19319v1.pdf)  
  Keywords: world model, dit, video generation  
- **[PhyWorld: Physics-Faithful World Model for Video Generation](https://arxiv.org/abs/2605.19242v1)**  
  Authors: Pu Zhao, Juyi Lin, Timothy Rupprecht, Arash Akbari, Chence Yang, Rahul Chowdhury, Elaheh Motamedi, Arman Akbari, Yumei He, Chen Wang, Geng Yuan, Weiwei Chen, Yanzhi Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.19242v1.pdf)  
  Keywords: dynamics, world model, video generation, physical, benchmark, world simulator, physics, video-to-video, flow matching, dit  
- **[WorldString: Actionable World Representation](https://arxiv.org/abs/2605.18743v2)**  
  Authors: Kunqi Xu, Jitao Li, Jianglong Ye, Tianshu Tang, Isabella Liu, Sifei Liu, Xueyan Zou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.18743v2.pdf)  
  Keywords: dynamics, world model, architecture, physical, video generation  
- **[LongLive-2.0: An NVFP4 Parallel Infrastructure for Long Video Generation](https://arxiv.org/abs/2605.18739v2)**  
  Authors: Yukang Chen, Luozhou Wang, Wei Huang, Shuai Yang, Bohan Zhang, Yicheng Xiao, Ruihang Chu, Weian Mao, Qixin Hu, Shaoteng Liu, Yuyang Zhao, Huizi Mao, Ying-Cong Chen, Enze Xie, Xiaojuan Qi, Song Han  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.18739v2.pdf)  
  Keywords: long video, autoregressive, denoising, interactive, efficient, video generation, architecture, diffusion model, benchmark, layout, distillation, streaming  
- **[EgoInteract: Synthetic Egocentric Videos Generation for Interaction Understanding and Anticipation](https://arxiv.org/abs/2605.18214v1)**  
  Authors: Rosario Leonardi, Francesco Ragusa, Daniele Materia, Alessandro Passanisi, James Fort, Jakob Engel, Giovanni Maria Farinella  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.18214v1.pdf)  
  Keywords: dynamics, simulation, video generation, benchmark, controllable  



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
