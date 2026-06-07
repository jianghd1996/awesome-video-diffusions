# Awesome Video Diffusions [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of latest research papers, projects and resources related to Video Diffusion Models and Video Generation. Content is automatically updated daily.

> Last Update: 2026-06-07 03:58:19

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
- [Architecture & Efficiency](#architecture-&-efficiency) (358 papers) - Architectural innovations (DiT, UNet), flow matching, and training/inference efficiency
- [Audio & Multi-modal](#audio-&-multi-modal) (32 papers) - Audio-driven and multi-modal conditioned video generation
- [Controllable Generation](#controllable-generation) (129 papers) - Controllable video generation with motion, camera, pose, or layout guidance
- [Human & Character Animation](#human-&-character-animation) (24 papers) - Human-centric video generation including talking heads, dance, and character animation
- [Image-to-Video Generation](#image-to-video-generation) (42 papers) - Methods for animating still images into videos
- [Long Video Generation](#long-video-generation) (133 papers) - Generating temporally consistent long-form videos beyond short clips
- [Personalization & Customization](#personalization-&-customization) (83 papers) - Personalized video generation with custom subjects, identities, or styles
- [Physical Understanding](#physical-understanding) (149 papers) - Physics-aware video generation and dynamics modeling
- [Surveys & Benchmarks](#surveys-&-benchmarks) (232 papers) - Survey papers, benchmarks, and evaluation metrics for video generation
- [Text-to-Video Generation](#text-to-video-generation) (53 papers) - Foundation models and methods for generating videos from text prompts
- [Video Editing](#video-editing) (31 papers) - Diffusion-based video editing, style transfer, and manipulation
- [Video Inpainting & Completion](#video-inpainting-&-completion) (12 papers) - Video inpainting, completion, outpainting, and temporal prediction
- [Video Super-Resolution & Enhancement](#video-super-resolution-&-enhancement) (72 papers) - Video quality improvement, upscaling, restoration, and frame interpolation
- [World Models & Simulation](#world-models-&-simulation) (123 papers) - Video generation as world simulators and interactive environment generation



## Table of Contents

- [Categorized Papers](#categorized-papers)
- [Classic Papers](#classic-papers)
- [Open Source Projects](#open-source-projects)
- [Applications](#applications)
- [Tutorials & Blogs](#tutorials--blogs)





## Categorized Papers

### 3D-aware Video Generation

- **[PointAction: 3D Points as Universal Action Representations for Robot Control](https://arxiv.org/abs/2606.03943v1)**  
  Authors: Mutian Tong, Han Jiang, Qiao Feng, Lingjie Liu, Jiatao Gu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.03943v1.pdf)  
  Keywords: diffusion model, dynamics, video prediction, 4d generation, video diffusion, video generation, simulation  
- **[RoboDream: Compositional World Models for Scalable Robot Data Synthesis](https://arxiv.org/abs/2606.02577v1)**  
  Authors: Junjie Ye, Rong Xue, Basile Van Hoorick, Runhao Li, Harshitha Rajaprakash, Pavel Tokmakov, Muhammad Zubair Irshad, Vitor Guizilini, Yue Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.02577v1.pdf)  
  Keywords: trajectory, diffusion model, dit, world model, video diffusion, physical, novel view  
- **[Towards 3D-Aware Video Diffusion Models: Render-Free Human Motion Control with Mesh Tokenization](https://arxiv.org/abs/2606.02000v1)**  
  Authors: Jingyun Liang, Min Wei, Shikai Li, Yizeng Han, Hangjie Yuan, Lei Sun, Weihua Chen, Fan Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.02000v1.pdf)  
  Keywords: trajectory, diffusion model, benchmark, dit, motion control, 3d-aware, architecture, human motion, video diffusion, video generation  
- **[Effective Multi-sensor Conditioning for Street-view Novel-view Synthesis](https://arxiv.org/abs/2606.01590v1)**  
  Authors: Zhengfei Kuang, Adam Sun, Liyuan Zhu, Tong Wu, Shengqu Cai, Jonathan Tremblay, Iro Armeni, Ehsan Adeli, Lior Yariv, Gordon Wetzstein  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.01590v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://streetnvs.github.io)  
  Keywords: trajectory, diffusion model, dit, video diffusion, novel view  
- **[Real2SAM2Real: Generative 3D Caches as Complementary Context for Video Diffusion](https://arxiv.org/abs/2606.00299v1)**  
  Authors: Jiayi Wu, Haoming Cai, Cornelia Fermuller, Christopher Metzler, Yiannis Aloimonos  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.00299v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://jiayi-wu-leo.github.io/real2sam2real)  
  Keywords: diffusion model, dynamics, dit, temporal consistency, 3d-aware, video diffusion  
- **[Robust Dreamer: Deviation-Aware Latent Gaussian Memory for Action-Controlled AR Video Generation](https://arxiv.org/abs/2605.30855v2)**  
  Authors: Hanlin Chen, Jiaxin Wei, Xibin Song, Yifu Wang, Steve Wang, Hongdong Li, Pan Ji, Gim Hee Lee  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30855v2.pdf)  
  Keywords: dit, autoregressive, image-to-video, 3d-aware, denoising, interactive, video generation, simulation  
- **[Full-4D: Generating Full-Scope 4D Scenes from a Single-View Video](https://arxiv.org/abs/2605.25500v1)**  
  Authors: Tingxi Chen, Ke Hao, Yabo Chen, Zhengxue Cheng, Rong Xie, Li Song, Haibin Huang, Chi Zhang, Xuelong Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25500v1.pdf)  
  Keywords: diffusion model, dit, multi-view video, distillation, flow matching, 4d generation, video interpolation, interactive, video diffusion, video synthesis, physical  
- **[Pantheon360: Taming Digital Twin Generation via 3D-Aware 360° Video Diffusion](https://arxiv.org/abs/2605.25449v1)**  
  Authors: Ting-Hsuan Chen, Ying-Huan Chen, Tao Tu, Jie-Ying Lee, Cho-Ying Wu, Fangzhou Lin, Hengyuan Zhang, David Paz, Xinyu Huang, Yuliang Guo, Yu-Lun Liu, Yue Wang, Liu Ren  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25449v1.pdf)  
  Keywords: trajectory, diffusion model, controllable, camera control, temporal consistency, 3d-aware, video diffusion, video generation, simulation  
- **[SRUG: Shadow-Guided Relightable Urban Scene with Generation Model](https://arxiv.org/abs/2605.24700v3)**  
  Authors: Yonghao Zhao, Zexin Yin, Jian Yang, Beibei Wang, Jin Xie  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.24700v3.pdf)  
  Keywords: evaluation, dit, physical, novel view  
- **[3DPhysVideo: Consistency-Guided Flow SDE for Video Generation via 3D Scene Reconstruction and Physical Simulation](https://arxiv.org/abs/2605.16795v1)**  
  Authors: Hwidong Kim, Yunho Kim, Tae-Kyun Kim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.16795v1.pdf)  
  Keywords: evaluation, benchmark, dynamics, dit, i2v, image-to-video, physical simulation, denoising, novel view, physics, efficient, physical, video generation, simulation  

### Applications

*Showing the latest 50 out of 55 papers*

- **[LongSpace: Exploring Long-Horizon Spatial Memory from Perception to Recall in Video](https://arxiv.org/abs/2606.05677v1)**  
  Authors: Shiqiang Lang, Jing Liu, Haoyang He, Peiwen Sun, Yuanteng Chen, Tao Liu, Lan Yang, Longteng Guo, Honggang Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.05677v1.pdf)  
  Keywords: autonomous driving, benchmark, layout, long video  
- **[Auteur: Language-Driven Cinematographic Framing for Human-Centric Video Generation](https://arxiv.org/abs/2606.01900v1)**  
  Authors: Muhammed Burak Kizil, Enes Sanli, Niloy J. Mitra, Xuelin Chen, Erkut Erdem, Aykut Erdem, Duygu Ceylan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.01900v1.pdf)  
  Keywords: camera control, film, video generation, human motion  
- **[PAI-Studio: Cinematic Video Background Replacement with Camera-Aware Motion](https://arxiv.org/abs/2606.01399v1)**  
  Authors: Heyuan Gao, Bangxun Tang, Yiren Song, Guian Fang, Zijian He, Jie Yang, Mike Zheng Shou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.01399v1.pdf)  
  Keywords: evaluation, dynamics, dit, identity, film, architecture, video synthesis, diffusion transformer  
- **[AlbedoEdit: Unified Instance-Level Video Editing with Albedo Guidance](https://arxiv.org/abs/2606.01362v1)**  
  Authors: Xilong Zhou, Bao-Huy Nguyen, Zheng Zeng, Jacob Munkberg, Jon Hasselgren, Thomas Leimkühler, Nima Kalantari, Miloš Hašan, Christian Theobalt  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.01362v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://vcai.mpi-inf.mpg.de/projects/AlbedoEdit)  
  Keywords: creative, dit, video editing  
- **[SKIP: Sparse Keyframe Interpolation Paradigm for Efficient Embodied World Models](https://arxiv.org/abs/2606.00664v1)**  
  Authors: Ziheng He, Yixiang Chen, Ning Yang, Zhanqian Wu, Qisen Ma, Yuan Xu, Jiabing Yang, Peiyan Li, Xiangnan Wu, Xiaofeng Wang, Zheng Zhu, Jing Liu, Nianfeng Liu, Yan Huang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.00664v1.pdf)  
  Keywords: diffusion model, dit, frame interpolation, action-conditioned, robotics, world model, video diffusion, efficient, simulation  
- **[Foundation VAEs for 3D CT Reconstruction, Augmentation, and Generation](https://arxiv.org/abs/2605.30893v1)**  
  Authors: Qi Chen, Shuhan Ding, Yu Gu, Nan Liu, Jiang Bian, Alan Yuille, Zongwei Zhou, Jingjing Fu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30893v1.pdf) | [![GitHub](https://img.shields.io/github/stars/qic999/Foundation-VAE?style=social)](https://github.com/qic999/Foundation-VAE)  
  Keywords: medical, diffusion model, dit  
- **[World Models: A Comprehensive Survey of Architectures, Methodologies, Reasoning Paradigms, and Applications](https://arxiv.org/abs/2606.00133v1)**  
  Authors: Arif Hassan Zidan, Yi Pan, Hanqi Jiang, Ruiyu Yan, Wei Ruan, Zihao Wu, Lifeng Chen, Weihang You, Xinliang Li, Bowen Chen, Huawen Hu, Peilong Wang, Sizhuang Liu, Jing Zhang, Siyuan Li, Zhengliang Liu, Yu Bao, Lin Zhao, Lichao Sun, Dajiang Zhu, Xiang Li, Jinglei Lv, Quanzheng Li, Wei Liu, Tianming Liu, Wei Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.00133v1.pdf)  
  Keywords: evaluation, benchmark, dynamics, autonomous driving, education, video prediction, medical, robotics, world model, architecture, interactive, survey, physics, video generation  
- **[DriveWAM: Video Generative Priors Enable Scalable World-Action Modeling for Autonomous Driving](https://arxiv.org/abs/2605.28544v1)**  
  Authors: Chen Shi, Jinrui Xu, Shaoshuai Shi, Kehua Sheng, Bo Zhang, Li Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28544v1.pdf)  
  Keywords: benchmark, dynamics, autonomous driving, autoregressive, physical, architecture, video diffusion, diffusion transformer  
- **[Turning Video Models into Generalist Robot Policies](https://arxiv.org/abs/2605.27817v1)**  
  Authors: Sizhe Lester Li, Evan Kim, Xingjian Bai, Tong Zhao, Tao Pang, Max Simchowitz, Vincent Sitzmann  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.27817v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://vera.csail.mit.edu)  
  Keywords: benchmark, dynamics, robotics, world model, efficient  
- **[AnyScene: Towards Highly Controllable Driving Scene Generation at Anywhere and Beyond](https://arxiv.org/abs/2605.26113v1)**  
  Authors: Haiming Zhang, Junfei Zhou, Feng Jiang, Jingzhong Li, Zhenglong Guo, Penglin Dai, Jifeng Dai, Yan Xie, Benjin Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.26113v1.pdf)  
  Keywords: layout, controllable, dit, autonomous driving, autoregressive, video synthesis, diffusion transformer, video generation, simulation  

### Architecture & Efficiency

*Showing the latest 50 out of 358 papers*

- **[RhymeFlow: Training-Free Acceleration for Video Generation with Asynchronous Denoising Flow Scheduling](https://arxiv.org/abs/2606.06309v1)**  
  Authors: Chensheng Dai, Shengjun Zhang, Yifan Li, Zhang Zhang, Zheng Zhu, Yueqi Duan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.06309v1.pdf)  
  Keywords: trajectory, dit, denoising, acceleration, video synthesis, diffusion transformer, video generation  
- **[LoomVideo: Unifying Multimodal Inputs into Video Generation and Editing](https://arxiv.org/abs/2606.06042v1)**  
  Authors: Jianzong Wu, Hao Lian, Jiongfan Yang, Dachao Hao, Ye Tian, Yunhai Tong, Jingyuan Zhu, Biaolong Chen, Qiaosong Qi, Aixi Zhang, Wanggui He, Mushui Liu, Jinlong Liu, Hao Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.06042v1.pdf)  
  Keywords: benchmark, dit, architecture, acceleration, efficient, diffusion transformer, video generation, video editing  
- **[V2V-Bench: A Comprehensive Benchmark for Video-to-Video Generation Evaluation](https://arxiv.org/abs/2606.05665v1)**  
  Authors: Tao Liu, Leela Krishna, Gouti Pavan Kumar, Sreeja K, Vishav Garg  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.05665v1.pdf)  
  Keywords: evaluation, benchmark, dit, i2v, t2v, video generation, video-to-video  
- **[Do Models Share Safety Representations? Cross-Model Steering for Safe Visual Generation](https://arxiv.org/abs/2606.05290v1)**  
  Authors: Tobia Poppi, Silvia Cappelletti, Sara Sarto, Florian Schiffers, Garin Kessler, Marcella Cornia, Lorenzo Baraldi, Rita Cucchiara  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.05290v1.pdf)  
  Keywords: text-to-video, architecture, video generation  
- **[Controllable Dynamic 3D Shape Generation via 3D Trajectories and Text](https://arxiv.org/abs/2606.05162v1)**  
  Authors: Jaeyeong Kim, Ines Kim, Jahyeok Koo, Seungryong Kim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.05162v1.pdf)  
  Keywords: evaluation, trajectory, controllable, dit, video generation  
- **[Echo-Infinity: Learning Evolving Memory for Real-Time Infinite Video Generation](https://arxiv.org/abs/2606.04527v1)**  
  Authors: Yuxuan Bian, Zeyue Xue, Songchun Zhang, Shiyi Zhang, Weiyang Jin, Yaowei Li, Junhao Zhuang, Haoran Li, Jie Huang, Haoyang Huang, Nan Duan, Qiang Xu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.04527v1.pdf)  
  Keywords: dit, autoregressive, video diffusion, diffusion transformer, video generation  
- **[DSA: Dynamic Step Allocation for Fast Autoregressive Video Generation](https://arxiv.org/abs/2606.04432v1)**  
  Authors: Thanh-Tung Le, Yunhan Zhao, Menglei Chai, Zhengyang Shen, Zhe Cao, Danhang Tang, Xiaohui Xie, Deying Kong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.04432v1.pdf)  
  Keywords: diffusion model, dit, autoregressive, denoising, distillation, interactive, video diffusion, diffusion transformer, video generation  
- **[Building The Ph(ysical)AI Layer Of Machine Intelligence](https://arxiv.org/abs/2606.04106v1)**  
  Authors: Ulbert Jose Botero, Liam Smith, Brooks Olney, Pooya Khorrami, Steven Kusiak, Watson Jia, Sage Trudeau, Daniel Capecci  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.04106v1.pdf)  
  Keywords: physics, architecture, efficient, physical  
- **[AAD-1: Asymmetric Adversarial Distillation for One-Step Autoregressive Video Generation](https://arxiv.org/abs/2606.03972v2)**  
  Authors: Haobo Li, Yanhong Zeng, Yunhong Lu, Jiapeng Zhu, Hao Ouyang, Qiuyu Wang, Ka Leong Cheng, Yujun Shen, Zhipeng Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.03972v2.pdf)  
  Keywords: autoregressive, image-to-video, distillation, architecture, video generation  
- **[Video-Mirai: Autoregressive Video Diffusion Models Need Foresight](https://arxiv.org/abs/2606.03971v1)**  
  Authors: Yonghao Yu, Lang Huang, Runyi Li, Zerun Wang, Toshihiko Yamasaki  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.03971v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://y0uroy.github.io/Video-Mirai)  
  Keywords: diffusion model, layout, dit, autoregressive, identity, architecture, streaming, video diffusion  

### Audio & Multi-modal

- **[Mamba-Enhanced Implicit Motion Learning for Audio-Driven Portrait Animation](https://arxiv.org/abs/2606.03402v2)**  
  Authors: Xuan Wei, Jiahui Chen, Kaiheng Li, Mingyu Shao, Qingqi Hong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.03402v2.pdf)  
  Keywords: diffusion model, benchmark, dynamics, audio-driven, human animation, gesture, architecture, human motion, video generation  
- **[Inference-Time Scaling for Joint Audio-Video Generation](https://arxiv.org/abs/2606.03183v1)**  
  Authors: Jaemin Jung, Kyeongha Rho, Inkyu Shin, Joon Son Chung  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.03183v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://jung-jaemin.github.io/ITS-AVGen-Proj)  
  Keywords: benchmark, video generation, sound  
- **[Cohort-Scale Neural Atlases of Ultrasound Video](https://arxiv.org/abs/2606.00890v1)**  
  Authors: Zhuorui Zhang, Roger Pallarès-López, Xuan Wu, Praneeth Namburi, Brian W. Anthony  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.00890v1.pdf)  
  Keywords: sound  
- **[LongCat-Video-Avatar 1.5 Technical Report](https://arxiv.org/abs/2605.26486v1)**  
  Authors: Meituan LongCat Team, Xunliang Cai, Meng Cheng, Feng Gao, Zhe Kong, Jiamu Li, Le Li, Weiheng Li, Hongyu Liu, Shuai Tan, Xiaoming Wei, Tianyu Yang, Yong Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.26486v1.pdf)  
  Keywords: evaluation, benchmark, avatar, dit, audio-driven, distillation, identity, video generation  
- **[StreamChar: Long-Horizon Streaming Character Audio-Video Generation with Decoupled Orchestration](https://arxiv.org/abs/2605.25659v1)**  
  Authors: Linrui Tian, Qi Wang, Bang Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25659v1.pdf)  
  Keywords: dit, audio-driven, autoregressive, denoising, distillation, identity, streaming, efficient, video generation  
- **[Test-Time Self-Adaptive Conditioning for Stable Audio-Driven Talking-Head Generation](https://arxiv.org/abs/2605.25488v1)**  
  Authors: Zhicheng Zhang, Lei Wang, Yu Zhang, Yongsheng Gao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25488v1.pdf)  
  Keywords: benchmark, dynamics, dit, audio-driven, identity, video generation  
- **[AVBench: Human-Aligned and Automated Evaluation Benchmark for Audio-Video Generative Models](https://arxiv.org/abs/2605.24652v1)**  
  Authors: Jialiang Yang, Bin Xia, Ruihang Chu, Dingdong Wang, Wanke Xia, Zhun Mou, Tianyang Zhong, Yiting Zhao, Wenming Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.24652v1.pdf)  
  Keywords: evaluation, benchmark, dit, style, sound  
- **[What Semantics Survive the Connector? Diagnosing VLM-to-DiT Alignment in Video Editing](https://arxiv.org/abs/2605.20795v1)**  
  Authors: Hangyu Lin, Chao Wen, Chengming Xu, Jianxiong Gao, Jiangning Zhang, Xiaobin Hu, Yanwei Fu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20795v1.pdf)  
  Keywords: evaluation, dit, flow matching, architecture, multi-modal, video editing  
- **[Sound Sparks Motion: Audio and Text Tuning for Video Editing](https://arxiv.org/abs/2605.15307v1)**  
  Authors: AmirHossein Naghi Razlighi, Aryan Mikaeili, Ali Mahdavi-Amiri, Daniel Cohen-Or, Yiorgos Chrysanthou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.15307v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://amirhossein-razlighi.github.io/Sound_Sparks_Motion)  
  Keywords: dit, motion control, sound, video generation, video editing  
- **[OmniNFT: Modality-wise Omni Diffusion Reinforcement for Joint Audio-Video Generation](https://arxiv.org/abs/2605.12480v1)**  
  Authors: Guohui Zhang, XiaoXiao Ma, Jie Huang, Hang Xu, Hu Yu, Siming Fu, Yuming Li, Zeyue Xue, Lin Song, Haoyang Huang, Nan Duan, Feng Zhao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.12480v1.pdf)  
  Keywords: multi-modal, efficient, video generation, dit  

### Controllable Generation

*Showing the latest 50 out of 129 papers*

- **[Physics in 2-Steps: Locking Motion Priors Before Visual Refinement Erases Them](https://arxiv.org/abs/2606.06361v1)**  
  Authors: Woojung Han, Seil Kang, Youngjun Jun, Min-Hung Chen, Fu-En Yang, Seong Jae Hwang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.06361v1.pdf)  
  Keywords: trajectory, diffusion model, image-to-video, denoising, video diffusion, physics, physical  
- **[RhymeFlow: Training-Free Acceleration for Video Generation with Asynchronous Denoising Flow Scheduling](https://arxiv.org/abs/2606.06309v1)**  
  Authors: Chensheng Dai, Shengjun Zhang, Yifan Li, Zhang Zhang, Zheng Zhu, Yueqi Duan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.06309v1.pdf)  
  Keywords: trajectory, dit, denoising, acceleration, video synthesis, diffusion transformer, video generation  
- **[ReCache: Learning Budget-Aware Caching Schedules for Diffusion Models via REINFORCE](https://arxiv.org/abs/2606.06060v1)**  
  Authors: Mishan Aliev, Eva Neudachina, Ilya Bykov, Aleksandr Oganov, Kirill Struminsky, Aibek Alanov, Denis Rakitin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.06060v1.pdf) | [![GitHub](https://img.shields.io/github/stars/thecrazymage/ReCache?style=social)](https://github.com/thecrazymage/ReCache)  
  Keywords: trajectory, diffusion model, controllable, denoising  
- **[Resonant Minds: Closed-Loop Social Avatars with Theory of Mind](https://arxiv.org/abs/2606.05896v1)**  
  Authors: Jianxu Shangguan, Jing Xu, Hang Ye, Xiaoxuan Ma, Yizhou Wang, Wentao Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.05896v1.pdf)  
  Keywords: evaluation, dynamics, avatar, controllable, talking head, video generation  
- **[LongSpace: Exploring Long-Horizon Spatial Memory from Perception to Recall in Video](https://arxiv.org/abs/2606.05677v1)**  
  Authors: Shiqiang Lang, Jing Liu, Haoyang He, Peiwen Sun, Yuanteng Chen, Tao Liu, Lan Yang, Longteng Guo, Honggang Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.05677v1.pdf)  
  Keywords: autonomous driving, benchmark, layout, long video  
- **[Controllable Dynamic 3D Shape Generation via 3D Trajectories and Text](https://arxiv.org/abs/2606.05162v1)**  
  Authors: Jaeyeong Kim, Ines Kim, Jahyeok Koo, Seungryong Kim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.05162v1.pdf)  
  Keywords: evaluation, trajectory, controllable, dit, video generation  
- **[Dream.exe: Can Video Generation Models Dream Executable Robot Manipulation?](https://arxiv.org/abs/2606.04811v2)**  
  Authors: Rui Zhao, Kaiming Yang, Jifeng Zhu, Siyang Chen, Ziqi Wang, Weijia Wu, Kevin Qinghong Lin, Heng Wang, Mike Zheng Shou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.04811v2.pdf) | [![GitHub](https://img.shields.io/github/stars/showlab/Dream.exe?style=social)](https://github.com/showlab/Dream.exe)  
  Keywords: evaluation, trajectory, benchmark, physics, physical, video generation  
- **[Video-Mirai: Autoregressive Video Diffusion Models Need Foresight](https://arxiv.org/abs/2606.03971v1)**  
  Authors: Yonghao Yu, Lang Huang, Runyi Li, Zerun Wang, Toshihiko Yamasaki  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.03971v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://y0uroy.github.io/Video-Mirai)  
  Keywords: diffusion model, layout, dit, autoregressive, identity, architecture, streaming, video diffusion  
- **[RoboDream: Compositional World Models for Scalable Robot Data Synthesis](https://arxiv.org/abs/2606.02577v1)**  
  Authors: Junjie Ye, Rong Xue, Basile Van Hoorick, Runhao Li, Harshitha Rajaprakash, Pavel Tokmakov, Muhammad Zubair Irshad, Vitor Guizilini, Yue Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.02577v1.pdf)  
  Keywords: trajectory, diffusion model, dit, world model, video diffusion, physical, novel view  
- **[From Zero to Hero: Training-Free Custom Concept Spawning in World Models](https://arxiv.org/abs/2606.02575v1)**  
  Authors: Kiymet Akdemir, Pinar Yanardag  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.02575v1.pdf)  
  Keywords: controllable, dit, autoregressive, image-to-video, identity, world model, interactive, concept, video generation, simulation  

### Human & Character Animation

- **[Resonant Minds: Closed-Loop Social Avatars with Theory of Mind](https://arxiv.org/abs/2606.05896v1)**  
  Authors: Jianxu Shangguan, Jing Xu, Hang Ye, Xiaoxuan Ma, Yizhou Wang, Wentao Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.05896v1.pdf)  
  Keywords: evaluation, dynamics, avatar, controllable, talking head, video generation  
- **[Mamba-Enhanced Implicit Motion Learning for Audio-Driven Portrait Animation](https://arxiv.org/abs/2606.03402v2)**  
  Authors: Xuan Wei, Jiahui Chen, Kaiheng Li, Mingyu Shao, Qingqi Hong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.03402v2.pdf)  
  Keywords: diffusion model, benchmark, dynamics, audio-driven, human animation, gesture, architecture, human motion, video generation  
- **[Towards 3D-Aware Video Diffusion Models: Render-Free Human Motion Control with Mesh Tokenization](https://arxiv.org/abs/2606.02000v1)**  
  Authors: Jingyun Liang, Min Wei, Shikai Li, Yizeng Han, Hangjie Yuan, Lei Sun, Weihua Chen, Fan Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.02000v1.pdf)  
  Keywords: trajectory, diffusion model, benchmark, dit, motion control, 3d-aware, architecture, human motion, video diffusion, video generation  
- **[Auteur: Language-Driven Cinematographic Framing for Human-Centric Video Generation](https://arxiv.org/abs/2606.01900v1)**  
  Authors: Muhammed Burak Kizil, Enes Sanli, Niloy J. Mitra, Xuelin Chen, Erkut Erdem, Aykut Erdem, Duygu Ceylan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.01900v1.pdf)  
  Keywords: camera control, film, video generation, human motion  
- **[Archon: A Unified Multimodal Model for Holistic Digital Human Generation](https://arxiv.org/abs/2605.30311v1)**  
  Authors: Chong Bao, Shichen Liu, Lijun Yu, David Futschik, Stylianos Moschoglou, Shefali Srivastava, Ziqian Bai, Feitong Tan, Guofeng Zhang, Zhaopeng Cui, Sean Fanello, Yinda Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30311v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://zju3dv.github.io/archon)  
  Keywords: dynamics, avatar, autoregressive, video diffusion, efficient  
- **[LongCat-Video-Avatar 1.5 Technical Report](https://arxiv.org/abs/2605.26486v1)**  
  Authors: Meituan LongCat Team, Xunliang Cai, Meng Cheng, Feng Gao, Zhe Kong, Jiamu Li, Le Li, Weiheng Li, Hongyu Liu, Shuai Tan, Xiaoming Wei, Tianyu Yang, Yong Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.26486v1.pdf)  
  Keywords: evaluation, benchmark, avatar, dit, audio-driven, distillation, identity, video generation  
- **[RoMo: A Large-Scale, Richly Organized Dataset and Semantic Taxonomy for Human Motion Generation](https://arxiv.org/abs/2605.26241v1)**  
  Authors: Jiahao Zhang, Joseph Liu, Young-Yoon Lee, Seonghyeon Moon, Victor Zordan, Guy Tevet, Karen Liu, Stephen Gould, Oren Jacob, Haomiao Jiang, Mubbasir Kapadia, Yizhak Ben-Shabat  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.26241v1.pdf)  
  Keywords: evaluation, human motion  
- **[iTryOn: Mastering Interactive Video Virtual Try-On with Spatial-Semantic Guidance](https://arxiv.org/abs/2605.21431v1)**  
  Authors: Jun Zheng, Zhengze Xu, Mengting Chen, Jing Wang, Jinsong Lan, Xiaoyong Zhu, Kaifu Zhang, Bo Zheng, Xiaodan Liang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.21431v1.pdf)  
  Keywords: benchmark, dynamics, controllable, dit, temporal consistency, virtual try-on, interactive, video diffusion, diffusion transformer  
- **[EverAnimate: Minute-Scale Human Animation via Latent Flow Restoration](https://arxiv.org/abs/2605.15042v1)**  
  Authors: Wuyang Li, Yang Gao, Mariam Hassan, Lan Feng, Wentao Pan, Po-Chien Luan, Alexandre Alahi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.15042v1.pdf)  
  Keywords: identity, long-form, flow matching, human animation, human motion, efficient, video generation  
- **[PhyMotion: Structured 3D Motion Reward for Physics-Grounded Human Video Generation](https://arxiv.org/abs/2605.14269v1)**  
  Authors: Yidong Huang, Zun Wang, Han Lin, Dong-Ki Kim, Shayegan Omidshafiei, Jaehong Yoon, Jaemin Cho, Yue Zhang, Mohit Bansal  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.14269v1.pdf)  
  Keywords: evaluation, dynamics, autoregressive, human motion, physics, physical, video generation  

### Image-to-Video Generation

- **[Physics in 2-Steps: Locking Motion Priors Before Visual Refinement Erases Them](https://arxiv.org/abs/2606.06361v1)**  
  Authors: Woojung Han, Seil Kang, Youngjun Jun, Min-Hung Chen, Fu-En Yang, Seong Jae Hwang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.06361v1.pdf)  
  Keywords: trajectory, diffusion model, image-to-video, denoising, video diffusion, physics, physical  
- **[V2V-Bench: A Comprehensive Benchmark for Video-to-Video Generation Evaluation](https://arxiv.org/abs/2606.05665v1)**  
  Authors: Tao Liu, Leela Krishna, Gouti Pavan Kumar, Sreeja K, Vishav Garg  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.05665v1.pdf)  
  Keywords: evaluation, benchmark, dit, i2v, t2v, video generation, video-to-video  
- **[AAD-1: Asymmetric Adversarial Distillation for One-Step Autoregressive Video Generation](https://arxiv.org/abs/2606.03972v2)**  
  Authors: Haobo Li, Yanhong Zeng, Yunhong Lu, Jiapeng Zhu, Hao Ouyang, Qiuyu Wang, Ka Leong Cheng, Yujun Shen, Zhipeng Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.03972v2.pdf)  
  Keywords: autoregressive, image-to-video, distillation, architecture, video generation  
- **[Cosmos 3: Omnimodal World Models for Physical AI](https://arxiv.org/abs/2606.02800v1)**  
  Authors: Aditi, Niket Agarwal, Arslan Ali, Jon Allen, Martin Antolini, Adeline Aubame, Alisson Azzolini, Junjie Bai, Maciej Bala, Yogesh Balaji, Josh Bapst, Aarti Basant, Mukesh Beladiya, Mohammad Qazim Bhat, Zaid Pervaiz Bhat, Dan Blick, Vanni Brighella, Han Cai, Tiffany Cai, Eric Cameracci, Jiaxin Cao, Yulong Cao, Mark Carlson, Carlos Casanova, Ting-Yun Chang, Yan Chang, Yu-Wei Chao, Prithvijit Chattopadhyay, Roshan Chaudhari, Chieh-Yun Chen, Junyu Chen, Ke Chen, Qizhi Chen, Wenkai Chen, Xiaotong Chen, Yu Chen, An-Chieh Cheng, Click Cheng, Xiu Chia, Jeana Choi, Chaeyeon Chung, Wenyan Cong, Yin Cui, Magdalena Dadela, Nalin Dadhich, Wenliang Dai, Joyjit Daw, Alperen Degirmenci, Rodrigo Vieira Del Monte, Robert Denomme, Sameer Dharur, Marco Di Lucca, Ke Ding, Wenhao Ding, Yifan Ding, Yuzhu Dong, Nicole Drumheller, Yilun Du, Aigul Dzhumamuratova, Aleksandr Efitorov, Hamid Eghbalzadeh, Naomi Eigbe, Imad El Hanafi, Hassan Eslami, Benedikt Falk, Jiaojiao Fan, Jim Fan, Amol Fasale, Sergiy Fefilatyev, Liang Feng, Francesco Ferroni, Sanja Fidler, Xiao Fu, Vikram Fugro, Prashant Gaikwad, TJ Galda, Katelyn Gao, Yihuai Gao, Wenhang Ge, Sreyan Ghosh, Arushi Goel, Vivek Goel, Akash Gokul, Rama Govindaraju, Jinwei Gu, Miguel Guerrero, Elfie Guo, Aryaman Gupta, Siddharth Gururani, Hugo Hadfield, Song Han, Ankur Handa, Zekun Hao, Mohammad Harrim, Ali Hassani, Nathan Hayes-Roth, Yufan He, Chris Helvig, Cyrus Hogg, Madison Huang, Michael Huang, Sophia Huang, Yufan Huang, Jacob Huffman, DeLesley Hutchins, Suneel Indupuru, Boris Ivanovic, Arihant Jain, Joel Jang, Ryan Ji, Yanan Jian, Dongfu Jiang, Jingyi Jin, Atharva Joshi, Nikhilesh Joshi, Pranjali Joshi, Jaehun Jung, Weiwei Kang, Scott Kassekert, Jan Kautz, Ashna Khetan, Julia Kiczka, Slawek Kierat, Gwanghyun Kim, Kuno Kim, Sunny Kim, Kezhi Kong, Xin Kong, Zhifeng Kong, Tomasz Kornuta, Egor Krivov, Hui Kuang, Saurav Kumar, Chia-Wen Kuo, George Kurian, Wojciech Kutak, JF Lafleche, Himangshu Lahkar, Omar Laymoun, Jayjun Lee, Sanggil Lee, Gabriele Leone, Boyi Li, Freya Li, Jiajun Li, Jinfeng Li, Ling Li, Pengcheng Li, Shangru Li, Tingle Li, Xiaolong Li, Xuan Li, Zhaoshuo Li, Zhiqi Li, Hao Liang, Maosheng Liao, Chen-Hsuan Lin, Tsung-Yi Lin, Ming-Yu Liu, Sifei Liu, Zihan Liu, Hai Loc Lu, Xiangyu Lu, Alice Luo, Ruipu Luo, Wenjie Luo, Jiangran Lyu, Martin Ding Ma, Nic Ma, Qianli Ma, Dawid Majchrowski, Louis Marcoux, Miguel Martin, Qing Miao, Ashkan Mirzaei, Shreyas Misra, Kaichun Mo, Durra Mohsin, Hyejin Moon, Pawel Morkisz, Saeid Motiian, Kirill Motkov, Seungjun Nah, Yashraj Narang, Deepak Narayanan, Thabang Ngazimbi, Julian Ouyang, David Page, Yatian Pang, Sehwi Park, Mahesh Patekar, Mostofa Patwary, Marco Pavone, Trung Pham, Wei Ping, Soha Pouya, Shrimai Prabhumoye, Varun Praveen, Delin Qu, Hesam Rabeti, Morteza Ramezanali, Marilyn Reeb, Xuanchi Ren, Kristen Rumley, Wojciech Rymer, Jun Saito, Yeongho Seol, John Shao, Piyush Shekdar, Tianwei Shen, Humphrey Shi, Min Shi, Stella Shi, Kevin Shih, Mohammad Shoeybi, Mateusz Sieniawski, Shuran Song, Alexander Sotelo, Amir Sotoodeh, Sunil Srinivasa, Vignesh Srinivasakumar, Bartosz Stefaniak, Rahul Heinrich Steiger, Shangkun Sun, Jiaxiang Tang, Shitao Tang, Yangyang Tang, Yue Tang, Tolou Tavakkoli, Kayley Ting, Krzysztof Tomala, Wei-Cheng Tseng, Jibin Varghese, Sergei Vasilev, Thomas Volk, Raju Wagwani, Roger Waleffe, Andrew Z. Wang, Boxiang Wang, Haoxiang Wang, Qiao Wang, Shihao Wang, Shijie Wang, Ting-Chun Wang, Yan Wang, Yu Wang, David Wehr, Fangyin Wei, Xinshuo Weng, Jay Zhangjie Wu, Kedi Wu, Hongchi Xia, Summer Xiao, Tianjun Xiao, Kevin Xie, Daguang Xu, Jiashu Xu, Mengyao Xu, Ruqing Xu, Xingqian Xu, Yao Xu, Dinghao Yang, Dong Yang, Hans Yang, Xiaodong Yang, Xuning Yang, Yichu Yang, Yurong You, Zhiding Yu, Hao Yuan, Simon Yuen, Xiaohui Zeng, Pengcuo Zeren, Cindy Zha, Haotian Zhang, Jenny Zhang, Jing Zhang, Liangkai Zhang, Paris Zhang, Shun Zhang, Xuanmeng Zhang, Zhizheng Zhang, Ann Zhao, Yilin Zhao, Yuliya Zhautouskaya, Charles Zhou, Fengzhe Zhou, Shilin Zhu, Yuke Zhu, Dima Zhylko, Artur Zolkowski  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.02800v1.pdf) | [![GitHub](https://img.shields.io/github/stars/nvidia/cosmos?style=social)](https://github.com/nvidia/cosmos) | [![Project](https://img.shields.io/badge/-Project-blue)](https://openmdw.ai/license/1-1) | [![HuggingFace](https://img.shields.io/badge/-HuggingFace-yellow)](https://huggingface.co/collections/nvidia/cosmos3)  
  Keywords: evaluation, benchmark, image-to-video, world model, architecture, world simulator, physical  
- **[From Zero to Hero: Training-Free Custom Concept Spawning in World Models](https://arxiv.org/abs/2606.02575v1)**  
  Authors: Kiymet Akdemir, Pinar Yanardag  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.02575v1.pdf)  
  Keywords: controllable, dit, autoregressive, image-to-video, identity, world model, interactive, concept, video generation, simulation  
- **[OptiWorld: Optimal Control for Video World Generation under Physical Constraints](https://arxiv.org/abs/2606.00499v1)**  
  Authors: Yu Yuan, Jianhao Yuan, Xijun Wang, Daiqing Li, Liu He, Lu Ling, Stanley H. Chan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.00499v1.pdf)  
  Keywords: trajectory, dynamics, dit, image-to-video, world model, efficient, physical, video generation  
- **[Robust Dreamer: Deviation-Aware Latent Gaussian Memory for Action-Controlled AR Video Generation](https://arxiv.org/abs/2605.30855v2)**  
  Authors: Hanlin Chen, Jiaxin Wei, Xibin Song, Yifu Wang, Steve Wang, Hongdong Li, Pan Ji, Gim Hee Lee  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30855v2.pdf)  
  Keywords: dit, autoregressive, image-to-video, 3d-aware, denoising, interactive, video generation, simulation  
- **[minWM: A Full-Stack Open-Source Framework for Real-Time Interactive Video World Models](https://arxiv.org/abs/2605.30263v1)**  
  Authors: Min Zhao, Hongzhou Zhu, Bokai Yan, Zihan Zhou, Yimin Chen, Wenqiang Sun, Kaiwen Zheng, Guande He, Xiao Yang, Chongxuan Li, Fan Bao, Jun Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30263v1.pdf) | [![GitHub](https://img.shields.io/github/stars/shengshu-ai/minWM?style=social)](https://github.com/shengshu-ai/minWM)  
  Keywords: trajectory, diffusion model, controllable, i2v, camera control, dit, autoregressive, t2v, distillation, world model, architecture, style, streaming, video diffusion, interactive, video generation  
- **[LiveSVG: Zero-Shot SVG Animation via Video Generation](https://arxiv.org/abs/2605.30174v1)**  
  Authors: Matan Levy, Ran Margolin, Bar Cavia, Dvir Samuel, Yael Pritch, Shmuel Peleg, Alex Rav Acha, Ariel Shamir, Dani Lischinski  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30174v1.pdf)  
  Keywords: evaluation, diffusion model, benchmark, dit, image-to-video, distillation, video diffusion, video generation  
- **[Proprio: Latent Self-Scoring and Inference-Time Refinement for Physically Plausible Video Generation](https://arxiv.org/abs/2605.28230v1)**  
  Authors: Mariam Hassan, Kaouther Messaoud, Wuyang Li, Alexandre Alahi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.28230v1.pdf)  
  Keywords: evaluation, benchmark, dynamics, image-to-video, video generation, physics, physical, text-to-video  

### Long Video Generation

*Showing the latest 50 out of 133 papers*

- **[LongSpace: Exploring Long-Horizon Spatial Memory from Perception to Recall in Video](https://arxiv.org/abs/2606.05677v1)**  
  Authors: Shiqiang Lang, Jing Liu, Haoyang He, Peiwen Sun, Yuanteng Chen, Tao Liu, Lan Yang, Longteng Guo, Honggang Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.05677v1.pdf)  
  Keywords: autonomous driving, benchmark, layout, long video  
- **[Echo-Infinity: Learning Evolving Memory for Real-Time Infinite Video Generation](https://arxiv.org/abs/2606.04527v1)**  
  Authors: Yuxuan Bian, Zeyue Xue, Songchun Zhang, Shiyi Zhang, Weiyang Jin, Yaowei Li, Junhao Zhuang, Haoran Li, Jie Huang, Haoyang Huang, Nan Duan, Qiang Xu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.04527v1.pdf)  
  Keywords: dit, autoregressive, video diffusion, diffusion transformer, video generation  
- **[DSA: Dynamic Step Allocation for Fast Autoregressive Video Generation](https://arxiv.org/abs/2606.04432v1)**  
  Authors: Thanh-Tung Le, Yunhan Zhao, Menglei Chai, Zhengyang Shen, Zhe Cao, Danhang Tang, Xiaohui Xie, Deying Kong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.04432v1.pdf)  
  Keywords: diffusion model, dit, autoregressive, denoising, distillation, interactive, video diffusion, diffusion transformer, video generation  
- **[AAD-1: Asymmetric Adversarial Distillation for One-Step Autoregressive Video Generation](https://arxiv.org/abs/2606.03972v2)**  
  Authors: Haobo Li, Yanhong Zeng, Yunhong Lu, Jiapeng Zhu, Hao Ouyang, Qiuyu Wang, Ka Leong Cheng, Yujun Shen, Zhipeng Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.03972v2.pdf)  
  Keywords: autoregressive, image-to-video, distillation, architecture, video generation  
- **[Video-Mirai: Autoregressive Video Diffusion Models Need Foresight](https://arxiv.org/abs/2606.03971v1)**  
  Authors: Yonghao Yu, Lang Huang, Runyi Li, Zerun Wang, Toshihiko Yamasaki  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.03971v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://y0uroy.github.io/Video-Mirai)  
  Keywords: diffusion model, layout, dit, autoregressive, identity, architecture, streaming, video diffusion  
- **[Pixel Cube: Diffusion-based Portrait Video Relighting Through Realistic Lighting Reproduction](https://arxiv.org/abs/2606.02919v2)**  
  Authors: Yufan Zhang, Yu Ji, Ayo Ajiboye, Rundi Wu, Yu Guo, Changxi Zheng, Jinwei Ye  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.02919v2.pdf)  
  Keywords: diffusion model, dit, temporal consistency, identity, video diffusion  
- **[From Zero to Hero: Training-Free Custom Concept Spawning in World Models](https://arxiv.org/abs/2606.02575v1)**  
  Authors: Kiymet Akdemir, Pinar Yanardag  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.02575v1.pdf)  
  Keywords: controllable, dit, autoregressive, image-to-video, identity, world model, interactive, concept, video generation, simulation  
- **[LongLive-RAG: A General Retrieval-Augmented Framework for Long Video Generation](https://arxiv.org/abs/2606.02553v1)**  
  Authors: Qixin Hu, Shuai Yang, Wei Huang, Song Han, Yukang Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.02553v1.pdf) | [![GitHub](https://img.shields.io/github/stars/qixinhu11/LongLive-RAG?style=social)](https://github.com/qixinhu11/LongLive-RAG)  
  Keywords: trajectory, dit, autoregressive, long video, identity, video diffusion, video generation  
- **[Retrieve What's Missing: Coverage-Maximizing Retrieval for Consistent Long Video Generation](https://arxiv.org/abs/2606.02479v1)**  
  Authors: Minseok Joo, Dogyun Park, Taehoon Lee, Kyujin Lee, Hyunwoo J. Kim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.02479v1.pdf)  
  Keywords: efficient, autoregressive, long video, video generation  
- **[Spatial-Temporal Decoupled Reference Conditioning for Identity-Preserving Text-to-Video Generation](https://arxiv.org/abs/2606.02441v1)**  
  Authors: Yuheng Chen, Teng Hu, Yuji Wang, Qingdong He, Lizhuang Ma, Jiangning Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.02441v1.pdf)  
  Keywords: layout, dit, temporal consistency, identity, video generation, text-to-video  

### Personalization & Customization

*Showing the latest 50 out of 83 papers*

- **[Activation Steering of Video Generation Models via Reduced-Order Linear Optimal Control](https://arxiv.org/abs/2606.04775v1)**  
  Authors: Jihoon Hong, Alice Chan, Qiyue Dai, Julian Skifstad, Glen Chou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.04775v1.pdf)  
  Keywords: benchmark, dynamics, t2v, video generation, concept, text-to-video  
- **[Video-Mirai: Autoregressive Video Diffusion Models Need Foresight](https://arxiv.org/abs/2606.03971v1)**  
  Authors: Yonghao Yu, Lang Huang, Runyi Li, Zerun Wang, Toshihiko Yamasaki  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.03971v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://y0uroy.github.io/Video-Mirai)  
  Keywords: diffusion model, layout, dit, autoregressive, identity, architecture, streaming, video diffusion  
- **[Pixel Cube: Diffusion-based Portrait Video Relighting Through Realistic Lighting Reproduction](https://arxiv.org/abs/2606.02919v2)**  
  Authors: Yufan Zhang, Yu Ji, Ayo Ajiboye, Rundi Wu, Yu Guo, Changxi Zheng, Jinwei Ye  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.02919v2.pdf)  
  Keywords: diffusion model, dit, temporal consistency, identity, video diffusion  
- **[From Zero to Hero: Training-Free Custom Concept Spawning in World Models](https://arxiv.org/abs/2606.02575v1)**  
  Authors: Kiymet Akdemir, Pinar Yanardag  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.02575v1.pdf)  
  Keywords: controllable, dit, autoregressive, image-to-video, identity, world model, interactive, concept, video generation, simulation  
- **[LongLive-RAG: A General Retrieval-Augmented Framework for Long Video Generation](https://arxiv.org/abs/2606.02553v1)**  
  Authors: Qixin Hu, Shuai Yang, Wei Huang, Song Han, Yukang Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.02553v1.pdf) | [![GitHub](https://img.shields.io/github/stars/qixinhu11/LongLive-RAG?style=social)](https://github.com/qixinhu11/LongLive-RAG)  
  Keywords: trajectory, dit, autoregressive, long video, identity, video diffusion, video generation  
- **[Spatial-Temporal Decoupled Reference Conditioning for Identity-Preserving Text-to-Video Generation](https://arxiv.org/abs/2606.02441v1)**  
  Authors: Yuheng Chen, Teng Hu, Yuji Wang, Qingdong He, Lizhuang Ma, Jiangning Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.02441v1.pdf)  
  Keywords: layout, dit, temporal consistency, identity, video generation, text-to-video  
- **[PAI-Studio: Cinematic Video Background Replacement with Camera-Aware Motion](https://arxiv.org/abs/2606.01399v1)**  
  Authors: Heyuan Gao, Bangxun Tang, Yiren Song, Guian Fang, Zijian He, Jie Yang, Mike Zheng Shou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.01399v1.pdf)  
  Keywords: evaluation, dynamics, dit, identity, film, architecture, video synthesis, diffusion transformer  
- **[Collaborative Few-Step Distillation and Low-Bit Quantization for Wan2.2 Dual-Expert Video Diffusion Models](https://arxiv.org/abs/2606.00658v1)**  
  Authors: Jinyang Du, Shenghao Jin, Ziqian Xu, Ruihao Gong, Shiqiao Gu, Yang Yong, Jinyang Guo, Xianglong Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.00658v1.pdf)  
  Keywords: trajectory, diffusion model, t2v, denoising, distillation, style, video diffusion  
- **[SlotMemory: Object-Centric KV Memory for Streaming Long-Video Generation](https://arxiv.org/abs/2605.31033v1)**  
  Authors: Weijia Dou, Hui Li, Jiahao Cui, Lei Zhou, Jingdong Wang, Siyu Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.31033v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://tj12323.github.io/SlotMemory)  
  Keywords: t2v, identity, long-form, streaming, video diffusion, interactive, video synthesis, video generation  
- **[minWM: A Full-Stack Open-Source Framework for Real-Time Interactive Video World Models](https://arxiv.org/abs/2605.30263v1)**  
  Authors: Min Zhao, Hongzhou Zhu, Bokai Yan, Zihan Zhou, Yimin Chen, Wenqiang Sun, Kaiwen Zheng, Guande He, Xiao Yang, Chongxuan Li, Fan Bao, Jun Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30263v1.pdf) | [![GitHub](https://img.shields.io/github/stars/shengshu-ai/minWM?style=social)](https://github.com/shengshu-ai/minWM)  
  Keywords: trajectory, diffusion model, controllable, i2v, camera control, dit, autoregressive, t2v, distillation, world model, architecture, style, streaming, video diffusion, interactive, video generation  

### Physical Understanding

*Showing the latest 50 out of 149 papers*

- **[Physics in 2-Steps: Locking Motion Priors Before Visual Refinement Erases Them](https://arxiv.org/abs/2606.06361v1)**  
  Authors: Woojung Han, Seil Kang, Youngjun Jun, Min-Hung Chen, Fu-En Yang, Seong Jae Hwang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.06361v1.pdf)  
  Keywords: trajectory, diffusion model, image-to-video, denoising, video diffusion, physics, physical  
- **[Resonant Minds: Closed-Loop Social Avatars with Theory of Mind](https://arxiv.org/abs/2606.05896v1)**  
  Authors: Jianxu Shangguan, Jing Xu, Hang Ye, Xiaoxuan Ma, Yizhou Wang, Wentao Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.05896v1.pdf)  
  Keywords: evaluation, dynamics, avatar, controllable, talking head, video generation  
- **[The Invisible Hand of Physics: When Video Diffusion Models Know More Than They Show](https://arxiv.org/abs/2606.05328v1)**  
  Authors: Parsa Esmati, Somjit Nath, Katja Hofmann, Derek Nowrouzezahrai, Samira Ebrahimi Kahou, Majid Mirmehdi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.05328v1.pdf)  
  Keywords: diffusion model, physical, denoising, video diffusion, world simulator, diffusion transformer, physics  
- **[Dream.exe: Can Video Generation Models Dream Executable Robot Manipulation?](https://arxiv.org/abs/2606.04811v2)**  
  Authors: Rui Zhao, Kaiming Yang, Jifeng Zhu, Siyang Chen, Ziqi Wang, Weijia Wu, Kevin Qinghong Lin, Heng Wang, Mike Zheng Shou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.04811v2.pdf) | [![GitHub](https://img.shields.io/github/stars/showlab/Dream.exe?style=social)](https://github.com/showlab/Dream.exe)  
  Keywords: evaluation, trajectory, benchmark, physics, physical, video generation  
- **[Activation Steering of Video Generation Models via Reduced-Order Linear Optimal Control](https://arxiv.org/abs/2606.04775v1)**  
  Authors: Jihoon Hong, Alice Chan, Qiyue Dai, Julian Skifstad, Glen Chou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.04775v1.pdf)  
  Keywords: benchmark, dynamics, t2v, video generation, concept, text-to-video  
- **[Physics-Informed Video Generation via Mixture-of-Experts Latent Alignment](https://arxiv.org/abs/2606.04737v1)**  
  Authors: Cong Wang, Hanxin Zhu, Jiayi Luo, Yonglin Tian, Xiaoqian Cheng, Peiyan Tu, Xin Jin, Long Chen, Zhibo Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.04737v1.pdf)  
  Keywords: benchmark, dynamics, physics, physics-aware, physical, video generation  
- **[Building The Ph(ysical)AI Layer Of Machine Intelligence](https://arxiv.org/abs/2606.04106v1)**  
  Authors: Ulbert Jose Botero, Liam Smith, Brooks Olney, Pooya Khorrami, Steven Kusiak, Watson Jia, Sage Trudeau, Daniel Capecci  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.04106v1.pdf)  
  Keywords: physics, architecture, efficient, physical  
- **[PointAction: 3D Points as Universal Action Representations for Robot Control](https://arxiv.org/abs/2606.03943v1)**  
  Authors: Mutian Tong, Han Jiang, Qiao Feng, Lingjie Liu, Jiatao Gu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.03943v1.pdf)  
  Keywords: diffusion model, dynamics, video prediction, 4d generation, video diffusion, video generation, simulation  
- **[Mamba-Enhanced Implicit Motion Learning for Audio-Driven Portrait Animation](https://arxiv.org/abs/2606.03402v2)**  
  Authors: Xuan Wei, Jiahui Chen, Kaiheng Li, Mingyu Shao, Qingqi Hong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.03402v2.pdf)  
  Keywords: diffusion model, benchmark, dynamics, audio-driven, human animation, gesture, architecture, human motion, video generation  
- **[Learning to Solve, Forgetting to Retain: Correct-Set Turnover in RLVR](https://arxiv.org/abs/2606.03087v1)**  
  Authors: Chuanyu Qin, Chenxu Yang, Qingyi Si, Naibin Gu, Peng Fu, Zheng Lin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.03087v1.pdf)  
  Keywords: benchmark, dynamics, dit  

### Surveys & Benchmarks

*Showing the latest 50 out of 232 papers*

- **[LoomVideo: Unifying Multimodal Inputs into Video Generation and Editing](https://arxiv.org/abs/2606.06042v1)**  
  Authors: Jianzong Wu, Hao Lian, Jiongfan Yang, Dachao Hao, Ye Tian, Yunhai Tong, Jingyuan Zhu, Biaolong Chen, Qiaosong Qi, Aixi Zhang, Wanggui He, Mushui Liu, Jinlong Liu, Hao Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.06042v1.pdf)  
  Keywords: benchmark, dit, architecture, acceleration, efficient, diffusion transformer, video generation, video editing  
- **[Resonant Minds: Closed-Loop Social Avatars with Theory of Mind](https://arxiv.org/abs/2606.05896v1)**  
  Authors: Jianxu Shangguan, Jing Xu, Hang Ye, Xiaoxuan Ma, Yizhou Wang, Wentao Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.05896v1.pdf)  
  Keywords: evaluation, dynamics, avatar, controllable, talking head, video generation  
- **[LongSpace: Exploring Long-Horizon Spatial Memory from Perception to Recall in Video](https://arxiv.org/abs/2606.05677v1)**  
  Authors: Shiqiang Lang, Jing Liu, Haoyang He, Peiwen Sun, Yuanteng Chen, Tao Liu, Lan Yang, Longteng Guo, Honggang Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.05677v1.pdf)  
  Keywords: autonomous driving, benchmark, layout, long video  
- **[V2V-Bench: A Comprehensive Benchmark for Video-to-Video Generation Evaluation](https://arxiv.org/abs/2606.05665v1)**  
  Authors: Tao Liu, Leela Krishna, Gouti Pavan Kumar, Sreeja K, Vishav Garg  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.05665v1.pdf)  
  Keywords: evaluation, benchmark, dit, i2v, t2v, video generation, video-to-video  
- **[Controllable Dynamic 3D Shape Generation via 3D Trajectories and Text](https://arxiv.org/abs/2606.05162v1)**  
  Authors: Jaeyeong Kim, Ines Kim, Jahyeok Koo, Seungryong Kim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.05162v1.pdf)  
  Keywords: evaluation, trajectory, controllable, dit, video generation  
- **[Dream.exe: Can Video Generation Models Dream Executable Robot Manipulation?](https://arxiv.org/abs/2606.04811v2)**  
  Authors: Rui Zhao, Kaiming Yang, Jifeng Zhu, Siyang Chen, Ziqi Wang, Weijia Wu, Kevin Qinghong Lin, Heng Wang, Mike Zheng Shou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.04811v2.pdf) | [![GitHub](https://img.shields.io/github/stars/showlab/Dream.exe?style=social)](https://github.com/showlab/Dream.exe)  
  Keywords: evaluation, trajectory, benchmark, physics, physical, video generation  
- **[Activation Steering of Video Generation Models via Reduced-Order Linear Optimal Control](https://arxiv.org/abs/2606.04775v1)**  
  Authors: Jihoon Hong, Alice Chan, Qiyue Dai, Julian Skifstad, Glen Chou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.04775v1.pdf)  
  Keywords: benchmark, dynamics, t2v, video generation, concept, text-to-video  
- **[Physics-Informed Video Generation via Mixture-of-Experts Latent Alignment](https://arxiv.org/abs/2606.04737v1)**  
  Authors: Cong Wang, Hanxin Zhu, Jiayi Luo, Yonglin Tian, Xiaoqian Cheng, Peiyan Tu, Xin Jin, Long Chen, Zhibo Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.04737v1.pdf)  
  Keywords: benchmark, dynamics, physics, physics-aware, physical, video generation  
- **[Bootstrap Your Generator: Unpaired Visual Editing with Flow Matching](https://arxiv.org/abs/2606.03911v1)**  
  Authors: Yoad Tewel, Yuval Atzmon, Gal Chechik, Lior Wolf  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.03911v1.pdf)  
  Keywords: evaluation, flow matching, dit, video editing  
- **[Mamba-Enhanced Implicit Motion Learning for Audio-Driven Portrait Animation](https://arxiv.org/abs/2606.03402v2)**  
  Authors: Xuan Wei, Jiahui Chen, Kaiheng Li, Mingyu Shao, Qingqi Hong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.03402v2.pdf)  
  Keywords: diffusion model, benchmark, dynamics, audio-driven, human animation, gesture, architecture, human motion, video generation  

### Text-to-Video Generation

*Showing the latest 50 out of 53 papers*

- **[V2V-Bench: A Comprehensive Benchmark for Video-to-Video Generation Evaluation](https://arxiv.org/abs/2606.05665v1)**  
  Authors: Tao Liu, Leela Krishna, Gouti Pavan Kumar, Sreeja K, Vishav Garg  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.05665v1.pdf)  
  Keywords: evaluation, benchmark, dit, i2v, t2v, video generation, video-to-video  
- **[Do Models Share Safety Representations? Cross-Model Steering for Safe Visual Generation](https://arxiv.org/abs/2606.05290v1)**  
  Authors: Tobia Poppi, Silvia Cappelletti, Sara Sarto, Florian Schiffers, Garin Kessler, Marcella Cornia, Lorenzo Baraldi, Rita Cucchiara  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.05290v1.pdf)  
  Keywords: text-to-video, architecture, video generation  
- **[Activation Steering of Video Generation Models via Reduced-Order Linear Optimal Control](https://arxiv.org/abs/2606.04775v1)**  
  Authors: Jihoon Hong, Alice Chan, Qiyue Dai, Julian Skifstad, Glen Chou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.04775v1.pdf)  
  Keywords: benchmark, dynamics, t2v, video generation, concept, text-to-video  
- **[Spatial-Temporal Decoupled Reference Conditioning for Identity-Preserving Text-to-Video Generation](https://arxiv.org/abs/2606.02441v1)**  
  Authors: Yuheng Chen, Teng Hu, Yuji Wang, Qingdong He, Lizhuang Ma, Jiangning Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.02441v1.pdf)  
  Keywords: layout, dit, temporal consistency, identity, video generation, text-to-video  
- **[SafeGen-Bench: Benchmarking Safety in Image-Conditioned Text-to-Video Generation](https://arxiv.org/abs/2606.01481v1)**  
  Authors: Yingzi Ma, Xiaogeng Liu, Yawen Zheng, Chaowei Xiao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.01481v1.pdf)  
  Keywords: diffusion model, benchmark, controllable, dit, t2v, video generation, text-to-video  
- **[Knowledge-Intensive Video Generation](https://arxiv.org/abs/2606.01285v1)**  
  Authors: Chenxu Wang, Mingda Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.01285v1.pdf)  
  Keywords: evaluation, benchmark, text-to-video, video generation  
- **[Boundary-Protection W8A8 HiFloat8 Quantization for Large-Scale Text-to-Video Diffusion Transformers](https://arxiv.org/abs/2606.00957v1)**  
  Authors: Yiming Zhao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.00957v1.pdf)  
  Keywords: evaluation, dit, t2v, video diffusion, diffusion transformer, text-to-video  
- **[Collaborative Few-Step Distillation and Low-Bit Quantization for Wan2.2 Dual-Expert Video Diffusion Models](https://arxiv.org/abs/2606.00658v1)**  
  Authors: Jinyang Du, Shenghao Jin, Ziqian Xu, Ruihao Gong, Shiqiao Gu, Yang Yong, Jinyang Guo, Xianglong Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.00658v1.pdf)  
  Keywords: trajectory, diffusion model, t2v, denoising, distillation, style, video diffusion  
- **[TunerDiT: Training-free Progressive Steering of Diffusion Transformer for Multi-Event Video Generation](https://arxiv.org/abs/2605.31590v1)**  
  Authors: Ruotong Liao, Guowen Huang, Qing Cheng, Guangyao Zhai, Lei Zhang, Xun Xiao, Thomas Seidl, Daniel Cremers, Volker Tresp  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.31590v1.pdf)  
  Keywords: trajectory, benchmark, layout, dit, t2v, denoising, video generation, video diffusion, diffusion transformer, text-to-video  
- **[SlotMemory: Object-Centric KV Memory for Streaming Long-Video Generation](https://arxiv.org/abs/2605.31033v1)**  
  Authors: Weijia Dou, Hui Li, Jiahao Cui, Lei Zhou, Jingdong Wang, Siyu Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.31033v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://tj12323.github.io/SlotMemory)  
  Keywords: t2v, identity, long-form, streaming, video diffusion, interactive, video synthesis, video generation  

### Video Editing

- **[LoomVideo: Unifying Multimodal Inputs into Video Generation and Editing](https://arxiv.org/abs/2606.06042v1)**  
  Authors: Jianzong Wu, Hao Lian, Jiongfan Yang, Dachao Hao, Ye Tian, Yunhai Tong, Jingyuan Zhu, Biaolong Chen, Qiaosong Qi, Aixi Zhang, Wanggui He, Mushui Liu, Jinlong Liu, Hao Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.06042v1.pdf)  
  Keywords: benchmark, dit, architecture, acceleration, efficient, diffusion transformer, video generation, video editing  
- **[V2V-Bench: A Comprehensive Benchmark for Video-to-Video Generation Evaluation](https://arxiv.org/abs/2606.05665v1)**  
  Authors: Tao Liu, Leela Krishna, Gouti Pavan Kumar, Sreeja K, Vishav Garg  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.05665v1.pdf)  
  Keywords: evaluation, benchmark, dit, i2v, t2v, video generation, video-to-video  
- **[Bootstrap Your Generator: Unpaired Visual Editing with Flow Matching](https://arxiv.org/abs/2606.03911v1)**  
  Authors: Yoad Tewel, Yuval Atzmon, Gal Chechik, Lior Wolf  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.03911v1.pdf)  
  Keywords: evaluation, flow matching, dit, video editing  
- **[AlbedoEdit: Unified Instance-Level Video Editing with Albedo Guidance](https://arxiv.org/abs/2606.01362v1)**  
  Authors: Xilong Zhou, Bao-Huy Nguyen, Zheng Zeng, Jacob Munkberg, Jon Hasselgren, Thomas Leimkühler, Nima Kalantari, Miloš Hašan, Christian Theobalt  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.01362v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://vcai.mpi-inf.mpg.de/projects/AlbedoEdit)  
  Keywords: creative, dit, video editing  
- **[DeltaCam: Differential Intrinsic Camera Modeling for Video Generation](https://arxiv.org/abs/2605.25266v1)**  
  Authors: Debabrata Mandal, Zhihan Peng, Yujie Wang, Praneeth Chakravarthula  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25266v1.pdf)  
  Keywords: dynamics, controllable, dit, video style transfer, style, video diffusion, video generation, video-to-video  
- **[Geo-Align: Video Generation Alignment via Metric Geometry Reward](https://arxiv.org/abs/2605.23903v1)**  
  Authors: Zizun Li, Haoyu Guo, Runzhe Teng, Chunhua Shen, Tong He  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.23903v1.pdf)  
  Keywords: dit, camera control, physical, video generation, video-to-video  
- **[SimInsert: Seamless Video Object Insertion via Regional Sparse Attention Fusion](https://arxiv.org/abs/2605.23245v1)**  
  Authors: Xinyu Chen, Yuyi Qian, Jiang Lin, Shenyi Wang, Gao Wang, Zhiqiu Zhang, Jizhi Zhang, Mingjie Wang, Qiang Tang, Qian Wang, Song Wu, Zili Yi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.23245v1.pdf)  
  Keywords: trajectory, diffusion model, dit, image-to-video, denoising, interactive, video diffusion, efficient, video editing  
- **[StreamGVE: Training-Free Video Editing via Few-Step Streaming Video Generation](https://arxiv.org/abs/2605.21466v1)**  
  Authors: Guanlong Jiao, Chenyangguang Zhang, Jia Jun Cheng Xian, Zewei Zhang, Renjie Liao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.21466v1.pdf)  
  Keywords: dit, streaming, video generation, video editing  
- **[Preserve, Reveal, Expand: Faithful 4D Video Editing with Region-Aware Conditioning](https://arxiv.org/abs/2605.20961v1)**  
  Authors: Zhangchi Hu, Wenzhang Sun, Xiangchen Yin, Jiahui Yuan, Chunfeng Wang, Hao Li, Kun Zhan, Xiaoyan Sun  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20961v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://ricepastem.github.io/PREX-Open)  
  Keywords: evaluation, diffusion model, benchmark, dit, video diffusion, video editing  
- **[What Semantics Survive the Connector? Diagnosing VLM-to-DiT Alignment in Video Editing](https://arxiv.org/abs/2605.20795v1)**  
  Authors: Hangyu Lin, Chao Wen, Chengming Xu, Jianxiong Gao, Jiangning Zhang, Xiaobin Hu, Yanwei Fu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20795v1.pdf)  
  Keywords: evaluation, dit, flow matching, architecture, multi-modal, video editing  

### Video Inpainting & Completion

- **[PointAction: 3D Points as Universal Action Representations for Robot Control](https://arxiv.org/abs/2606.03943v1)**  
  Authors: Mutian Tong, Han Jiang, Qiao Feng, Lingjie Liu, Jiatao Gu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.03943v1.pdf)  
  Keywords: diffusion model, dynamics, video prediction, 4d generation, video diffusion, video generation, simulation  
- **[World Models: A Comprehensive Survey of Architectures, Methodologies, Reasoning Paradigms, and Applications](https://arxiv.org/abs/2606.00133v1)**  
  Authors: Arif Hassan Zidan, Yi Pan, Hanqi Jiang, Ruiyu Yan, Wei Ruan, Zihao Wu, Lifeng Chen, Weihang You, Xinliang Li, Bowen Chen, Huawen Hu, Peilong Wang, Sizhuang Liu, Jing Zhang, Siyuan Li, Zhengliang Liu, Yu Bao, Lin Zhao, Lichao Sun, Dajiang Zhu, Xiang Li, Jinglei Lv, Quanzheng Li, Wei Liu, Tianming Liu, Wei Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.00133v1.pdf)  
  Keywords: evaluation, benchmark, dynamics, autonomous driving, education, video prediction, medical, robotics, world model, architecture, interactive, survey, physics, video generation  
- **[Full-4D: Generating Full-Scope 4D Scenes from a Single-View Video](https://arxiv.org/abs/2605.25500v1)**  
  Authors: Tingxi Chen, Ke Hao, Yabo Chen, Zhengxue Cheng, Rong Xie, Li Song, Haibin Huang, Chi Zhang, Xuelong Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25500v1.pdf)  
  Keywords: diffusion model, dit, multi-view video, distillation, flow matching, 4d generation, video interpolation, interactive, video diffusion, video synthesis, physical  
- **[CRONOS: Benchmarking Counterfactual Physical Consistency in Video Models](https://arxiv.org/abs/2605.23699v1)**  
  Authors: León Begiristain, Olaf Dünkel, Adam Kortylewski  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.23699v1.pdf)  
  Keywords: evaluation, benchmark, dynamics, dit, video prediction, world model, physical  
- **[GEM-4D: Geometry-Enhanced Video World Models for Robot Manipulation](https://arxiv.org/abs/2605.22882v2)**  
  Authors: Kaichen Zhou, Yuzhen Chen, Fangneng Zhan, Hang Hua, Grace Chen, Xinhai Chang, Ao Qu, Yilun Du, Zhuang Liu, Paul Pu Liang, Mengyu Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.22882v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://gem-4d.github.io)  
  Keywords: dynamics, dit, video prediction, world model, architecture, physical, simulation  
- **[Goodbye Drift: Anchored Tree Sampling for Long-Horizon Video-to-Video Generation](https://arxiv.org/abs/2605.20476v1)**  
  Authors: Matthew Bendel, Stephen W. Bailey, Mithilesh Vaidya, Sumukh Badam, Xingzhe He  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20476v1.pdf)  
  Keywords: outpainting, dit, autoregressive, t2v, distillation, style, video generation, video-to-video  
- **[Nano World Models: A Minimalist Implementation of Future Video Prediction](https://arxiv.org/abs/2605.23993v2)**  
  Authors: Siqiao Huang, Partha Kaushik, Michael Chen, Hengkai Pan, Kaiwen Geng, Omar Chehab, Fernando Moreno-Pino, Max Simchowitz  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.23993v2.pdf)  
  Keywords: evaluation, dit, autoregressive, video prediction, world model, architecture, interactive, video generation, simulation  
- **[Relit-LiVE: Relight Video by Jointly Learning Environment Video](https://arxiv.org/abs/2605.06658v1)**  
  Authors: Weiqing Xiao, Hong Li, Xiuyu Yang, Houyuan Chen, Wenyi Li, Tianqi Liu, Shaocong Xu, Chongjie Ye, Hao Zhao, Beibei Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.06658v1.pdf) | [![GitHub](https://img.shields.io/github/stars/zhuxing0/Relit-LiVE?style=social)](https://github.com/zhuxing0/Relit-LiVE)  
  Keywords: diffusion model, benchmark, dit, video prediction, streaming, video diffusion, physical  
- **[Quaternion Nonlinear Transform-Induced Nuclear Norm for Low-Rank Tensor Completion](https://arxiv.org/abs/2605.01467v1)**  
  Authors: Biswarup Karmakar, Ratikanta Behera  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.01467v1.pdf)  
  Keywords: benchmark, efficient, video inpainting  
- **[LMGenDrive: Bridging Multimodal Understanding and Generative World Modeling for End-to-End Driving](https://arxiv.org/abs/2604.08719v1)**  
  Authors: Hao Shao, Letian Wang, Yang Zhou, Yuxuan Hu, Zhuofan Zong, Steven L. Waslander, Wei Zhan, Hongsheng Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2604.08719v1.pdf)  
  Keywords: benchmark, autonomous driving, autoregressive, video prediction, world model, video generation  

### Video Super-Resolution & Enhancement

*Showing the latest 50 out of 72 papers*

- **[Physics in 2-Steps: Locking Motion Priors Before Visual Refinement Erases Them](https://arxiv.org/abs/2606.06361v1)**  
  Authors: Woojung Han, Seil Kang, Youngjun Jun, Min-Hung Chen, Fu-En Yang, Seong Jae Hwang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.06361v1.pdf)  
  Keywords: trajectory, diffusion model, image-to-video, denoising, video diffusion, physics, physical  
- **[RhymeFlow: Training-Free Acceleration for Video Generation with Asynchronous Denoising Flow Scheduling](https://arxiv.org/abs/2606.06309v1)**  
  Authors: Chensheng Dai, Shengjun Zhang, Yifan Li, Zhang Zhang, Zheng Zhu, Yueqi Duan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.06309v1.pdf)  
  Keywords: trajectory, dit, denoising, acceleration, video synthesis, diffusion transformer, video generation  
- **[ReCache: Learning Budget-Aware Caching Schedules for Diffusion Models via REINFORCE](https://arxiv.org/abs/2606.06060v1)**  
  Authors: Mishan Aliev, Eva Neudachina, Ilya Bykov, Aleksandr Oganov, Kirill Struminsky, Aibek Alanov, Denis Rakitin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.06060v1.pdf) | [![GitHub](https://img.shields.io/github/stars/thecrazymage/ReCache?style=social)](https://github.com/thecrazymage/ReCache)  
  Keywords: trajectory, diffusion model, controllable, denoising  
- **[The Invisible Hand of Physics: When Video Diffusion Models Know More Than They Show](https://arxiv.org/abs/2606.05328v1)**  
  Authors: Parsa Esmati, Somjit Nath, Katja Hofmann, Derek Nowrouzezahrai, Samira Ebrahimi Kahou, Majid Mirmehdi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.05328v1.pdf)  
  Keywords: diffusion model, physical, denoising, video diffusion, world simulator, diffusion transformer, physics  
- **[DSA: Dynamic Step Allocation for Fast Autoregressive Video Generation](https://arxiv.org/abs/2606.04432v1)**  
  Authors: Thanh-Tung Le, Yunhan Zhao, Menglei Chai, Zhengyang Shen, Zhe Cao, Danhang Tang, Xiaohui Xie, Deying Kong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.04432v1.pdf)  
  Keywords: diffusion model, dit, autoregressive, denoising, distillation, interactive, video diffusion, diffusion transformer, video generation  
- **[Real-Time Generation of Streamable Talking Portrait Video with Reference-Guided Deep Compression VAEs](https://arxiv.org/abs/2606.01620v1)**  
  Authors: Sicheng Xu, Yu Deng, Shoukang Hu, Yichuan Wang, Yizhong Zhang, Zhan Chen, Jiaolong Yang, Baining Guo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.01620v1.pdf)  
  Keywords: diffusion model, rectified flow, dit, autoregressive, denoising, architecture, streaming, video diffusion, interactive, video generation  
- **[SKIP: Sparse Keyframe Interpolation Paradigm for Efficient Embodied World Models](https://arxiv.org/abs/2606.00664v1)**  
  Authors: Ziheng He, Yixiang Chen, Ning Yang, Zhanqian Wu, Qisen Ma, Yuan Xu, Jiabing Yang, Peiyan Li, Xiangnan Wu, Xiaofeng Wang, Zheng Zhu, Jing Liu, Nianfeng Liu, Yan Huang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.00664v1.pdf)  
  Keywords: diffusion model, dit, frame interpolation, action-conditioned, robotics, world model, video diffusion, efficient, simulation  
- **[Collaborative Few-Step Distillation and Low-Bit Quantization for Wan2.2 Dual-Expert Video Diffusion Models](https://arxiv.org/abs/2606.00658v1)**  
  Authors: Jinyang Du, Shenghao Jin, Ziqian Xu, Ruihao Gong, Shiqiao Gu, Yang Yong, Jinyang Guo, Xianglong Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.00658v1.pdf)  
  Keywords: trajectory, diffusion model, t2v, denoising, distillation, style, video diffusion  
- **[TunerDiT: Training-free Progressive Steering of Diffusion Transformer for Multi-Event Video Generation](https://arxiv.org/abs/2605.31590v1)**  
  Authors: Ruotong Liao, Guowen Huang, Qing Cheng, Guangyao Zhai, Lei Zhang, Xun Xiao, Thomas Seidl, Daniel Cremers, Volker Tresp  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.31590v1.pdf)  
  Keywords: trajectory, benchmark, layout, dit, t2v, denoising, video generation, video diffusion, diffusion transformer, text-to-video  
- **[Robust Dreamer: Deviation-Aware Latent Gaussian Memory for Action-Controlled AR Video Generation](https://arxiv.org/abs/2605.30855v2)**  
  Authors: Hanlin Chen, Jiaxin Wei, Xibin Song, Yifu Wang, Steve Wang, Hongdong Li, Pan Ji, Gim Hee Lee  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30855v2.pdf)  
  Keywords: dit, autoregressive, image-to-video, 3d-aware, denoising, interactive, video generation, simulation  

### World Models & Simulation

*Showing the latest 50 out of 123 papers*

- **[The Invisible Hand of Physics: When Video Diffusion Models Know More Than They Show](https://arxiv.org/abs/2606.05328v1)**  
  Authors: Parsa Esmati, Somjit Nath, Katja Hofmann, Derek Nowrouzezahrai, Samira Ebrahimi Kahou, Majid Mirmehdi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.05328v1.pdf)  
  Keywords: diffusion model, physical, denoising, video diffusion, world simulator, diffusion transformer, physics  
- **[DSA: Dynamic Step Allocation for Fast Autoregressive Video Generation](https://arxiv.org/abs/2606.04432v1)**  
  Authors: Thanh-Tung Le, Yunhan Zhao, Menglei Chai, Zhengyang Shen, Zhe Cao, Danhang Tang, Xiaohui Xie, Deying Kong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.04432v1.pdf)  
  Keywords: diffusion model, dit, autoregressive, denoising, distillation, interactive, video diffusion, diffusion transformer, video generation  
- **[PointAction: 3D Points as Universal Action Representations for Robot Control](https://arxiv.org/abs/2606.03943v1)**  
  Authors: Mutian Tong, Han Jiang, Qiao Feng, Lingjie Liu, Jiatao Gu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.03943v1.pdf)  
  Keywords: diffusion model, dynamics, video prediction, 4d generation, video diffusion, video generation, simulation  
- **[Cosmos 3: Omnimodal World Models for Physical AI](https://arxiv.org/abs/2606.02800v1)**  
  Authors: Aditi, Niket Agarwal, Arslan Ali, Jon Allen, Martin Antolini, Adeline Aubame, Alisson Azzolini, Junjie Bai, Maciej Bala, Yogesh Balaji, Josh Bapst, Aarti Basant, Mukesh Beladiya, Mohammad Qazim Bhat, Zaid Pervaiz Bhat, Dan Blick, Vanni Brighella, Han Cai, Tiffany Cai, Eric Cameracci, Jiaxin Cao, Yulong Cao, Mark Carlson, Carlos Casanova, Ting-Yun Chang, Yan Chang, Yu-Wei Chao, Prithvijit Chattopadhyay, Roshan Chaudhari, Chieh-Yun Chen, Junyu Chen, Ke Chen, Qizhi Chen, Wenkai Chen, Xiaotong Chen, Yu Chen, An-Chieh Cheng, Click Cheng, Xiu Chia, Jeana Choi, Chaeyeon Chung, Wenyan Cong, Yin Cui, Magdalena Dadela, Nalin Dadhich, Wenliang Dai, Joyjit Daw, Alperen Degirmenci, Rodrigo Vieira Del Monte, Robert Denomme, Sameer Dharur, Marco Di Lucca, Ke Ding, Wenhao Ding, Yifan Ding, Yuzhu Dong, Nicole Drumheller, Yilun Du, Aigul Dzhumamuratova, Aleksandr Efitorov, Hamid Eghbalzadeh, Naomi Eigbe, Imad El Hanafi, Hassan Eslami, Benedikt Falk, Jiaojiao Fan, Jim Fan, Amol Fasale, Sergiy Fefilatyev, Liang Feng, Francesco Ferroni, Sanja Fidler, Xiao Fu, Vikram Fugro, Prashant Gaikwad, TJ Galda, Katelyn Gao, Yihuai Gao, Wenhang Ge, Sreyan Ghosh, Arushi Goel, Vivek Goel, Akash Gokul, Rama Govindaraju, Jinwei Gu, Miguel Guerrero, Elfie Guo, Aryaman Gupta, Siddharth Gururani, Hugo Hadfield, Song Han, Ankur Handa, Zekun Hao, Mohammad Harrim, Ali Hassani, Nathan Hayes-Roth, Yufan He, Chris Helvig, Cyrus Hogg, Madison Huang, Michael Huang, Sophia Huang, Yufan Huang, Jacob Huffman, DeLesley Hutchins, Suneel Indupuru, Boris Ivanovic, Arihant Jain, Joel Jang, Ryan Ji, Yanan Jian, Dongfu Jiang, Jingyi Jin, Atharva Joshi, Nikhilesh Joshi, Pranjali Joshi, Jaehun Jung, Weiwei Kang, Scott Kassekert, Jan Kautz, Ashna Khetan, Julia Kiczka, Slawek Kierat, Gwanghyun Kim, Kuno Kim, Sunny Kim, Kezhi Kong, Xin Kong, Zhifeng Kong, Tomasz Kornuta, Egor Krivov, Hui Kuang, Saurav Kumar, Chia-Wen Kuo, George Kurian, Wojciech Kutak, JF Lafleche, Himangshu Lahkar, Omar Laymoun, Jayjun Lee, Sanggil Lee, Gabriele Leone, Boyi Li, Freya Li, Jiajun Li, Jinfeng Li, Ling Li, Pengcheng Li, Shangru Li, Tingle Li, Xiaolong Li, Xuan Li, Zhaoshuo Li, Zhiqi Li, Hao Liang, Maosheng Liao, Chen-Hsuan Lin, Tsung-Yi Lin, Ming-Yu Liu, Sifei Liu, Zihan Liu, Hai Loc Lu, Xiangyu Lu, Alice Luo, Ruipu Luo, Wenjie Luo, Jiangran Lyu, Martin Ding Ma, Nic Ma, Qianli Ma, Dawid Majchrowski, Louis Marcoux, Miguel Martin, Qing Miao, Ashkan Mirzaei, Shreyas Misra, Kaichun Mo, Durra Mohsin, Hyejin Moon, Pawel Morkisz, Saeid Motiian, Kirill Motkov, Seungjun Nah, Yashraj Narang, Deepak Narayanan, Thabang Ngazimbi, Julian Ouyang, David Page, Yatian Pang, Sehwi Park, Mahesh Patekar, Mostofa Patwary, Marco Pavone, Trung Pham, Wei Ping, Soha Pouya, Shrimai Prabhumoye, Varun Praveen, Delin Qu, Hesam Rabeti, Morteza Ramezanali, Marilyn Reeb, Xuanchi Ren, Kristen Rumley, Wojciech Rymer, Jun Saito, Yeongho Seol, John Shao, Piyush Shekdar, Tianwei Shen, Humphrey Shi, Min Shi, Stella Shi, Kevin Shih, Mohammad Shoeybi, Mateusz Sieniawski, Shuran Song, Alexander Sotelo, Amir Sotoodeh, Sunil Srinivasa, Vignesh Srinivasakumar, Bartosz Stefaniak, Rahul Heinrich Steiger, Shangkun Sun, Jiaxiang Tang, Shitao Tang, Yangyang Tang, Yue Tang, Tolou Tavakkoli, Kayley Ting, Krzysztof Tomala, Wei-Cheng Tseng, Jibin Varghese, Sergei Vasilev, Thomas Volk, Raju Wagwani, Roger Waleffe, Andrew Z. Wang, Boxiang Wang, Haoxiang Wang, Qiao Wang, Shihao Wang, Shijie Wang, Ting-Chun Wang, Yan Wang, Yu Wang, David Wehr, Fangyin Wei, Xinshuo Weng, Jay Zhangjie Wu, Kedi Wu, Hongchi Xia, Summer Xiao, Tianjun Xiao, Kevin Xie, Daguang Xu, Jiashu Xu, Mengyao Xu, Ruqing Xu, Xingqian Xu, Yao Xu, Dinghao Yang, Dong Yang, Hans Yang, Xiaodong Yang, Xuning Yang, Yichu Yang, Yurong You, Zhiding Yu, Hao Yuan, Simon Yuen, Xiaohui Zeng, Pengcuo Zeren, Cindy Zha, Haotian Zhang, Jenny Zhang, Jing Zhang, Liangkai Zhang, Paris Zhang, Shun Zhang, Xuanmeng Zhang, Zhizheng Zhang, Ann Zhao, Yilin Zhao, Yuliya Zhautouskaya, Charles Zhou, Fengzhe Zhou, Shilin Zhu, Yuke Zhu, Dima Zhylko, Artur Zolkowski  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.02800v1.pdf) | [![GitHub](https://img.shields.io/github/stars/nvidia/cosmos?style=social)](https://github.com/nvidia/cosmos) | [![Project](https://img.shields.io/badge/-Project-blue)](https://openmdw.ai/license/1-1) | [![HuggingFace](https://img.shields.io/badge/-HuggingFace-yellow)](https://huggingface.co/collections/nvidia/cosmos3)  
  Keywords: evaluation, benchmark, image-to-video, world model, architecture, world simulator, physical  
- **[RoboDream: Compositional World Models for Scalable Robot Data Synthesis](https://arxiv.org/abs/2606.02577v1)**  
  Authors: Junjie Ye, Rong Xue, Basile Van Hoorick, Runhao Li, Harshitha Rajaprakash, Pavel Tokmakov, Muhammad Zubair Irshad, Vitor Guizilini, Yue Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.02577v1.pdf)  
  Keywords: trajectory, diffusion model, dit, world model, video diffusion, physical, novel view  
- **[From Zero to Hero: Training-Free Custom Concept Spawning in World Models](https://arxiv.org/abs/2606.02575v1)**  
  Authors: Kiymet Akdemir, Pinar Yanardag  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.02575v1.pdf)  
  Keywords: controllable, dit, autoregressive, image-to-video, identity, world model, interactive, concept, video generation, simulation  
- **[Real-Time Generation of Streamable Talking Portrait Video with Reference-Guided Deep Compression VAEs](https://arxiv.org/abs/2606.01620v1)**  
  Authors: Sicheng Xu, Yu Deng, Shoukang Hu, Yichuan Wang, Yizhong Zhang, Zhan Chen, Jiaolong Yang, Baining Guo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.01620v1.pdf)  
  Keywords: diffusion model, rectified flow, dit, autoregressive, denoising, architecture, streaming, video diffusion, interactive, video generation  
- **[MPMWorlds: Material-Point-Method Simulations for Inferring and Extrapolating Physical Dynamics](https://arxiv.org/abs/2606.01538v1)**  
  Authors: Žiga Kovačič, Kevin Ellis  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.01538v1.pdf)  
  Keywords: diffusion model, dynamics, physical simulation, video diffusion, physical, simulation  
- **[MBench: A Comprehensive Benchmark on Memory Capability for Video World Models](https://arxiv.org/abs/2606.00793v1)**  
  Authors: Shengjun Zhang, Zhang Zhang, Simin Huang, Zhenyu Tang, Hanyang Wang, Chensheng Dai, Min Chen, Yifan Li, Yuxin Li, Yingjie Chen, Hao Liu, Chen Li, Yueqi Duan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.00793v1.pdf)  
  Keywords: evaluation, benchmark, long video, world model, video generation  
- **[SKIP: Sparse Keyframe Interpolation Paradigm for Efficient Embodied World Models](https://arxiv.org/abs/2606.00664v1)**  
  Authors: Ziheng He, Yixiang Chen, Ning Yang, Zhanqian Wu, Qisen Ma, Yuan Xu, Jiabing Yang, Peiyan Li, Xiangnan Wu, Xiaofeng Wang, Zheng Zhu, Jing Liu, Nianfeng Liu, Yan Huang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.00664v1.pdf)  
  Keywords: diffusion model, dit, frame interpolation, action-conditioned, robotics, world model, video diffusion, efficient, simulation  



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
