# Awesome Video Diffusions [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of latest research papers, projects and resources related to Video Diffusion Models and Video Generation. Content is automatically updated daily.

> Last Update: 2026-07-05 03:25:26

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

- [3D-aware Video Generation](#3d-aware-video-generation) (23 papers) - Video generation with 3D awareness, multi-view consistency, and 4D content creation
- [Applications](#applications) (48 papers) - Domain-specific applications of video diffusion models
- [Architecture & Efficiency](#architecture-&-efficiency) (364 papers) - Architectural innovations (DiT, UNet), flow matching, and training/inference efficiency
- [Audio & Multi-modal](#audio-&-multi-modal) (24 papers) - Audio-driven and multi-modal conditioned video generation
- [Controllable Generation](#controllable-generation) (141 papers) - Controllable video generation with motion, camera, pose, or layout guidance
- [Human & Character Animation](#human-&-character-animation) (22 papers) - Human-centric video generation including talking heads, dance, and character animation
- [Image-to-Video Generation](#image-to-video-generation) (50 papers) - Methods for animating still images into videos
- [Long Video Generation](#long-video-generation) (134 papers) - Generating temporally consistent long-form videos beyond short clips
- [Personalization & Customization](#personalization-&-customization) (89 papers) - Personalized video generation with custom subjects, identities, or styles
- [Physical Understanding](#physical-understanding) (154 papers) - Physics-aware video generation and dynamics modeling
- [Surveys & Benchmarks](#surveys-&-benchmarks) (235 papers) - Survey papers, benchmarks, and evaluation metrics for video generation
- [Text-to-Video Generation](#text-to-video-generation) (66 papers) - Foundation models and methods for generating videos from text prompts
- [Video Editing](#video-editing) (28 papers) - Diffusion-based video editing, style transfer, and manipulation
- [Video Inpainting & Completion](#video-inpainting-&-completion) (9 papers) - Video inpainting, completion, outpainting, and temporal prediction
- [Video Super-Resolution & Enhancement](#video-super-resolution-&-enhancement) (67 papers) - Video quality improvement, upscaling, restoration, and frame interpolation
- [World Models & Simulation](#world-models-&-simulation) (130 papers) - Video generation as world simulators and interactive environment generation



## Table of Contents

- [Categorized Papers](#categorized-papers)
- [Classic Papers](#classic-papers)
- [Open Source Projects](#open-source-projects)
- [Applications](#applications)
- [Tutorials & Blogs](#tutorials--blogs)





## Categorized Papers

### 3D-aware Video Generation

- **[HandsOnWorld: Unconstrained Egocentric Video Generation with Camera-Disentangled Hand Control](https://arxiv.org/abs/2607.02075v1)**  
  Authors: Yushuo Chen, Xiaoyu Shi, Xiaoshi Wu, Xintao Wang, Pengfei Wan, Yebin Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.02075v1.pdf)  
  Keywords: video generation, 3d-aware  
- **[NeoMap: Training-free Novel-View Synthesis from Single Images and Videos](https://arxiv.org/abs/2607.01962v1)**  
  Authors: Jinxi Li, Tianyi Zhang, Yafei Yang, Zihui Zhang, Peng Huang, Koon Wing Macgyver Lin, Bo Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.01962v1.pdf)  
  Keywords: video synthesis, novel view, denoising, dit, benchmark  
- **[RayPE: Ray-Space Positional Encoding for 3D-Aware Video Generation](https://arxiv.org/abs/2606.27345v2)**  
  Authors: Minghao Yin, Jiahao Lu, Wenbo Hu, Wang Zhao, Shan Ying, Kai Han  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.27345v2.pdf)  
  Keywords: diffusion transformer, video diffusion, video generation, identity, 3d-aware, camera control, dit  
- **[Follow Your Track: Precise Skeleton Animation Controlled by 3D Trajectories](https://arxiv.org/abs/2606.25344v1)**  
  Authors: Yueting Liu, Yanqin Jiang, Nian Liu, Jingmen Zhou, Zhengjun Zha, Weiming Hu, Jin Gao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.25344v1.pdf)  
  Keywords: body motion, efficient, temporal consistency, 4d generation, trajectory, dit  
- **[OmniDrive: An LLM-Choreographed Multi-Agent World Model with Unified Latent Co-Compression for Multi-View Driving Video Generation](https://arxiv.org/abs/2606.17536v1)**  
  Authors: Zijie Meng, Yufei Liu, Chengqian Ma, Zhiyu Li, Jiyuan Liu, Wenhua Nie, Bingcai Wei, Shuqin Chen, Weichen Xu, Jiquan Yuan, Miao Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17536v1.pdf)  
  Keywords: video generation, layout, world model, autonomous driving, dit, multi-view video, controllable  
- **[R2RDreamer: 3D-aware Data Augmentation for Spatially-generalized 2D Manipulation Policies](https://arxiv.org/abs/2606.17040v1)**  
  Authors: Xiuwei Xu, Haowen Sun, Angyuan Ma, Yiwei Zhang, Zhenyu Wu, Xiaofeng Wang, Bingyao Yu, Zheng Zhu, Jie Zhou, Jiwen Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17040v1.pdf)  
  Keywords: 3d-aware, style, video completion, image-to-video, simulation, dit, controllable  
- **[Flex4DHuman: Flexible Multi-view Video Diffusion for 4D Human Reconstruction](https://arxiv.org/abs/2606.13655v2)**  
  Authors: Jen-Hao Cheng, Yipeng Wang, Hao Zhang, Gengshan Yang, Jenq-Neng Hwang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13655v2.pdf)  
  Keywords: diffusion model, video diffusion, text-to-video, architecture, simulation, dit, multi-view video  
- **[Latent Spatial Memory for Video World Models](https://arxiv.org/abs/2606.09828v1)**  
  Authors: Weijie Wang, Haoyu Zhao, Yifan Yang, Feng Chen, Zeyu Zhang, Yefei He, Zicheng Duan, Donny Y. Chen, Yuqing Yang, Bohan Zhuang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.09828v1.pdf)  
  Keywords: diffusion model, video generation, world model, novel view, depth-guided  
- **[CP4D: Compositional Physics-aware 4D Scene Generation](https://arxiv.org/abs/2606.09187v1)**  
  Authors: Hanxin Zhu, Cong Wang, Tianyu He, Long Chen, Xin Jin, Chen Gao, Zhibo Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.09187v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://anonymous.4open.science/w/CP4D)  
  Keywords: diffusion model, video diffusion, physical, dynamics, physics-aware, 4d generation, physics, interactive  
- **[RigPAPR: Rig-Based Animation of Static Neural Point Clouds from a Fixed-Viewpoint Video](https://arxiv.org/abs/2606.06685v1)**  
  Authors: Shichong Peng, Yanshu Zhang, Ke Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.06685v1.pdf)  
  Keywords: i2v, image-to-video, novel view  

### Applications

- **[SpheRoPE: Zero-Shot Optimization-Free 360 Panorama Generation with Spherical RoPE](https://arxiv.org/abs/2606.32033v1)**  
  Authors: Or Hirschorn, Aaron Olender, Eli Alshan, Ianir Ideses, Lior Fritz, Sagie Benaim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.32033v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://orhir.github.io/SpheRoPE)  
  Keywords: diffusion transformer, creative  
- **[World Narrative Model for Highly Controllable Video Generation: A Paradigm Shift from Pixel Sampling to Physical World Orchestration](https://arxiv.org/abs/2606.31946v1)**  
  Authors: Ye Chen, Xuanhong Chen, Yupeng Zhu, Liming Tan, Zhewen Wan, Yuxuan Xiong, Tielong Wang, Jinfan Liu, Wuze Zhang, Xiongzhen Zhang, Feifei Li, Xianglin Luo, Zhehan Zhao, Zhifan Zhang, Laisheng Kou, Zhujing Liang, Yugang Chen, Muchun Chen, Xu Miao, Yijing Zhang, Xiaojie Sheng, Qiang Hu, Jialiang Chen, Weimin Zhang, Wenjun Zhang, Bingbing Ni  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.31946v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://glassroom.sjtu.edu.cn/WNM)  
  Keywords: video generation, layout, physical, efficient, film, dit, controllable  
- **[InfiniVerse: Occupancy Guided Unbounded Scene Generation for Autonomous Driving](https://arxiv.org/abs/2606.31109v1)**  
  Authors: Xiaoyu Ye, Leheng Li, Xinyu Ji, Yingjie Cai, Hongda He, Xu Yan, Guanyi Zhao, Ying-Cong Chen, Bingbing Liu, Shuguang Cui, Zhen Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.31109v1.pdf)  
  Keywords: diffusion model, video diffusion, autonomous driving, dit, evaluation, autoregressive, benchmark, controllable  
- **[Vertigo Vertigo: Reconstructing a Cinematic Ideal through its Predictive AI Double](https://arxiv.org/abs/2607.00047v1)**  
  Authors: Adam Cole, Mick Grierson  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.00047v1.pdf)  
  Keywords: diffusion model, video diffusion, film, frame interpolation, dit, acceleration  
- **[UnfoldArt: Zero-Shot Recovery of Full Articulated 3D Objects from Text or Image](https://arxiv.org/abs/2606.30608v2)**  
  Authors: Mohamed el Amine Boudjoghra, Ivan Laptev, Angela Dai  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.30608v2.pdf)  
  Keywords: dit, robotics, interactive  
- **[Semantic-Aware, Physics-Informed, Geometry-Grounded Weather Video Synthesis](https://arxiv.org/abs/2606.29020v1)**  
  Authors: Chenghao Qian, Nedko Savov, Lingdong Kong, Yeying Jin, Rui Song, Wenjing Li, Zhun Zhong, Jiaqi Ma, Gustav Markkula, Luc Van Gool  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.29020v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://jumponthemoon.github.io/w-crafter)  
  Keywords: dynamics, physical, identity, video synthesis, autonomous driving, simulation, physics, dit  
- **[A Good Talk Does not Look Like a Summary, It Teaches You! Measuring Takeaways from Paper-to-Video Talks](https://arxiv.org/abs/2606.28531v1)**  
  Authors: Ishani Mondal, Aparna Garimella, Ananya Sai, Pannaga Shivaswamy, Jordan Boyd-Graber  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.28531v1.pdf)  
  Keywords: evaluation, video generation, concept, education  
- **[ReWorld: Learning Better Representations for World Action Models](https://arxiv.org/abs/2606.27504v1)**  
  Authors: Tianze Xia, Lijun Zhou, Kaixin Xiong, Jingfeng Yao, Yu Zhu, Zhenxin Zhu, Bing Wang, Guang Chen, Hangjun Ye, Wenyu Liu, Haiyang Sun, Xinggang Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.27504v1.pdf)  
  Keywords: video generation, world model, autonomous driving, architecture, efficient, dit  
- **[PRISM: Feed-Forward Single-Image 3D Reconstruction via Geometric Warp-Residual Modeling](https://arxiv.org/abs/2606.25430v1)**  
  Authors: Zhijie Zheng, Xinhao Xiang, Jiawei Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.25430v1.pdf)  
  Keywords: diffusion model, video diffusion, distillation, robotics, benchmark  
- **[CineCap: Structured Reasoning with Spatio-Temporal Anchors for Cinematographic Video Captioning](https://arxiv.org/abs/2606.24636v1)**  
  Authors: Xinyu Mao, Yuhui Zeng, Xiaokun Liu, Wenyu Qin, Meng Wang, Xin Tao, Pengfei Wan, Xiaohan Xing, Max Meng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.24636v1.pdf) | [![GitHub](https://img.shields.io/github/stars/Hectormxy/CineCap.git?style=social)](https://github.com/Hectormxy/CineCap.git)  
  Keywords: video generation, concept, film, dit, evaluation, benchmark, controllable  

### Architecture & Efficiency

*Showing the latest 50 out of 364 papers*

- **[OrbitQuant: Data-Agnostic Quantization for Image and Video Diffusion Transformers](https://arxiv.org/abs/2607.02461v1)**  
  Authors: Donghyun Lee, Jitesh Chavan, Duy Nguyen, Sam Huang, Liming Jiang, Priyadarshini Panda, Timo Mertens, Saurabh Shukla  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.02461v1.pdf)  
  Keywords: diffusion transformer, video diffusion, video generation, image to video, dit  
- **[NEvo: Neural-Guided Evolutionary Video Synthesis for Dynamic Visual Selectivity](https://arxiv.org/abs/2607.02317v1)**  
  Authors: Yingtian Tang, Sogand Salehi, Ming Zhou, Amir Zamir, Leyla Isik, Martin Schrimpf  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.02317v1.pdf)  
  Keywords: video synthesis, dynamics, efficient  
- **[NeoMap: Training-free Novel-View Synthesis from Single Images and Videos](https://arxiv.org/abs/2607.01962v1)**  
  Authors: Jinxi Li, Tianyi Zhang, Yafei Yang, Zihui Zhang, Peng Huang, Koon Wing Macgyver Lin, Bo Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.01962v1.pdf)  
  Keywords: video synthesis, novel view, denoising, dit, benchmark  
- **[QWERTY: Training-Free Motion Control via Query-Warped Video Diffusion Transformers](https://arxiv.org/abs/2607.01869v1)**  
  Authors: Kyobin Choo, Youngmin Kim, Hyunkyung Han, Geunrip Park, Chanyoung Kim, Sunyoung Jung, Seong Jae Hwang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.01869v1.pdf)  
  Keywords: diffusion model, video diffusion, diffusion transformer, image-to-video, trajectory, dit, motion control  
- **[SimWorlds: A Multi-Agent System for Dynamic 3D Scene Creation](https://arxiv.org/abs/2607.01766v1)**  
  Authors: Chunjiang Liu, Xiaoyuan Wang, Haoyu Chen, Yizhou Zhao, Ming-Hsuan Yang, László A. Jeni  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.01766v1.pdf)  
  Keywords: video generation, layout, physical, physics, dit, benchmark  
- **[ICDepth: Taming Video Diffusion Models for Video Depth Estimation via In-Context Conditioning](https://arxiv.org/abs/2607.01677v1)**  
  Authors: Xuanhua He, Jiaxin Xie, Mingzhe Zheng, Qifeng Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.01677v1.pdf)  
  Keywords: diffusion model, video diffusion, diffusion transformer, text-to-video, temporal consistency, dit, benchmark  
- **[Unified Panoramic-Gaussian Representation for Monocular 4D Scene Synthesis](https://arxiv.org/abs/2607.01663v1)**  
  Authors: Yuankun Yang, Yi Wei, Wenyang Zhou, Li Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.01663v1.pdf)  
  Keywords: dit, physical, video generation, trajectory  
- **[Anti-Prompt: Image Protection against Text-Guided Image-to-Video Generation](https://arxiv.org/abs/2607.01499v1)**  
  Authors: Yeonghwan Song, Chanhui Lee, Jinsoo Park, Jeany Son  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.01499v1.pdf)  
  Keywords: video generation, architecture, temporal consistency, i2v, image-to-video, denoising, dit, evaluation  
- **[Ink3D: Sculpting 3D Assets with Extremely Complex Textures via Video Generative Models](https://arxiv.org/abs/2607.01222v1)**  
  Authors: Yue Han, Chong Li, Zhening Liu, Cong Huang, Fang Deng, Yong Liu, Fangyun Wei, Yan Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.01222v1.pdf)  
  Keywords: dit, video generation  
- **[Dataset Biases and Shortcut Learning in Motion-Based AI-Generated Video Detection](https://arxiv.org/abs/2607.00948v1)**  
  Authors: Joren Michels, Lode Jorissen, Nick Michiels  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.00948v1.pdf)  
  Keywords: dit, evaluation  

### Audio & Multi-modal

- **[AVTok: 1D Unified Tokenization for Holistic Audio-Video Generation](https://arxiv.org/abs/2606.30811v1)**  
  Authors: Kien T. Pham, I Chieh Chen, Qifeng Chen, Long Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.30811v1.pdf)  
  Keywords: video generation, audio-to-video, sound, architecture, efficient, dit  
- **[TRUST: Efficient Abdominal Trauma Recognition via Image-to-Ultrasound-Video Transfer Learning](https://arxiv.org/abs/2606.27777v1)**  
  Authors: Enguang Wang, Hao Zhou, Shuo Gao, Tuo Liu, Guangquan Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.27777v1.pdf)  
  Keywords: dynamics, sound, efficient, image-to-video, dit  
- **[PhyEditBench: A Real-World Multi-Stage Benchmark for Physics-Aware Image Editing](https://arxiv.org/abs/2606.26551v2)**  
  Authors: Shengbin Guo, Shaokang He, Chaoyue Meng, Shengpeng Xiao, Xunzhi Xiang, Shaofeng Zhang, Qi Fan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.26551v2.pdf) | [![GitHub](https://img.shields.io/github/stars/Previsior/PhyEditBench?style=social)](https://github.com/Previsior/PhyEditBench)  
  Keywords: video generation, physical, dynamics, physics-aware, multi-modal, physics, dit, evaluation, benchmark  
- **[Wan-Streamer v0.1: End-to-end Real-time Interactive Foundation Models](https://arxiv.org/abs/2606.25041v3)**  
  Authors: Lianghua Huang, Zhi-Fan Wu, Wei Wang, Yupeng Shi, Mengyang Feng, Junjie He, Chen-Wei Xie, Yu Liu, Jingren Zhou, Ang Wang, Bang Zhang, Baole Ai, Chen Liang, Cheng Yu, Chongyang Zhong, Jinwei Qi, Kai Zhu, Pandeng Li, Peng Zhang, Wenyuan Zhang, Xinhua Cheng, Yitong Huang, Yun Zheng, Yuzheng Wang, Zoubin Bi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.25041v3.pdf)  
  Keywords: streaming, audio-driven, interactive, avatar  
- **[InteractiveAvatar: Real-Time Streaming Video Generation for Consistent and Intent-Aware Avatars](https://arxiv.org/abs/2606.22905v2)**  
  Authors: Quanyue Song, Yishan He, Yanfei Zhang, Shihao Cheng, Zhixiang He, Zhizhi Guo, Chi Zhang, Xuelong Li, Caigui Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.22905v2.pdf)  
  Keywords: video generation, avatar, temporal consistency, streaming, audio-driven, distillation, interactive, autoregressive  
- **[T-MOR: Learning Motion-Aware Skeleton Representations for Human Action Recognition](https://arxiv.org/abs/2606.21607v1)**  
  Authors: Di Yang, Mahmoud Ali, Quan Kong, Gianpiero Francesca, Francois Bremond  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.21607v1.pdf)  
  Keywords: physical, human motion, multi-modal, dit, benchmark  
- **[PermaVid: Consistent Video Generation Across Edits via Disentangled Context Memory](https://arxiv.org/abs/2606.16449v2)**  
  Authors: Shuai Yang, Bingjie Gao, Ziwei Liu, Jiaqi Wang, Dahua Lin, Tong Wu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16449v2.pdf)  
  Keywords: dit, video generation, layout, multi-modal  
- **[ReFree: Towards Realistic Co-Speech Video Generation via Reward-Free RL and Multilevel Speech Guidance](https://arxiv.org/abs/2606.13304v1)**  
  Authors: Salaheldin Mohamed, M. Hamza Mughal, Rishabh Dabral, Christian Theobalt  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13304v1.pdf)  
  Keywords: evaluation, video generation, speech-driven  
- **[MSUE: Multi-Modal Soccer Understanding Expert](https://arxiv.org/abs/2606.12106v1)**  
  Authors: Litao Li, Yibo Yu, Yufeng Hu, Zhuo Yang, Jiali Wen, Yixin Chen, Yixi Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.12106v1.pdf)  
  Keywords: architecture, long-form, multi-modal, benchmark  
- **[Conan-embedding-v3: Fusing Modality-Specific Models for Omni-Modal Embedding](https://arxiv.org/abs/2606.09331v1)**  
  Authors: Shiyu Li, Zhiyuan Hu, Yifan Wang, Peiming Li, Zheng Wei, Yang Tang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.09331v1.pdf)  
  Keywords: architecture, multi-modal, dynamics  

### Controllable Generation

*Showing the latest 50 out of 141 papers*

- **[WorldDirector: Building Controllable World Simulators with Persistent Dynamic Memory](https://arxiv.org/abs/2607.02517v1)**  
  Authors: Hanlin Wang, Hao Ouyang, Qiuyu Wang, Wen Wang, Qingyan Bai, Ka Leong Cheng, Yue Yu, Yixuan Li, Yihao Meng, Zichen Liu, Yanhong Zeng, Yujun Shen, Qifeng Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.02517v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://worlddirector.github.io)  
  Keywords: video generation, physical, dynamics, world model, world simulator, controllable  
- **[QWERTY: Training-Free Motion Control via Query-Warped Video Diffusion Transformers](https://arxiv.org/abs/2607.01869v1)**  
  Authors: Kyobin Choo, Youngmin Kim, Hyunkyung Han, Geunrip Park, Chanyoung Kim, Sunyoung Jung, Seong Jae Hwang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.01869v1.pdf)  
  Keywords: diffusion model, video diffusion, diffusion transformer, image-to-video, trajectory, dit, motion control  
- **[SimWorlds: A Multi-Agent System for Dynamic 3D Scene Creation](https://arxiv.org/abs/2607.01766v1)**  
  Authors: Chunjiang Liu, Xiaoyuan Wang, Haoyu Chen, Yizhou Zhao, Ming-Hsuan Yang, László A. Jeni  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.01766v1.pdf)  
  Keywords: video generation, layout, physical, physics, dit, benchmark  
- **[Unified Panoramic-Gaussian Representation for Monocular 4D Scene Synthesis](https://arxiv.org/abs/2607.01663v1)**  
  Authors: Yuankun Yang, Yi Wei, Wenyang Zhou, Li Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.01663v1.pdf)  
  Keywords: dit, physical, video generation, trajectory  
- **[TrajLoc: Trajectory-Attention Localization for Multi-Object Motion Control](https://arxiv.org/abs/2607.00861v1)**  
  Authors: Omer Sela, Inbar Huberman-Spiegelglas, Michael Rotman, Sagie Benaim, Avi Ben-Cohen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.00861v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://sela-omer.github.io/traj-loc)  
  Keywords: identity, i2v, image-to-video, trajectory, dit, evaluation, motion control  
- **[Pano2World: End-to-End 3D Generation via Unified Multi-View Sequences](https://arxiv.org/abs/2607.00832v1)**  
  Authors: Zhenjia Li, Jinrang Jia, Yifeng Shi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.00832v1.pdf)  
  Keywords: diffusion model, video generation, temporal consistency, denoising, trajectory, benchmark  
- **[World Narrative Model for Highly Controllable Video Generation: A Paradigm Shift from Pixel Sampling to Physical World Orchestration](https://arxiv.org/abs/2606.31946v1)**  
  Authors: Ye Chen, Xuanhong Chen, Yupeng Zhu, Liming Tan, Zhewen Wan, Yuxuan Xiong, Tielong Wang, Jinfan Liu, Wuze Zhang, Xiongzhen Zhang, Feifei Li, Xianglin Luo, Zhehan Zhao, Zhifan Zhang, Laisheng Kou, Zhujing Liang, Yugang Chen, Muchun Chen, Xu Miao, Yijing Zhang, Xiaojie Sheng, Qiang Hu, Jialiang Chen, Weimin Zhang, Wenjun Zhang, Bingbing Ni  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.31946v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://glassroom.sjtu.edu.cn/WNM)  
  Keywords: video generation, layout, physical, efficient, film, dit, controllable  
- **[InfiniVerse: Occupancy Guided Unbounded Scene Generation for Autonomous Driving](https://arxiv.org/abs/2606.31109v1)**  
  Authors: Xiaoyu Ye, Leheng Li, Xinyu Ji, Yingjie Cai, Hongda He, Xu Yan, Guanyi Zhao, Ying-Cong Chen, Bingbing Liu, Shuguang Cui, Zhen Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.31109v1.pdf)  
  Keywords: diffusion model, video diffusion, autonomous driving, dit, evaluation, autoregressive, benchmark, controllable  
- **[3D Scene-Adaptive Trajectory-Controllable Human Image Animation with Camera Movement](https://arxiv.org/abs/2606.30514v2)**  
  Authors: Deyin Liu, Jicheng Xu, Lin Yuanbo Wu, Xiaowei Zhao, Xiatian Zhu, Zhe Jin, Anjan Dutta  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.30514v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://robinhood256100.github.io/web-disp)  
  Keywords: video generation, human motion, image animation, trajectory, camera control, dit, benchmark, controllable  
- **[HorizonRelight: Relighting Long-horizon Videos Consistently via Diffusion Transformers](https://arxiv.org/abs/2606.29095v1)**  
  Authors: Jing Yang, Mayoore Jaiswal, Zian Wang, Steven Zeng, Rochelle Pereira, Yajie Zhao, Jianyuan Min  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.29095v1.pdf)  
  Keywords: diffusion transformer, video diffusion, temporal consistency, dit, controllable  

### Human & Character Animation

- **[3D Scene-Adaptive Trajectory-Controllable Human Image Animation with Camera Movement](https://arxiv.org/abs/2606.30514v2)**  
  Authors: Deyin Liu, Jicheng Xu, Lin Yuanbo Wu, Xiaowei Zhao, Xiatian Zhu, Zhe Jin, Anjan Dutta  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.30514v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://robinhood256100.github.io/web-disp)  
  Keywords: video generation, human motion, image animation, trajectory, camera control, dit, benchmark, controllable  
- **[OmniDance: Multimodal Driven Dance Video Generation with Large-scale Internet Data](https://arxiv.org/abs/2606.30019v1)**  
  Authors: Kaixing Yang, Jiashu Zhu, Xulong Tang, Ziqiao Peng, Xiangyue Zhang, Chubin Chen, Puwei Wang, Jiahong Wu, Xiangxiang Chu, Hongyan Liu, Jun He  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.30019v1.pdf) | [![GitHub](https://img.shields.io/github/stars/AMAP-ML/OmniDance?style=social)](https://github.com/AMAP-ML/OmniDance)  
  Keywords: video generation, dynamics, architecture, human motion, i2v, dit  
- **[EMOSH: Expressive Motion and Shape Disentanglement for Human Animation](https://arxiv.org/abs/2606.28026v1)**  
  Authors: Dongbin Zhang, Hao Liu, Binquan Dai, Kangjie Chen, Chuming Wang, Chen Li, Jing Lyu, Haoqian Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.28026v1.pdf)  
  Keywords: video generation, identity, avatar, human animation, gesture, dit, controllable  
- **[Directing the World: Fast Autoregressive Video Generation with Compositional Human-Camera Control](https://arxiv.org/abs/2606.27964v1)**  
  Authors: Haoyuan Wang, Yabo Chen, Haibin Huang, Chi Zhang, Xuelong Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.27964v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://whydahuzi.github.io/Directing-the-World.github.io)  
  Keywords: video generation, dynamics, world model, human motion, autoregressive, trajectory, interactive, camera control, motion control, controllable  
- **[Follow Your Track: Precise Skeleton Animation Controlled by 3D Trajectories](https://arxiv.org/abs/2606.25344v1)**  
  Authors: Yueting Liu, Yanqin Jiang, Nian Liu, Jingmen Zhou, Zhengjun Zha, Weiming Hu, Jin Gao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.25344v1.pdf)  
  Keywords: body motion, efficient, temporal consistency, 4d generation, trajectory, dit  
- **[Wan-Streamer v0.1: End-to-end Real-time Interactive Foundation Models](https://arxiv.org/abs/2606.25041v3)**  
  Authors: Lianghua Huang, Zhi-Fan Wu, Wei Wang, Yupeng Shi, Mengyang Feng, Junjie He, Chen-Wei Xie, Yu Liu, Jingren Zhou, Ang Wang, Bang Zhang, Baole Ai, Chen Liang, Cheng Yu, Chongyang Zhong, Jinwei Qi, Kai Zhu, Pandeng Li, Peng Zhang, Wenyuan Zhang, Xinhua Cheng, Yitong Huang, Yun Zheng, Yuzheng Wang, Zoubin Bi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.25041v3.pdf)  
  Keywords: streaming, audio-driven, interactive, avatar  
- **[InteractiveAvatar: Real-Time Streaming Video Generation for Consistent and Intent-Aware Avatars](https://arxiv.org/abs/2606.22905v2)**  
  Authors: Quanyue Song, Yishan He, Yanfei Zhang, Shihao Cheng, Zhixiang He, Zhizhi Guo, Chi Zhang, Xuelong Li, Caigui Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.22905v2.pdf)  
  Keywords: video generation, avatar, temporal consistency, streaming, audio-driven, distillation, interactive, autoregressive  
- **[Generative Relightable Avatars](https://arxiv.org/abs/2606.22718v1)**  
  Authors: Kunwar Maheep Singh, Christian Theobalt, Rishabh Dabral  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.22718v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://vcai.mpi-inf.mpg.de/projects/GRA)  
  Keywords: diffusion model, video diffusion, physical, dynamics, avatar, video-to-video, physics, long video, evaluation, controllable  
- **[T-MOR: Learning Motion-Aware Skeleton Representations for Human Action Recognition](https://arxiv.org/abs/2606.21607v1)**  
  Authors: Di Yang, Mahmoud Ali, Quan Kong, Gianpiero Francesca, Francois Bremond  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.21607v1.pdf)  
  Keywords: physical, human motion, multi-modal, dit, benchmark  
- **[Avatar V: Scaling Video-Reference Avatar Video Generation](https://arxiv.org/abs/2606.13872v1)**  
  Authors: Benjamin Liang, Ce Chen, Desmond Lin, Ivan Somov, Jiajun Zhao, Jiewei Yuan, Jingfeng Zhang, Junhao Huang, Nik Nolte, Pedram Haqiqi, Penghan Wang, Rong Yan, Rui Zhang, Sam Prokopchuk, Sivan Wang, Viktor Goriachko, Yi Ren, Yuanming Li, Yutao Chen, Zhenhui Ye, Zhibin Hong, Zilong Nie, Zujin Guo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13872v1.pdf)  
  Keywords: video generation, dynamics, acceleration, identity, avatar, style, flow matching, distillation, dit, super-resolution, evaluation, benchmark  

### Image-to-Video Generation

- **[OrbitQuant: Data-Agnostic Quantization for Image and Video Diffusion Transformers](https://arxiv.org/abs/2607.02461v1)**  
  Authors: Donghyun Lee, Jitesh Chavan, Duy Nguyen, Sam Huang, Liming Jiang, Priyadarshini Panda, Timo Mertens, Saurabh Shukla  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.02461v1.pdf)  
  Keywords: diffusion transformer, video diffusion, video generation, image to video, dit  
- **[QWERTY: Training-Free Motion Control via Query-Warped Video Diffusion Transformers](https://arxiv.org/abs/2607.01869v1)**  
  Authors: Kyobin Choo, Youngmin Kim, Hyunkyung Han, Geunrip Park, Chanyoung Kim, Sunyoung Jung, Seong Jae Hwang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.01869v1.pdf)  
  Keywords: diffusion model, video diffusion, diffusion transformer, image-to-video, trajectory, dit, motion control  
- **[Anti-Prompt: Image Protection against Text-Guided Image-to-Video Generation](https://arxiv.org/abs/2607.01499v1)**  
  Authors: Yeonghwan Song, Chanhui Lee, Jinsoo Park, Jeany Son  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.01499v1.pdf)  
  Keywords: video generation, architecture, temporal consistency, i2v, image-to-video, denoising, dit, evaluation  
- **[TrajLoc: Trajectory-Attention Localization for Multi-Object Motion Control](https://arxiv.org/abs/2607.00861v1)**  
  Authors: Omer Sela, Inbar Huberman-Spiegelglas, Michael Rotman, Sagie Benaim, Avi Ben-Cohen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.00861v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://sela-omer.github.io/traj-loc)  
  Keywords: identity, i2v, image-to-video, trajectory, dit, evaluation, motion control  
- **[3D Scene-Adaptive Trajectory-Controllable Human Image Animation with Camera Movement](https://arxiv.org/abs/2606.30514v2)**  
  Authors: Deyin Liu, Jicheng Xu, Lin Yuanbo Wu, Xiaowei Zhao, Xiatian Zhu, Zhe Jin, Anjan Dutta  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.30514v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://robinhood256100.github.io/web-disp)  
  Keywords: video generation, human motion, image animation, trajectory, camera control, dit, benchmark, controllable  
- **[OmniDance: Multimodal Driven Dance Video Generation with Large-scale Internet Data](https://arxiv.org/abs/2606.30019v1)**  
  Authors: Kaixing Yang, Jiashu Zhu, Xulong Tang, Ziqiao Peng, Xiangyue Zhang, Chubin Chen, Puwei Wang, Jiahong Wu, Xiangxiang Chu, Hongyan Liu, Jun He  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.30019v1.pdf) | [![GitHub](https://img.shields.io/github/stars/AMAP-ML/OmniDance?style=social)](https://github.com/AMAP-ML/OmniDance)  
  Keywords: video generation, dynamics, architecture, human motion, i2v, dit  
- **[PhysisForcing: Physics Reinforced World Simulator for Robotic Manipulation](https://arxiv.org/abs/2606.28128v1)**  
  Authors: Peiwen Zhang, Yufan Deng, Shangkun Sun, Juncheng Ma, Duomin Wang, Jonas Du, Zilin Pan, Ye Huang, Hao Liang, Songyan Huang, Ruihua Zhang, Enze Xie, Ming-Yu Liu, Daquan Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.28128v1.pdf)  
  Keywords: video generation, physical, world model, i2v, simulation, physics, trajectory, world simulator, dit  
- **[TRUST: Efficient Abdominal Trauma Recognition via Image-to-Ultrasound-Video Transfer Learning](https://arxiv.org/abs/2606.27777v1)**  
  Authors: Enguang Wang, Hao Zhou, Shuo Gao, Tuo Liu, Guangquan Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.27777v1.pdf)  
  Keywords: dynamics, sound, efficient, image-to-video, dit  
- **[VPA-Guard: Defending and Benchmarking Image-to-Video Generation Against Visual Prompt Attacks](https://arxiv.org/abs/2606.25592v1)**  
  Authors: Yining Sun, Haoyu Kang, Jiajun Wu, Heng Zhang, Danyang Zhang, Zhenjun Zhao, Haochen Han, Fangming Liu, Wai Kin Victor Chan, Alex Jinpeng Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.25592v1.pdf)  
  Keywords: video generation, dynamics, i2v, image-to-video, interactive, dit, benchmark  
- **[Chorus II: Cross-Request Sparsity Reuse for Efficient Image-to-Video Generation](https://arxiv.org/abs/2606.25040v1)**  
  Authors: Hao Liu, Chenghuan Huang, Hao Liu, Xing Cai, Chen Li, Ziyang Ma, Jing Lyu, Nong Xiao, Jiangsu Du  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.25040v1.pdf)  
  Keywords: diffusion model, video generation, layout, efficient, i2v, image-to-video, dit, acceleration  

### Long Video Generation

*Showing the latest 50 out of 134 papers*

- **[ICDepth: Taming Video Diffusion Models for Video Depth Estimation via In-Context Conditioning](https://arxiv.org/abs/2607.01677v1)**  
  Authors: Xuanhua He, Jiaxin Xie, Mingzhe Zheng, Qifeng Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.01677v1.pdf)  
  Keywords: diffusion model, video diffusion, diffusion transformer, text-to-video, temporal consistency, dit, benchmark  
- **[Anti-Prompt: Image Protection against Text-Guided Image-to-Video Generation](https://arxiv.org/abs/2607.01499v1)**  
  Authors: Yeonghwan Song, Chanhui Lee, Jinsoo Park, Jeany Son  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.01499v1.pdf)  
  Keywords: video generation, architecture, temporal consistency, i2v, image-to-video, denoising, dit, evaluation  
- **[Pano2World: End-to-End 3D Generation via Unified Multi-View Sequences](https://arxiv.org/abs/2607.00832v1)**  
  Authors: Zhenjia Li, Jinrang Jia, Yifeng Shi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.00832v1.pdf)  
  Keywords: diffusion model, video generation, temporal consistency, denoising, trajectory, benchmark  
- **[Towards Memory-Efficient Autoregressive Video Generation via Instance-Specific Parametric Absorption](https://arxiv.org/abs/2607.00712v1)**  
  Authors: Xiaomeng Fu, Jia Li, Yiming Hu, Yong Wang, Hayden Kwok-Hay So, Jiao Dai, Xiangxiang Chu, Jizhong Han  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.00712v1.pdf)  
  Keywords: video generation, identity, architecture, efficient, streaming, long video, autoregressive  
- **[MemLearner: Learning to Query Context memory for Video World Models](https://arxiv.org/abs/2606.31734v1)**  
  Authors: Jiwen Yu, Jianxiong Gao, Jianhong Bai, Yiran Qin, Kaiyi Huang, Quande Liu, Xintao Wang, Pengfei Wan, Kun Gai, Xihui Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.31734v1.pdf)  
  Keywords: video generation, world model, efficient, long video, interactive, dit  
- **[Bridging Video Understanding and Generation in a Unified Framework](https://arxiv.org/abs/2606.31326v1)**  
  Authors: Yuqi Wang, Runyi Li, Ruoyu Feng, Renjie Chen, Wenfeng Lin, Mingyu Guo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.31326v1.pdf)  
  Keywords: video generation, dynamics, architecture, autoregressive, benchmark  
- **[InfiniVerse: Occupancy Guided Unbounded Scene Generation for Autonomous Driving](https://arxiv.org/abs/2606.31109v1)**  
  Authors: Xiaoyu Ye, Leheng Li, Xinyu Ji, Yingjie Cai, Hongda He, Xu Yan, Guanyi Zhao, Ying-Cong Chen, Bingbing Liu, Shuguang Cui, Zhen Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.31109v1.pdf)  
  Keywords: diffusion model, video diffusion, autonomous driving, dit, evaluation, autoregressive, benchmark, controllable  
- **[HorizonRelight: Relighting Long-horizon Videos Consistently via Diffusion Transformers](https://arxiv.org/abs/2606.29095v1)**  
  Authors: Jing Yang, Mayoore Jaiswal, Zian Wang, Steven Zeng, Rochelle Pereira, Yajie Zhao, Jianyuan Min  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.29095v1.pdf)  
  Keywords: diffusion transformer, video diffusion, temporal consistency, dit, controllable  
- **[TempAct: Advancing Temporal Plausibility in Autoregressive Video Generation via Planner-Executor RL](https://arxiv.org/abs/2606.28016v2)**  
  Authors: Jing Wang, Xiangxin Zhou, Jiajun Liang, Kaiqi Liu, Wanyuan Pang, Zhenyu Xie, Tianyu Pang, Xiaodan Liang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.28016v2.pdf)  
  Keywords: diffusion model, video diffusion, video generation, temporal consistency, streaming, denoising, distillation, dit, autoregressive  
- **[Directing the World: Fast Autoregressive Video Generation with Compositional Human-Camera Control](https://arxiv.org/abs/2606.27964v1)**  
  Authors: Haoyuan Wang, Yabo Chen, Haibin Huang, Chi Zhang, Xuelong Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.27964v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://whydahuzi.github.io/Directing-the-World.github.io)  
  Keywords: video generation, dynamics, world model, human motion, autoregressive, trajectory, interactive, camera control, motion control, controllable  

### Personalization & Customization

*Showing the latest 50 out of 89 papers*

- **[TrajLoc: Trajectory-Attention Localization for Multi-Object Motion Control](https://arxiv.org/abs/2607.00861v1)**  
  Authors: Omer Sela, Inbar Huberman-Spiegelglas, Michael Rotman, Sagie Benaim, Avi Ben-Cohen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.00861v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://sela-omer.github.io/traj-loc)  
  Keywords: identity, i2v, image-to-video, trajectory, dit, evaluation, motion control  
- **[Towards Memory-Efficient Autoregressive Video Generation via Instance-Specific Parametric Absorption](https://arxiv.org/abs/2607.00712v1)**  
  Authors: Xiaomeng Fu, Jia Li, Yiming Hu, Yong Wang, Hayden Kwok-Hay So, Jiao Dai, Xiangxiang Chu, Jizhong Han  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.00712v1.pdf)  
  Keywords: video generation, identity, architecture, efficient, streaming, long video, autoregressive  
- **[GeoEdit: Geometry-Aware Object Editing via Dual-Branch Denoising](https://arxiv.org/abs/2606.30003v1)**  
  Authors: Yi He, Jiangming Wang, Xinyu Wang, Mark Fong, Songchun Zhang, Yuxuan Xue, Hai-Tao Zheng, Yue Ma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.30003v1.pdf) | [![GitHub](https://img.shields.io/github/stars/Heey731/GeoEdit?style=social)](https://github.com/Heey731/GeoEdit)  
  Keywords: video diffusion, physical, identity, denoising, dit, evaluation, benchmark  
- **[Semantic-Aware, Physics-Informed, Geometry-Grounded Weather Video Synthesis](https://arxiv.org/abs/2606.29020v1)**  
  Authors: Chenghao Qian, Nedko Savov, Lingdong Kong, Yeying Jin, Rui Song, Wenjing Li, Zhun Zhong, Jiaqi Ma, Gustav Markkula, Luc Van Gool  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.29020v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://jumponthemoon.github.io/w-crafter)  
  Keywords: dynamics, physical, identity, video synthesis, autonomous driving, simulation, physics, dit  
- **[A Good Talk Does not Look Like a Summary, It Teaches You! Measuring Takeaways from Paper-to-Video Talks](https://arxiv.org/abs/2606.28531v1)**  
  Authors: Ishani Mondal, Aparna Garimella, Ananya Sai, Pannaga Shivaswamy, Jordan Boyd-Graber  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.28531v1.pdf)  
  Keywords: evaluation, video generation, concept, education  
- **[EMOSH: Expressive Motion and Shape Disentanglement for Human Animation](https://arxiv.org/abs/2606.28026v1)**  
  Authors: Dongbin Zhang, Hao Liu, Binquan Dai, Kangjie Chen, Chuming Wang, Chen Li, Jing Lyu, Haoqian Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.28026v1.pdf)  
  Keywords: video generation, identity, avatar, human animation, gesture, dit, controllable  
- **[RayPE: Ray-Space Positional Encoding for 3D-Aware Video Generation](https://arxiv.org/abs/2606.27345v2)**  
  Authors: Minghao Yin, Jiahao Lu, Wenbo Hu, Wang Zhao, Shan Ying, Kai Han  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.27345v2.pdf)  
  Keywords: diffusion transformer, video diffusion, video generation, identity, 3d-aware, camera control, dit  
- **[NaviCache: Test-Time Self-Calibration Caching for Video Generation](https://arxiv.org/abs/2606.26795v1)**  
  Authors: Zheqi Lv, Zhibo Zhu, Jinke Wang, Qi Tian, Shengyu Zhang, Zhengyu Chen, Chengxi Zang, Zhou Zhao, Fei Wu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.26795v1.pdf)  
  Keywords: diffusion model, video diffusion, video generation, architecture, concept, trajectory, acceleration  
- **[Disco-LoRA: Disentangled Composition of Content, Style, and Motion for Multi-concept Video Customization](https://arxiv.org/abs/2606.26668v1)**  
  Authors: Xuancheng Xu, Gengyun Jia, Bing-Kun Bao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.26668v1.pdf)  
  Keywords: video generation, identity, text-to-video, style, concept, t2v, customization, benchmark, controllable  
- **[DomainShuttle: Freeform Open Domain Subject-driven Text-to-video Generation](https://arxiv.org/abs/2606.26058v1)**  
  Authors: Nan Chen, Yiyang Cai, Rongchang Xie, Junwen Pan, Cheng Chen, Weinan Jia, Zhuowei Chen, Wen Zhou, Zhenbang Sun, Wenhan Luo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.26058v1.pdf)  
  Keywords: video generation, text-to-video, style, dit, personalization, subject-driven  

### Physical Understanding

*Showing the latest 50 out of 154 papers*

- **[WorldDirector: Building Controllable World Simulators with Persistent Dynamic Memory](https://arxiv.org/abs/2607.02517v1)**  
  Authors: Hanlin Wang, Hao Ouyang, Qiuyu Wang, Wen Wang, Qingyan Bai, Ka Leong Cheng, Yue Yu, Yixuan Li, Yihao Meng, Zichen Liu, Yanhong Zeng, Yujun Shen, Qifeng Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.02517v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://worlddirector.github.io)  
  Keywords: video generation, physical, dynamics, world model, world simulator, controllable  
- **[NEvo: Neural-Guided Evolutionary Video Synthesis for Dynamic Visual Selectivity](https://arxiv.org/abs/2607.02317v1)**  
  Authors: Yingtian Tang, Sogand Salehi, Ming Zhou, Amir Zamir, Leyla Isik, Martin Schrimpf  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.02317v1.pdf)  
  Keywords: video synthesis, dynamics, efficient  
- **[SimWorlds: A Multi-Agent System for Dynamic 3D Scene Creation](https://arxiv.org/abs/2607.01766v1)**  
  Authors: Chunjiang Liu, Xiaoyuan Wang, Haoyu Chen, Yizhou Zhao, Ming-Hsuan Yang, László A. Jeni  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.01766v1.pdf)  
  Keywords: video generation, layout, physical, physics, dit, benchmark  
- **[Unified Panoramic-Gaussian Representation for Monocular 4D Scene Synthesis](https://arxiv.org/abs/2607.01663v1)**  
  Authors: Yuankun Yang, Yi Wei, Wenyang Zhou, Li Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.01663v1.pdf)  
  Keywords: dit, physical, video generation, trajectory  
- **[World Narrative Model for Highly Controllable Video Generation: A Paradigm Shift from Pixel Sampling to Physical World Orchestration](https://arxiv.org/abs/2606.31946v1)**  
  Authors: Ye Chen, Xuanhong Chen, Yupeng Zhu, Liming Tan, Zhewen Wan, Yuxuan Xiong, Tielong Wang, Jinfan Liu, Wuze Zhang, Xiongzhen Zhang, Feifei Li, Xianglin Luo, Zhehan Zhao, Zhifan Zhang, Laisheng Kou, Zhujing Liang, Yugang Chen, Muchun Chen, Xu Miao, Yijing Zhang, Xiaojie Sheng, Qiang Hu, Jialiang Chen, Weimin Zhang, Wenjun Zhang, Bingbing Ni  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.31946v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://glassroom.sjtu.edu.cn/WNM)  
  Keywords: video generation, layout, physical, efficient, film, dit, controllable  
- **[Bridging Video Understanding and Generation in a Unified Framework](https://arxiv.org/abs/2606.31326v1)**  
  Authors: Yuqi Wang, Runyi Li, Ruoyu Feng, Renjie Chen, Wenfeng Lin, Mingyu Guo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.31326v1.pdf)  
  Keywords: video generation, dynamics, architecture, autoregressive, benchmark  
- **[EcoVideo: Entropy-Orchestrated Video Generation Paradigm in Cloud-Edge Dynamics](https://arxiv.org/abs/2606.30557v1)**  
  Authors: Jiayu Chen, Hengyi Zhang, Maoliang Li, Minyu Li, Zihao Zheng, Xuanzhe Liu, Guojie Luo, Xiang Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.30557v1.pdf) | [![GitHub](https://img.shields.io/github/stars/IF-LAB-PKU/EcoVideo?style=social)](https://github.com/IF-LAB-PKU/EcoVideo)  
  Keywords: dit, denoising, video generation, dynamics  
- **[The Surprising Effectiveness of Video Diffusion Models for Hand Motion Reconstruction](https://arxiv.org/abs/2606.30308v1)**  
  Authors: Yuxi Wang, Chengkai Jin, Yufei Liu, Wenqi Ouyang, Tianyi Wei, Zhiwei Zeng, Siyuan Huang, Zhiqi Shen, Xingang Pan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.30308v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://vidihand.github.io)  
  Keywords: diffusion model, video diffusion, dynamics  
- **[OmniDance: Multimodal Driven Dance Video Generation with Large-scale Internet Data](https://arxiv.org/abs/2606.30019v1)**  
  Authors: Kaixing Yang, Jiashu Zhu, Xulong Tang, Ziqiao Peng, Xiangyue Zhang, Chubin Chen, Puwei Wang, Jiahong Wu, Xiangxiang Chu, Hongyan Liu, Jun He  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.30019v1.pdf) | [![GitHub](https://img.shields.io/github/stars/AMAP-ML/OmniDance?style=social)](https://github.com/AMAP-ML/OmniDance)  
  Keywords: video generation, dynamics, architecture, human motion, i2v, dit  
- **[GeoEdit: Geometry-Aware Object Editing via Dual-Branch Denoising](https://arxiv.org/abs/2606.30003v1)**  
  Authors: Yi He, Jiangming Wang, Xinyu Wang, Mark Fong, Songchun Zhang, Yuxuan Xue, Hai-Tao Zheng, Yue Ma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.30003v1.pdf) | [![GitHub](https://img.shields.io/github/stars/Heey731/GeoEdit?style=social)](https://github.com/Heey731/GeoEdit)  
  Keywords: video diffusion, physical, identity, denoising, dit, evaluation, benchmark  

### Surveys & Benchmarks

*Showing the latest 50 out of 235 papers*

- **[NeoMap: Training-free Novel-View Synthesis from Single Images and Videos](https://arxiv.org/abs/2607.01962v1)**  
  Authors: Jinxi Li, Tianyi Zhang, Yafei Yang, Zihui Zhang, Peng Huang, Koon Wing Macgyver Lin, Bo Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.01962v1.pdf)  
  Keywords: video synthesis, novel view, denoising, dit, benchmark  
- **[SimWorlds: A Multi-Agent System for Dynamic 3D Scene Creation](https://arxiv.org/abs/2607.01766v1)**  
  Authors: Chunjiang Liu, Xiaoyuan Wang, Haoyu Chen, Yizhou Zhao, Ming-Hsuan Yang, László A. Jeni  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.01766v1.pdf)  
  Keywords: video generation, layout, physical, physics, dit, benchmark  
- **[ICDepth: Taming Video Diffusion Models for Video Depth Estimation via In-Context Conditioning](https://arxiv.org/abs/2607.01677v1)**  
  Authors: Xuanhua He, Jiaxin Xie, Mingzhe Zheng, Qifeng Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.01677v1.pdf)  
  Keywords: diffusion model, video diffusion, diffusion transformer, text-to-video, temporal consistency, dit, benchmark  
- **[Anti-Prompt: Image Protection against Text-Guided Image-to-Video Generation](https://arxiv.org/abs/2607.01499v1)**  
  Authors: Yeonghwan Song, Chanhui Lee, Jinsoo Park, Jeany Son  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.01499v1.pdf)  
  Keywords: video generation, architecture, temporal consistency, i2v, image-to-video, denoising, dit, evaluation  
- **[Dataset Biases and Shortcut Learning in Motion-Based AI-Generated Video Detection](https://arxiv.org/abs/2607.00948v1)**  
  Authors: Joren Michels, Lode Jorissen, Nick Michiels  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.00948v1.pdf)  
  Keywords: dit, evaluation  
- **[TrajLoc: Trajectory-Attention Localization for Multi-Object Motion Control](https://arxiv.org/abs/2607.00861v1)**  
  Authors: Omer Sela, Inbar Huberman-Spiegelglas, Michael Rotman, Sagie Benaim, Avi Ben-Cohen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.00861v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://sela-omer.github.io/traj-loc)  
  Keywords: identity, i2v, image-to-video, trajectory, dit, evaluation, motion control  
- **[Pano2World: End-to-End 3D Generation via Unified Multi-View Sequences](https://arxiv.org/abs/2607.00832v1)**  
  Authors: Zhenjia Li, Jinrang Jia, Yifeng Shi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.00832v1.pdf)  
  Keywords: diffusion model, video generation, temporal consistency, denoising, trajectory, benchmark  
- **[No Place to Hide: Benchmarking Video Hallucination with Background-Controlled Pairs](https://arxiv.org/abs/2606.31933v1)**  
  Authors: Haojian Huang, Harold Haodong Chen, Meng Luo, Junjia Du, Shanqing Xu, Ziheng Chen, Yanxiang Huang, Yinchuan Li, Ying-Cong Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.31933v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://jethrojames.github.io/VidPair-Halluc)  
  Keywords: dit, evaluation, video generation, benchmark  
- **[Bridging Video Understanding and Generation in a Unified Framework](https://arxiv.org/abs/2606.31326v1)**  
  Authors: Yuqi Wang, Runyi Li, Ruoyu Feng, Renjie Chen, Wenfeng Lin, Mingyu Guo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.31326v1.pdf)  
  Keywords: video generation, dynamics, architecture, autoregressive, benchmark  
- **[InfiniVerse: Occupancy Guided Unbounded Scene Generation for Autonomous Driving](https://arxiv.org/abs/2606.31109v1)**  
  Authors: Xiaoyu Ye, Leheng Li, Xinyu Ji, Yingjie Cai, Hongda He, Xu Yan, Guanyi Zhao, Ying-Cong Chen, Bingbing Liu, Shuguang Cui, Zhen Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.31109v1.pdf)  
  Keywords: diffusion model, video diffusion, autonomous driving, dit, evaluation, autoregressive, benchmark, controllable  

### Text-to-Video Generation

*Showing the latest 50 out of 66 papers*

- **[ICDepth: Taming Video Diffusion Models for Video Depth Estimation via In-Context Conditioning](https://arxiv.org/abs/2607.01677v1)**  
  Authors: Xuanhua He, Jiaxin Xie, Mingzhe Zheng, Qifeng Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.01677v1.pdf)  
  Keywords: diffusion model, video diffusion, diffusion transformer, text-to-video, temporal consistency, dit, benchmark  
- **[Your Data Manifold is Secretly a Reward Model: Shell-LCC for Text-to-Video Generation](https://arxiv.org/abs/2606.30248v1)**  
  Authors: Shihao Zhang, Yuguang Yan, Junzhe Zhang, Wei Zhao, Bohan Wang, Hanwang Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.30248v1.pdf)  
  Keywords: text-to-video, diffusion model, video generation, t2v  
- **[Disco-LoRA: Disentangled Composition of Content, Style, and Motion for Multi-concept Video Customization](https://arxiv.org/abs/2606.26668v1)**  
  Authors: Xuancheng Xu, Gengyun Jia, Bing-Kun Bao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.26668v1.pdf)  
  Keywords: video generation, identity, text-to-video, style, concept, t2v, customization, benchmark, controllable  
- **[SharQ: Bridging Activation Sparsity and FP4 Quantization for LLM Inference](https://arxiv.org/abs/2606.26587v1)**  
  Authors: Haoqian Meng, Yilun Luo, Yafei Zhao, Wenyuan Liu, Huaqing Zheng, Xindian Ma, Peng Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.26587v1.pdf) | [![GitHub](https://img.shields.io/github/stars/actypedef/SharQ?style=social)](https://github.com/actypedef/SharQ)  
  Keywords: t2v, video generation  
- **[DomainShuttle: Freeform Open Domain Subject-driven Text-to-video Generation](https://arxiv.org/abs/2606.26058v1)**  
  Authors: Nan Chen, Yiyang Cai, Rongchang Xie, Junwen Pan, Cheng Chen, Weinan Jia, Zhuowei Chen, Wen Zhou, Zhenbang Sun, Wenhan Luo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.26058v1.pdf)  
  Keywords: video generation, text-to-video, style, dit, personalization, subject-driven  
- **[Causal-rCM: A Unified Teacher-Forcing and Self-Forcing Open Recipe for Autoregressive Diffusion Distillation in Streaming Video Generation and Interactive World Models](https://arxiv.org/abs/2606.25473v1)**  
  Authors: Kaiwen Zheng, Guande He, Min Zhao, Jintao Zhang, Huayu Chen, Jianfei Chen, Chen-Hsuan Lin, Ming-Yu Liu, Jun Zhu, Qianli Ma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.25473v1.pdf)  
  Keywords: diffusion transformer, video diffusion, video generation, physical, world model, action-conditioned, streaming, t2v, distillation, interactive, dit, autoregressive  
- **[Physics Question Scene Graph: Fine-grained Evaluation of Physical Plausibility in Text-to-Video Generation](https://arxiv.org/abs/2606.25306v1)**  
  Authors: Atin Pothiraj, Jaemin Cho, Yue Zhang, Elias Stengel-Eskin, Mohit Bansal  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.25306v1.pdf)  
  Keywords: video generation, physical, text-to-video, physics, evaluation, benchmark  
- **[GeoT2V-Bench: Benchmarking 3D Consistency in Text-to-Video Models via 3D Reconstruction](https://arxiv.org/abs/2606.24829v1)**  
  Authors: Chenrui Fan, Paolo Favaro  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.24829v1.pdf)  
  Keywords: text-to-video, style, t2v, trajectory, evaluation, benchmark  
- **[OrbitForge: Text-to-3D Scene Generation via Reconstruction-Anchored Video Synthesis](https://arxiv.org/abs/2606.24799v1)**  
  Authors: Chenrui Fan, Paolo Favaro  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.24799v1.pdf)  
  Keywords: text-to-video, video synthesis, distillation, dit, evaluation  
- **[Boosting Text-Driven Video Segmentation via Geometry-Aware Distillation](https://arxiv.org/abs/2606.24464v1)**  
  Authors: Tianyu Zhu, Yingping Liang, Hesong Li, Ying Fu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.24464v1.pdf) | [![GitHub](https://img.shields.io/github/stars/Tony1882880/GeoLaV?style=social)](https://github.com/Tony1882880/GeoLaV)  
  Keywords: text-driven video, distillation, benchmark  

### Video Editing

- **[LiveEdit: Towards Real-Time Diffusion-Based Streaming Video Editing](https://arxiv.org/abs/2606.26740v1)**  
  Authors: Xinyu Wang, Chongbo Zhao, Fangneng Zhan, Yue Ma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.26740v1.pdf)  
  Keywords: video generation, efficient, streaming, video editing, distillation, interactive, dit, evaluation, benchmark  
- **[Vera: A Layered Diffusion Model for Content-Preserving Video Editing](https://arxiv.org/abs/2606.23610v1)**  
  Authors: Hongkai Zheng, Ta-Ying Cheng, Benjamin Klein, Yisong Yue, Zhuoning Yuan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.23610v1.pdf)  
  Keywords: diffusion model, video diffusion, video generation, dynamics, text-to-video, architecture, creative, video editing, dit, benchmark  
- **[SteerVTE: Seamless Video Text Editing with Style and Glyph Control](https://arxiv.org/abs/2606.23254v1)**  
  Authors: Kai Zeng, Moran Li, Zhengwei Wang, Yingchen Yu, Yiheng Lin, Ruichuan An, Ming Lu, Qi She, Wentao Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.23254v1.pdf)  
  Keywords: diffusion model, video diffusion, diffusion transformer, image to video, style, video editing, dit  
- **[Generative Relightable Avatars](https://arxiv.org/abs/2606.22718v1)**  
  Authors: Kunwar Maheep Singh, Christian Theobalt, Rishabh Dabral  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.22718v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://vcai.mpi-inf.mpg.de/projects/GRA)  
  Keywords: diffusion model, video diffusion, physical, dynamics, avatar, video-to-video, physics, long video, evaluation, controllable  
- **[ReGenHuman: Re-Generating Human Appearances for Realistic Full-Body Video Anonymization](https://arxiv.org/abs/2606.14972v1)**  
  Authors: Adam Sun, Eshaan Barkataki, Arnold Milstein, Gordon Wetzstein, Ehsan Adeli  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.14972v1.pdf)  
  Keywords: dit, video diffusion, identity, video-to-video  
- **[Lip Forcing: Few-Step Autoregressive Diffusion for Real-time Lip Synchronization](https://arxiv.org/abs/2606.11180v1)**  
  Authors: Paul Hyunbin Cho, Jinhyuk Jang, SeokYoung Lee, Joungbin Lee, Siyoon Jin, Heeseong Shin, Jung Yi, Yunjin Park, Chulmin Park, Seungryong Kim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.11180v1.pdf)  
  Keywords: diffusion model, video diffusion, video-to-video, streaming, denoising, trajectory, dit, autoregressive  
- **[CoVEBench: Can Video Editing Models Handle Complex Instructions?](https://arxiv.org/abs/2606.08415v2)**  
  Authors: Jiangtao Wu, Jiaming Wang, Yiwen He, Yuanxing Zhang, Shihao Li, Dunyuan Liu, Xuedong Zhao, Jialu Chen, Zekun Moore Wang, Jiaheng Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.08415v2.pdf)  
  Keywords: dit, style, video editing, benchmark  
- **[TIDE: Task-Isolated Diffusion for Unified Video Editing and Generation](https://arxiv.org/abs/2606.08260v1)**  
  Authors: Qi Liu, Gang Yue, Mingyu Yin, Lisai Zhang, Yidi Wu, Yaole Wang, Yaohui Wang, Chang Yao, Jingyuan Chen, Lin Ma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.08260v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://LittleWork123.github.io/tide)  
  Keywords: diffusion transformer, video generation, video editing, dit, benchmark  
- **[LoomVideo: Unifying Multimodal Inputs into Video Generation and Editing](https://arxiv.org/abs/2606.06042v2)**  
  Authors: Jianzong Wu, Hao Lian, Jiongfan Yang, Dachao Hao, Ye Tian, Yunhai Tong, Jingyuan Zhu, Biaolong Chen, Qiaosong Qi, Aixi Zhang, Wanggui He, Mushui Liu, Jinlong Liu, Pipei Huang, Hao Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.06042v2.pdf)  
  Keywords: diffusion transformer, video generation, architecture, efficient, video editing, dit, acceleration, benchmark  
- **[V2V-Bench: A Comprehensive Benchmark for Video-to-Video Generation Evaluation](https://arxiv.org/abs/2606.05665v1)**  
  Authors: Tao Liu, Leela Krishna, Gouti Pavan Kumar, Sreeja K, Vishav Garg  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.05665v1.pdf)  
  Keywords: video generation, video-to-video, i2v, t2v, dit, evaluation, benchmark  

### Video Inpainting & Completion

- **[ImageWAM: Do World Action Models Really Need Video Generation, or Just Image Editing?](https://arxiv.org/abs/2606.19531v1)**  
  Authors: Yuyang Zhang, Wenyao Zhang, Zekun Qi, He Zhang, Haitao Lin, Jingbo Zhang, Yao Mu, Xiaokang Yang, Wenjun Zeng, Xin Jin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.19531v1.pdf)  
  Keywords: video generation, video prediction, world model, denoising, dit  
- **[R2RDreamer: 3D-aware Data Augmentation for Spatially-generalized 2D Manipulation Policies](https://arxiv.org/abs/2606.17040v1)**  
  Authors: Xiuwei Xu, Haowen Sun, Angyuan Ma, Yiwei Zhang, Zhenyu Wu, Xiaofeng Wang, Bingyao Yu, Zheng Zhu, Jie Zhou, Jiwen Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17040v1.pdf)  
  Keywords: 3d-aware, style, video completion, image-to-video, simulation, dit, controllable  
- **[PointAction: 3D Points as Universal Action Representations for Robot Control](https://arxiv.org/abs/2606.03943v1)**  
  Authors: Mutian Tong, Han Jiang, Qiao Feng, Lingjie Liu, Jiatao Gu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.03943v1.pdf)  
  Keywords: diffusion model, video diffusion, video generation, dynamics, video prediction, 4d generation, simulation  
- **[World Models: A Comprehensive Survey of Architectures, Methodologies, Reasoning Paradigms, and Applications](https://arxiv.org/abs/2606.00133v1)**  
  Authors: Arif Hassan Zidan, Yi Pan, Hanqi Jiang, Ruiyu Yan, Wei Ruan, Zihao Wu, Lifeng Chen, Weihang You, Xinliang Li, Bowen Chen, Huawen Hu, Peilong Wang, Sizhuang Liu, Jing Zhang, Siyuan Li, Zhengliang Liu, Yu Bao, Lin Zhao, Lichao Sun, Dajiang Zhu, Xiang Li, Jinglei Lv, Quanzheng Li, Wei Liu, Tianming Liu, Wei Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.00133v1.pdf)  
  Keywords: medical, video generation, dynamics, video prediction, education, world model, autonomous driving, architecture, physics, evaluation, interactive, survey, robotics, benchmark  
- **[Full-4D: Generating Full-Scope 4D Scenes from a Single-View Video](https://arxiv.org/abs/2605.25500v1)**  
  Authors: Tingxi Chen, Ke Hao, Yabo Chen, Zhengxue Cheng, Rong Xie, Li Song, Haibin Huang, Chi Zhang, Xuelong Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25500v1.pdf)  
  Keywords: diffusion model, video diffusion, physical, video synthesis, 4d generation, flow matching, distillation, interactive, dit, video interpolation, multi-view video  
- **[CRONOS: Benchmarking Counterfactual Physical Consistency in Video Models](https://arxiv.org/abs/2605.23699v1)**  
  Authors: León Begiristain, Olaf Dünkel, Adam Kortylewski  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.23699v1.pdf)  
  Keywords: dynamics, physical, video prediction, world model, dit, evaluation, benchmark  
- **[GEM-4D: Geometry-Enhanced Video World Models for Robot Manipulation](https://arxiv.org/abs/2605.22882v3)**  
  Authors: Kaichen Zhou, Yuzhen Chen, Fangneng Zhan, Hang Hua, Grace Chen, Xinhai Chang, Ao Qu, Yilun Du, Zhuang Liu, Paul Pu Liang, Mengyu Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.22882v3.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://gem-4d.github.io)  
  Keywords: dynamics, physical, video prediction, world model, architecture, simulation, dit  
- **[Goodbye Drift: Anchored Tree Sampling for Long-Horizon Video-to-Video Generation](https://arxiv.org/abs/2605.20476v1)**  
  Authors: Matthew Bendel, Stephen W. Bailey, Mithilesh Vaidya, Sumukh Badam, Xingzhe He  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20476v1.pdf)  
  Keywords: video generation, style, video-to-video, outpainting, t2v, distillation, dit, autoregressive  
- **[Nano World Models: A Minimalist Implementation of Future Video Prediction](https://arxiv.org/abs/2605.23993v2)**  
  Authors: Siqiao Huang, Partha Kaushik, Michael Chen, Hengkai Pan, Kaiwen Geng, Omar Chehab, Fernando Moreno-Pino, Max Simchowitz  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.23993v2.pdf)  
  Keywords: video generation, video prediction, world model, architecture, simulation, interactive, dit, evaluation, autoregressive  

### Video Super-Resolution & Enhancement

*Showing the latest 50 out of 67 papers*

- **[NeoMap: Training-free Novel-View Synthesis from Single Images and Videos](https://arxiv.org/abs/2607.01962v1)**  
  Authors: Jinxi Li, Tianyi Zhang, Yafei Yang, Zihui Zhang, Peng Huang, Koon Wing Macgyver Lin, Bo Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.01962v1.pdf)  
  Keywords: video synthesis, novel view, denoising, dit, benchmark  
- **[Anti-Prompt: Image Protection against Text-Guided Image-to-Video Generation](https://arxiv.org/abs/2607.01499v1)**  
  Authors: Yeonghwan Song, Chanhui Lee, Jinsoo Park, Jeany Son  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.01499v1.pdf)  
  Keywords: video generation, architecture, temporal consistency, i2v, image-to-video, denoising, dit, evaluation  
- **[Pano2World: End-to-End 3D Generation via Unified Multi-View Sequences](https://arxiv.org/abs/2607.00832v1)**  
  Authors: Zhenjia Li, Jinrang Jia, Yifeng Shi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.00832v1.pdf)  
  Keywords: diffusion model, video generation, temporal consistency, denoising, trajectory, benchmark  
- **[Vertigo Vertigo: Reconstructing a Cinematic Ideal through its Predictive AI Double](https://arxiv.org/abs/2607.00047v1)**  
  Authors: Adam Cole, Mick Grierson  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.00047v1.pdf)  
  Keywords: diffusion model, video diffusion, film, frame interpolation, dit, acceleration  
- **[EcoVideo: Entropy-Orchestrated Video Generation Paradigm in Cloud-Edge Dynamics](https://arxiv.org/abs/2606.30557v1)**  
  Authors: Jiayu Chen, Hengyi Zhang, Maoliang Li, Minyu Li, Zihao Zheng, Xuanzhe Liu, Guojie Luo, Xiang Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.30557v1.pdf) | [![GitHub](https://img.shields.io/github/stars/IF-LAB-PKU/EcoVideo?style=social)](https://github.com/IF-LAB-PKU/EcoVideo)  
  Keywords: dit, denoising, video generation, dynamics  
- **[GeoEdit: Geometry-Aware Object Editing via Dual-Branch Denoising](https://arxiv.org/abs/2606.30003v1)**  
  Authors: Yi He, Jiangming Wang, Xinyu Wang, Mark Fong, Songchun Zhang, Yuxuan Xue, Hai-Tao Zheng, Yue Ma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.30003v1.pdf) | [![GitHub](https://img.shields.io/github/stars/Heey731/GeoEdit?style=social)](https://github.com/Heey731/GeoEdit)  
  Keywords: video diffusion, physical, identity, denoising, dit, evaluation, benchmark  
- **[TempAct: Advancing Temporal Plausibility in Autoregressive Video Generation via Planner-Executor RL](https://arxiv.org/abs/2606.28016v2)**  
  Authors: Jing Wang, Xiangxin Zhou, Jiajun Liang, Kaiqi Liu, Wanyuan Pang, Zhenyu Xie, Tianyu Pang, Xiaodan Liang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.28016v2.pdf)  
  Keywords: diffusion model, video diffusion, video generation, temporal consistency, streaming, denoising, distillation, dit, autoregressive  
- **[TIGER: Taming Identity, Geometry, and Generative Priors for High-Quality Face Video Restoration](https://arxiv.org/abs/2606.24336v2)**  
  Authors: Yang Zhou, Wenxue Li, Peng Zhang, Yifei Chen, Fei Wang, Daiguo Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.24336v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://yzhoulv.github.io/Tiger)  
  Keywords: video generation, identity, efficient, rectified flow, video restoration, evaluation  
- **[Ocean4D: Generative Underwater 4D Reconstruction via Medium-Aware Video Diffusion](https://arxiv.org/abs/2606.23298v1)**  
  Authors: Yuqiang Huang, Yuxi Wang, Junyu Dong, Zhaoxiang Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.23298v1.pdf)  
  Keywords: dit, denoising, video diffusion, benchmark  
- **[One-Step Flow Matching for Generative Modeling of Path-Dependent Physical Fields](https://arxiv.org/abs/2606.22752v1)**  
  Authors: Yijing Zhou, Jasmin Jelovica  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.22752v1.pdf)  
  Keywords: physical simulation, physical, video synthesis, efficient, simulation, denoising, flow matching, distillation, dit  

### World Models & Simulation

*Showing the latest 50 out of 130 papers*

- **[WorldDirector: Building Controllable World Simulators with Persistent Dynamic Memory](https://arxiv.org/abs/2607.02517v1)**  
  Authors: Hanlin Wang, Hao Ouyang, Qiuyu Wang, Wen Wang, Qingyan Bai, Ka Leong Cheng, Yue Yu, Yixuan Li, Yihao Meng, Zichen Liu, Yanhong Zeng, Yujun Shen, Qifeng Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.02517v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://worlddirector.github.io)  
  Keywords: video generation, physical, dynamics, world model, world simulator, controllable  
- **[RetailSMV: Exocentric vs. Egocentric Adaptation of Foundation Video World Models in Retail](https://arxiv.org/abs/2607.00310v1)**  
  Authors: Amirreza Rouhi, Rajat Aggarwal, Parikshit Sakurikar, Anoop M. Namboodiri, Sashi P. Reddi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.00310v1.pdf)  
  Keywords: diffusion model, video diffusion, world model, efficient, world simulator  
- **[MemLearner: Learning to Query Context memory for Video World Models](https://arxiv.org/abs/2606.31734v1)**  
  Authors: Jiwen Yu, Jianxiong Gao, Jianhong Bai, Yiran Qin, Kaiyi Huang, Quande Liu, Xintao Wang, Pengfei Wan, Kun Gai, Xihui Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.31734v1.pdf)  
  Keywords: video generation, world model, efficient, long video, interactive, dit  
- **[UnfoldArt: Zero-Shot Recovery of Full Articulated 3D Objects from Text or Image](https://arxiv.org/abs/2606.30608v2)**  
  Authors: Mohamed el Amine Boudjoghra, Ivan Laptev, Angela Dai  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.30608v2.pdf)  
  Keywords: dit, robotics, interactive  
- **[Walking in the Implicit: Interactive World Exploration via Neural Scene Representation](https://arxiv.org/abs/2606.30045v1)**  
  Authors: Zhiqi Li, Chengrui Dong, Zhenhua Du, Hangning Zhou, Cong Qiu, Hailong Qin, Mu Yang, Dongxu Wei, Peidong Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.30045v1.pdf)  
  Keywords: diffusion transformer, video generation, latent video, interactive, dit  
- **[Semantic-Aware, Physics-Informed, Geometry-Grounded Weather Video Synthesis](https://arxiv.org/abs/2606.29020v1)**  
  Authors: Chenghao Qian, Nedko Savov, Lingdong Kong, Yeying Jin, Rui Song, Wenjing Li, Zhun Zhong, Jiaqi Ma, Gustav Markkula, Luc Van Gool  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.29020v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://jumponthemoon.github.io/w-crafter)  
  Keywords: dynamics, physical, identity, video synthesis, autonomous driving, simulation, physics, dit  
- **[ViPSim: Collaborating Visual and Parameter Spaces for Consistent Long-Horizon Embodied World Models](https://arxiv.org/abs/2606.28804v1)**  
  Authors: Longyu Chen, Heng Li, Wei Yang, Manqi Zhao, Dongsheng Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.28804v1.pdf)  
  Keywords: world model, video synthesis, trajectory, evaluation, benchmark  
- **[PhysisForcing: Physics Reinforced World Simulator for Robotic Manipulation](https://arxiv.org/abs/2606.28128v1)**  
  Authors: Peiwen Zhang, Yufan Deng, Shangkun Sun, Juncheng Ma, Duomin Wang, Jonas Du, Zilin Pan, Ye Huang, Hao Liang, Songyan Huang, Ruihua Zhang, Enze Xie, Ming-Yu Liu, Daquan Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.28128v1.pdf)  
  Keywords: video generation, physical, world model, i2v, simulation, physics, trajectory, world simulator, dit  
- **[Directing the World: Fast Autoregressive Video Generation with Compositional Human-Camera Control](https://arxiv.org/abs/2606.27964v1)**  
  Authors: Haoyuan Wang, Yabo Chen, Haibin Huang, Chi Zhang, Xuelong Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.27964v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://whydahuzi.github.io/Directing-the-World.github.io)  
  Keywords: video generation, dynamics, world model, human motion, autoregressive, trajectory, interactive, camera control, motion control, controllable  
- **[MemoBench: Benchmarking World Modeling in Dynamically Changing Environments](https://arxiv.org/abs/2606.27537v4)**  
  Authors: Haoyu Chen, Kaichen Zhou, Hang Hua, Kaile Zhang, Jingwen Qian, Wufei Ma, Haonan Chen, Chunjiang Liu, Yizhou Zhao, Xiaoyuan Wang, Weiyue Li, Alan Yuille, Paul Pu Liang, Yilun Du  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.27537v4.pdf)  
  Keywords: video generation, physical, world model, evaluation, benchmark  



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
