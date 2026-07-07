# Awesome Video Diffusions [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of latest research papers, projects and resources related to Video Diffusion Models and Video Generation. Content is automatically updated daily.

> Last Update: 2026-07-07 03:23:59

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
- [Applications](#applications) (46 papers) - Domain-specific applications of video diffusion models
- [Architecture & Efficiency](#architecture-&-efficiency) (363 papers) - Architectural innovations (DiT, UNet), flow matching, and training/inference efficiency
- [Audio & Multi-modal](#audio-&-multi-modal) (21 papers) - Audio-driven and multi-modal conditioned video generation
- [Controllable Generation](#controllable-generation) (142 papers) - Controllable video generation with motion, camera, pose, or layout guidance
- [Human & Character Animation](#human-&-character-animation) (21 papers) - Human-centric video generation including talking heads, dance, and character animation
- [Image-to-Video Generation](#image-to-video-generation) (49 papers) - Methods for animating still images into videos
- [Long Video Generation](#long-video-generation) (132 papers) - Generating temporally consistent long-form videos beyond short clips
- [Personalization & Customization](#personalization-&-customization) (88 papers) - Personalized video generation with custom subjects, identities, or styles
- [Physical Understanding](#physical-understanding) (158 papers) - Physics-aware video generation and dynamics modeling
- [Surveys & Benchmarks](#surveys-&-benchmarks) (232 papers) - Survey papers, benchmarks, and evaluation metrics for video generation
- [Text-to-Video Generation](#text-to-video-generation) (70 papers) - Foundation models and methods for generating videos from text prompts
- [Video Editing](#video-editing) (30 papers) - Diffusion-based video editing, style transfer, and manipulation
- [Video Inpainting & Completion](#video-inpainting-&-completion) (10 papers) - Video inpainting, completion, outpainting, and temporal prediction
- [Video Super-Resolution & Enhancement](#video-super-resolution-&-enhancement) (70 papers) - Video quality improvement, upscaling, restoration, and frame interpolation
- [World Models & Simulation](#world-models-&-simulation) (128 papers) - Video generation as world simulators and interactive environment generation



## Table of Contents

- [Categorized Papers](#categorized-papers)
- [Classic Papers](#classic-papers)
- [Open Source Projects](#open-source-projects)
- [Applications](#applications)
- [Tutorials & Blogs](#tutorials--blogs)





## Categorized Papers

### 3D-aware Video Generation

- **[MV-Forcing: Long Multi-View Video Generation via 4D-Grounded Spatio-Temporal Self-Forcing](https://arxiv.org/abs/2607.05376v1)**  
  Authors: Gal Fiebelman, Hadar Averbuch-Elor, Sagie Benaim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.05376v1.pdf)  
  Keywords: denoising, video generation, autoregressive, distillation, video diffusion, multi-view video, diffusion model  
- **[HandsOnWorld: Unconstrained Egocentric Video Generation with Camera-Disentangled Hand Control](https://arxiv.org/abs/2607.02075v1)**  
  Authors: Yushuo Chen, Xiaoyu Shi, Xiaoshi Wu, Xintao Wang, Pengfei Wan, Yebin Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.02075v1.pdf)  
  Keywords: 3d-aware, video generation  
- **[NeoMap: Training-free Novel-View Synthesis from Single Images and Videos](https://arxiv.org/abs/2607.01962v1)**  
  Authors: Jinxi Li, Tianyi Zhang, Yafei Yang, Zihui Zhang, Peng Huang, Koon Wing Macgyver Lin, Bo Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.01962v1.pdf)  
  Keywords: denoising, video synthesis, benchmark, dit, novel view  
- **[RayPE: Ray-Space Positional Encoding for 3D-Aware Video Generation](https://arxiv.org/abs/2606.27345v2)**  
  Authors: Minghao Yin, Jiahao Lu, Wenbo Hu, Wang Zhao, Shan Ying, Kai Han  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.27345v2.pdf)  
  Keywords: video generation, 3d-aware, video diffusion, dit, camera control, diffusion transformer, identity  
- **[Follow Your Track: Precise Skeleton Animation Controlled by 3D Trajectories](https://arxiv.org/abs/2606.25344v1)**  
  Authors: Yueting Liu, Yanqin Jiang, Nian Liu, Jingmen Zhou, Zhengjun Zha, Weiming Hu, Jin Gao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.25344v1.pdf)  
  Keywords: efficient, 4d generation, trajectory, body motion, dit, temporal consistency  
- **[OmniDrive: An LLM-Choreographed Multi-Agent World Model with Unified Latent Co-Compression for Multi-View Driving Video Generation](https://arxiv.org/abs/2606.17536v1)**  
  Authors: Zijie Meng, Yufei Liu, Chengqian Ma, Zhiyu Li, Jiyuan Liu, Wenhua Nie, Bingcai Wei, Shuqin Chen, Weichen Xu, Jiquan Yuan, Miao Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17536v1.pdf)  
  Keywords: video generation, layout, autonomous driving, dit, controllable, multi-view video, world model  
- **[R2RDreamer: 3D-aware Data Augmentation for Spatially-generalized 2D Manipulation Policies](https://arxiv.org/abs/2606.17040v1)**  
  Authors: Xiuwei Xu, Haowen Sun, Angyuan Ma, Yiwei Zhang, Zhenyu Wu, Xiaofeng Wang, Bingyao Yu, Zheng Zhu, Jie Zhou, Jiwen Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17040v1.pdf)  
  Keywords: video completion, style, 3d-aware, simulation, dit, controllable, image-to-video  
- **[Flex4DHuman: Flexible Multi-view Video Diffusion for 4D Human Reconstruction](https://arxiv.org/abs/2606.13655v2)**  
  Authors: Jen-Hao Cheng, Yipeng Wang, Hao Zhang, Gengshan Yang, Jenq-Neng Hwang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13655v2.pdf)  
  Keywords: architecture, video diffusion, simulation, dit, multi-view video, diffusion model, text-to-video  
- **[Latent Spatial Memory for Video World Models](https://arxiv.org/abs/2606.09828v1)**  
  Authors: Weijie Wang, Haoyu Zhao, Yifan Yang, Feng Chen, Zeyu Zhang, Yefei He, Zicheng Duan, Donny Y. Chen, Yuqing Yang, Bohan Zhuang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.09828v1.pdf)  
  Keywords: video generation, depth-guided, world model, diffusion model, novel view  
- **[CP4D: Compositional Physics-aware 4D Scene Generation](https://arxiv.org/abs/2606.09187v1)**  
  Authors: Hanxin Zhu, Cong Wang, Tianyu He, Long Chen, Xin Jin, Chen Gao, Zhibo Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.09187v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://anonymous.4open.science/w/CP4D)  
  Keywords: 4d generation, interactive, video diffusion, physics, dynamics, physical, diffusion model, physics-aware  

### Applications

- **[SpheRoPE: Zero-Shot Optimization-Free 360 Panorama Generation with Spherical RoPE](https://arxiv.org/abs/2606.32033v1)**  
  Authors: Or Hirschorn, Aaron Olender, Eli Alshan, Ianir Ideses, Lior Fritz, Sagie Benaim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.32033v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://orhir.github.io/SpheRoPE)  
  Keywords: diffusion transformer, creative  
- **[World Narrative Model for Highly Controllable Video Generation: A Paradigm Shift from Pixel Sampling to Physical World Orchestration](https://arxiv.org/abs/2606.31946v1)**  
  Authors: Ye Chen, Xuanhong Chen, Yupeng Zhu, Liming Tan, Zhewen Wan, Yuxuan Xiong, Tielong Wang, Jinfan Liu, Wuze Zhang, Xiongzhen Zhang, Feifei Li, Xianglin Luo, Zhehan Zhao, Zhifan Zhang, Laisheng Kou, Zhujing Liang, Yugang Chen, Muchun Chen, Xu Miao, Yijing Zhang, Xiaojie Sheng, Qiang Hu, Jialiang Chen, Weimin Zhang, Wenjun Zhang, Bingbing Ni  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.31946v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://glassroom.sjtu.edu.cn/WNM)  
  Keywords: efficient, video generation, layout, dit, film, controllable, physical  
- **[InfiniVerse: Occupancy Guided Unbounded Scene Generation for Autonomous Driving](https://arxiv.org/abs/2606.31109v1)**  
  Authors: Xiaoyu Ye, Leheng Li, Xinyu Ji, Yingjie Cai, Hongda He, Xu Yan, Guanyi Zhao, Ying-Cong Chen, Bingbing Liu, Shuguang Cui, Zhen Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.31109v1.pdf)  
  Keywords: evaluation, autonomous driving, benchmark, autoregressive, video diffusion, dit, controllable, diffusion model  
- **[Vertigo Vertigo: Reconstructing a Cinematic Ideal through its Predictive AI Double](https://arxiv.org/abs/2607.00047v1)**  
  Authors: Adam Cole, Mick Grierson  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.00047v1.pdf)  
  Keywords: video diffusion, dit, film, acceleration, frame interpolation, diffusion model  
- **[UnfoldArt: Zero-Shot Recovery of Full Articulated 3D Objects from Text or Image](https://arxiv.org/abs/2606.30608v2)**  
  Authors: Mohamed el Amine Boudjoghra, Ivan Laptev, Angela Dai  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.30608v2.pdf)  
  Keywords: dit, interactive, robotics  
- **[Semantic-Aware, Physics-Informed, Geometry-Grounded Weather Video Synthesis](https://arxiv.org/abs/2606.29020v1)**  
  Authors: Chenghao Qian, Nedko Savov, Lingdong Kong, Yeying Jin, Rui Song, Wenjing Li, Zhun Zhong, Jiaqi Ma, Gustav Markkula, Luc Van Gool  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.29020v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://jumponthemoon.github.io/w-crafter)  
  Keywords: autonomous driving, video synthesis, simulation, dit, physics, identity, dynamics, physical  
- **[A Good Talk Does not Look Like a Summary, It Teaches You! Measuring Takeaways from Paper-to-Video Talks](https://arxiv.org/abs/2606.28531v1)**  
  Authors: Ishani Mondal, Aparna Garimella, Ananya Sai, Pannaga Shivaswamy, Jordan Boyd-Graber  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.28531v1.pdf)  
  Keywords: concept, video generation, education, evaluation  
- **[ReWorld: Learning Better Representations for World Action Models](https://arxiv.org/abs/2606.27504v1)**  
  Authors: Tianze Xia, Lijun Zhou, Kaixin Xiong, Jingfeng Yao, Yu Zhu, Zhenxin Zhu, Bing Wang, Guang Chen, Hangjun Ye, Wenyu Liu, Haiyang Sun, Xinggang Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.27504v1.pdf)  
  Keywords: efficient, architecture, video generation, autonomous driving, dit, world model  
- **[PRISM: Feed-Forward Single-Image 3D Reconstruction via Geometric Warp-Residual Modeling](https://arxiv.org/abs/2606.25430v1)**  
  Authors: Zhijie Zheng, Xinhao Xiang, Jiawei Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.25430v1.pdf)  
  Keywords: benchmark, distillation, video diffusion, robotics, diffusion model  
- **[CineCap: Structured Reasoning with Spatio-Temporal Anchors for Cinematographic Video Captioning](https://arxiv.org/abs/2606.24636v1)**  
  Authors: Xinyu Mao, Yuhui Zeng, Xiaokun Liu, Wenyu Qin, Meng Wang, Xin Tao, Pengfei Wan, Xiaohan Xing, Max Meng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.24636v1.pdf) | [![GitHub](https://img.shields.io/github/stars/Hectormxy/CineCap.git?style=social)](https://github.com/Hectormxy/CineCap.git)  
  Keywords: video generation, concept, evaluation, benchmark, dit, film, controllable  

### Architecture & Efficiency

*Showing the latest 50 out of 363 papers*

- **[MV-Forcing: Long Multi-View Video Generation via 4D-Grounded Spatio-Temporal Self-Forcing](https://arxiv.org/abs/2607.05376v1)**  
  Authors: Gal Fiebelman, Hadar Averbuch-Elor, Sagie Benaim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.05376v1.pdf)  
  Keywords: denoising, video generation, autoregressive, distillation, video diffusion, multi-view video, diffusion model  
- **[FlowMark: Mask-Guided Video Watermarking](https://arxiv.org/abs/2607.05261v1)**  
  Authors: Vishal Asnani, Shruti Agarwal, John Collomosse  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.05261v1.pdf)  
  Keywords: dit, architecture, dynamics  
- **[Consistent and Editable: A Balanced Framework for Text-Guided Video Editing](https://arxiv.org/abs/2607.05056v1)**  
  Authors: Tao Jin, Li Xiao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.05056v1.pdf)  
  Keywords: dit, temporal consistency, diffusion model, video editing  
- **[DSWAM: A Dual-System World Action Foundation Model for Fine-Grained Robot Manipulation](https://arxiv.org/abs/2607.04927v1)**  
  Authors: Jian Zhu, Jianjun Zhang, Taiyi Su, Tianbin Liu, Zhangyuan Wang, Kai Xie, Zitai Huang, Chong Ma, Youzhang He, Tianjian Wang, Hanyang Wang, Weihao Ding, Yi Xu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.04927v1.pdf)  
  Keywords: video generation, evaluation, acceleration, world model, physical  
- **[Video Generation Models Are Inherent Lighting Estimators](https://arxiv.org/abs/2607.04674v1)**  
  Authors: Ziqi Cai, Shuchen Weng, Kaiqi Liu, Zifeng Wang, Zhiquan Zhang, Minggui Teng, Han Jiang, Boxin Shi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.04674v1.pdf)  
  Keywords: efficient, video generation, video diffusion, video inpainting, physical, diffusion model  
- **[Lights, Camera, Carbon: Architectural Scaling Laws for Video Generation Energy Consumption](https://arxiv.org/abs/2607.04553v1)**  
  Authors: Nidhal Jegham, Boris Gamazaychikov, Sasha Luccioni  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.04553v1.pdf)  
  Keywords: efficient, architecture, video generation, benchmark, video diffusion, t2v, dit, diffusion model, text-to-video  
- **[Mask2Real-WM: Segmentation Masks as a Sim-to-Real Bridge for Controllable Dexterous World Models](https://arxiv.org/abs/2607.04546v1)**  
  Authors: Riccardo O. Feingold, Davide Liconti, Chenyu Yang, Robert K. Katzschmann  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.04546v1.pdf)  
  Keywords: evaluation, benchmark, video diffusion, simulation, dit, action-conditioned, controllable, dynamics, world model, physical  
- **[Aura: Consistent Multi-Subject Video Generation via VLM-Grounded Semantic Alignment](https://arxiv.org/abs/2607.04311v1)**  
  Authors: Zixiang Zhou, Zhentao Yu, Yifeng Ma, Hongmei Wang, Wenqing Yu, Cong Wang, Zilin Yang, Rui Chen, Jiarong Ou, Yezhou Liu, Yuan Zhou, Qinglin Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.04311v1.pdf)  
  Keywords: video generation, video synthesis, dit, diffusion transformer, identity, controllable, dynamics, subject-driven  
- **[Worldscape-MoE: A Unified Mixture-of-Experts World Model for Scalable Heterogeneous Action Control](https://arxiv.org/abs/2607.03964v1)**  
  Authors: Jianjie Fang, Yongyan Xu, Ziyou Wang, Chen Gao, Yuchao Huang, Zhaolu Wang, Rongze Tang, Mingyuan Jia, Baining Zhao, Weichen Zhang, Xin Zhang, Haisheng Su, Yu Shang, Wei Wu, Xinlei Chen, Yong Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.03964v1.pdf)  
  Keywords: video generation, interactive, dit, diffusion transformer, controllable, dynamics, world model, physical  
- **[Reward Lightning: Fast Video Generation via Homologous Preference Distillation](https://arxiv.org/abs/2607.03960v1)**  
  Authors: Jiaxiang Cheng, Bing Ma, Xuhua Ren, Kai Yu, Peng Zhang, Tianxiang Zheng, Qinglin Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.03960v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://reward-lightning.github.io)  
  Keywords: video generation, distillation, video diffusion, acceleration, diffusion model  

### Audio & Multi-modal

- **[AVTok: 1D Unified Tokenization for Holistic Audio-Video Generation](https://arxiv.org/abs/2606.30811v1)**  
  Authors: Kien T. Pham, I Chieh Chen, Qifeng Chen, Long Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.30811v1.pdf)  
  Keywords: efficient, architecture, video generation, dit, audio-to-video, sound  
- **[TRUST: Efficient Abdominal Trauma Recognition via Image-to-Ultrasound-Video Transfer Learning](https://arxiv.org/abs/2606.27777v1)**  
  Authors: Enguang Wang, Hao Zhou, Shuo Gao, Tuo Liu, Guangquan Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.27777v1.pdf)  
  Keywords: efficient, dit, dynamics, sound, image-to-video  
- **[PhyEditBench: A Real-World Multi-Stage Benchmark for Physics-Aware Image Editing](https://arxiv.org/abs/2606.26551v2)**  
  Authors: Shengbin Guo, Shaokang He, Chaoyue Meng, Shengpeng Xiao, Xunzhi Xiang, Shaofeng Zhang, Qi Fan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.26551v2.pdf) | [![GitHub](https://img.shields.io/github/stars/Previsior/PhyEditBench?style=social)](https://github.com/Previsior/PhyEditBench)  
  Keywords: video generation, evaluation, benchmark, multi-modal, dit, physics, dynamics, physical, physics-aware  
- **[Wan-Streamer v0.1: End-to-end Real-time Interactive Foundation Models](https://arxiv.org/abs/2606.25041v3)**  
  Authors: Lianghua Huang, Zhi-Fan Wu, Wei Wang, Yupeng Shi, Mengyang Feng, Junjie He, Chen-Wei Xie, Yu Liu, Jingren Zhou, Ang Wang, Bang Zhang, Baole Ai, Chen Liang, Cheng Yu, Chongyang Zhong, Jinwei Qi, Kai Zhu, Pandeng Li, Peng Zhang, Wenyuan Zhang, Xinhua Cheng, Yitong Huang, Yun Zheng, Yuzheng Wang, Zoubin Bi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.25041v3.pdf)  
  Keywords: audio-driven, interactive, streaming, avatar  
- **[InteractiveAvatar: Real-Time Streaming Video Generation for Consistent and Intent-Aware Avatars](https://arxiv.org/abs/2606.22905v2)**  
  Authors: Quanyue Song, Yishan He, Yanfei Zhang, Shihao Cheng, Zhixiang He, Zhizhi Guo, Chi Zhang, Xuelong Li, Caigui Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.22905v2.pdf)  
  Keywords: streaming, video generation, autoregressive, distillation, interactive, avatar, temporal consistency, audio-driven  
- **[T-MOR: Learning Motion-Aware Skeleton Representations for Human Action Recognition](https://arxiv.org/abs/2606.21607v1)**  
  Authors: Di Yang, Mahmoud Ali, Quan Kong, Gianpiero Francesca, Francois Bremond  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.21607v1.pdf)  
  Keywords: human motion, benchmark, multi-modal, dit, physical  
- **[PermaVid: Consistent Video Generation Across Edits via Disentangled Context Memory](https://arxiv.org/abs/2606.16449v2)**  
  Authors: Shuai Yang, Bingjie Gao, Ziwei Liu, Jiaqi Wang, Dahua Lin, Tong Wu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16449v2.pdf)  
  Keywords: dit, multi-modal, video generation, layout  
- **[ReFree: Towards Realistic Co-Speech Video Generation via Reward-Free RL and Multilevel Speech Guidance](https://arxiv.org/abs/2606.13304v1)**  
  Authors: Salaheldin Mohamed, M. Hamza Mughal, Rishabh Dabral, Christian Theobalt  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13304v1.pdf)  
  Keywords: video generation, evaluation, speech-driven  
- **[MSUE: Multi-Modal Soccer Understanding Expert](https://arxiv.org/abs/2606.12106v1)**  
  Authors: Litao Li, Yibo Yu, Yufeng Hu, Zhuo Yang, Jiali Wen, Yixin Chen, Yixi Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.12106v1.pdf)  
  Keywords: benchmark, architecture, multi-modal, long-form  
- **[Conan-embedding-v3: Fusing Modality-Specific Models for Omni-Modal Embedding](https://arxiv.org/abs/2606.09331v1)**  
  Authors: Shiyu Li, Zhiyuan Hu, Yifan Wang, Peiming Li, Zheng Wei, Yang Tang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.09331v1.pdf)  
  Keywords: multi-modal, architecture, dynamics  

### Controllable Generation

*Showing the latest 50 out of 142 papers*

- **[Mask2Real-WM: Segmentation Masks as a Sim-to-Real Bridge for Controllable Dexterous World Models](https://arxiv.org/abs/2607.04546v1)**  
  Authors: Riccardo O. Feingold, Davide Liconti, Chenyu Yang, Robert K. Katzschmann  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.04546v1.pdf)  
  Keywords: evaluation, benchmark, video diffusion, simulation, dit, action-conditioned, controllable, dynamics, world model, physical  
- **[Aura: Consistent Multi-Subject Video Generation via VLM-Grounded Semantic Alignment](https://arxiv.org/abs/2607.04311v1)**  
  Authors: Zixiang Zhou, Zhentao Yu, Yifeng Ma, Hongmei Wang, Wenqing Yu, Cong Wang, Zilin Yang, Rui Chen, Jiarong Ou, Yezhou Liu, Yuan Zhou, Qinglin Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.04311v1.pdf)  
  Keywords: video generation, video synthesis, dit, diffusion transformer, identity, controllable, dynamics, subject-driven  
- **[Worldscape-MoE: A Unified Mixture-of-Experts World Model for Scalable Heterogeneous Action Control](https://arxiv.org/abs/2607.03964v1)**  
  Authors: Jianjie Fang, Yongyan Xu, Ziyou Wang, Chen Gao, Yuchao Huang, Zhaolu Wang, Rongze Tang, Mingyuan Jia, Baining Zhao, Weichen Zhang, Xin Zhang, Haisheng Su, Yu Shang, Wei Wu, Xinlei Chen, Yong Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.03964v1.pdf)  
  Keywords: video generation, interactive, dit, diffusion transformer, controllable, dynamics, world model, physical  
- **[ProxyUp: Training-Free Proxy-Conditioned Video Generation for Controllable Dynamics](https://arxiv.org/abs/2607.03732v1)**  
  Authors: Zanwei Zhou, Jiazhong Cen, Jiemin Fang, Yumeng He, Chen Yang, Sikuang Li, Fanpeng Meng, Zhikuan Bao, Wei Shen, Qi Tian  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.03732v1.pdf)  
  Keywords: video generation, video editing, simulation, dit, physics, controllable, dynamics, physical  
- **[Track the Noise, Move the World:3D-Grounded Motion-Consistent Noise for Controllable Video Generation](https://arxiv.org/abs/2607.02798v1)**  
  Authors: Long Vu, Tan Ngo, Animesh Karnewar, Amir Habibian, Binh-Son Hua, Hung Bui, Minh Hoai Nguyen, Phong Nguyen-Ha  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.02798v1.pdf)  
  Keywords: denoising, video generation, benchmark, video diffusion, dit, temporal consistency, latent video, motion control, controllable, diffusion model, text-to-video  
- **[WorldDirector: Building Controllable World Simulators with Persistent Dynamic Memory](https://arxiv.org/abs/2607.02517v1)**  
  Authors: Hanlin Wang, Hao Ouyang, Qiuyu Wang, Wen Wang, Qingyan Bai, Ka Leong Cheng, Yue Yu, Yixuan Li, Yihao Meng, Zichen Liu, Yanhong Zeng, Yujun Shen, Qifeng Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.02517v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://worlddirector.github.io)  
  Keywords: video generation, world simulator, controllable, dynamics, world model, physical  
- **[QWERTY: Training-Free Motion Control via Query-Warped Video Diffusion Transformers](https://arxiv.org/abs/2607.01869v1)**  
  Authors: Kyobin Choo, Youngmin Kim, Hyunkyung Han, Geunrip Park, Chanyoung Kim, Sunyoung Jung, Seong Jae Hwang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.01869v1.pdf)  
  Keywords: trajectory, video diffusion, dit, diffusion transformer, motion control, diffusion model, image-to-video  
- **[SimWorlds: A Multi-Agent System for Dynamic 3D Scene Creation](https://arxiv.org/abs/2607.01766v1)**  
  Authors: Chunjiang Liu, Xiaoyuan Wang, Haoyu Chen, Yizhou Zhao, Ming-Hsuan Yang, László A. Jeni  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.01766v1.pdf)  
  Keywords: video generation, layout, benchmark, dit, physics, physical  
- **[Unified Panoramic-Gaussian Representation for Monocular 4D Scene Synthesis](https://arxiv.org/abs/2607.01663v1)**  
  Authors: Yuankun Yang, Yi Wei, Wenyang Zhou, Li Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.01663v1.pdf)  
  Keywords: dit, physical, trajectory, video generation  
- **[TrajLoc: Trajectory-Attention Localization for Multi-Object Motion Control](https://arxiv.org/abs/2607.00861v1)**  
  Authors: Omer Sela, Inbar Huberman-Spiegelglas, Michael Rotman, Sagie Benaim, Avi Ben-Cohen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.00861v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://sela-omer.github.io/traj-loc)  
  Keywords: evaluation, trajectory, dit, motion control, identity, i2v, image-to-video  

### Human & Character Animation

- **[3D Scene-Adaptive Trajectory-Controllable Human Image Animation with Camera Movement](https://arxiv.org/abs/2606.30514v2)**  
  Authors: Deyin Liu, Jicheng Xu, Lin Yuanbo Wu, Xiaowei Zhao, Xiatian Zhu, Zhe Jin, Anjan Dutta  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.30514v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://robinhood256100.github.io/web-disp)  
  Keywords: human motion, video generation, benchmark, image animation, trajectory, dit, camera control, controllable  
- **[OmniDance: Multimodal Driven Dance Video Generation with Large-scale Internet Data](https://arxiv.org/abs/2606.30019v1)**  
  Authors: Kaixing Yang, Jiashu Zhu, Xulong Tang, Ziqiao Peng, Xiangyue Zhang, Chubin Chen, Puwei Wang, Jiahong Wu, Xiangxiang Chu, Hongyan Liu, Jun He  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.30019v1.pdf) | [![GitHub](https://img.shields.io/github/stars/AMAP-ML/OmniDance?style=social)](https://github.com/AMAP-ML/OmniDance)  
  Keywords: human motion, architecture, video generation, dit, dynamics, i2v  
- **[EMOSH: Expressive Motion and Shape Disentanglement for Human Animation](https://arxiv.org/abs/2606.28026v1)**  
  Authors: Dongbin Zhang, Hao Liu, Binquan Dai, Kangjie Chen, Chuming Wang, Chen Li, Jing Lyu, Haoqian Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.28026v1.pdf)  
  Keywords: video generation, avatar, human animation, dit, identity, controllable, gesture  
- **[Directing the World: Fast Autoregressive Video Generation with Compositional Human-Camera Control](https://arxiv.org/abs/2606.27964v1)**  
  Authors: Haoyuan Wang, Yabo Chen, Haibin Huang, Chi Zhang, Xuelong Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.27964v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://whydahuzi.github.io/Directing-the-World.github.io)  
  Keywords: human motion, video generation, autoregressive, trajectory, interactive, camera control, motion control, controllable, dynamics, world model  
- **[Follow Your Track: Precise Skeleton Animation Controlled by 3D Trajectories](https://arxiv.org/abs/2606.25344v1)**  
  Authors: Yueting Liu, Yanqin Jiang, Nian Liu, Jingmen Zhou, Zhengjun Zha, Weiming Hu, Jin Gao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.25344v1.pdf)  
  Keywords: efficient, 4d generation, trajectory, body motion, dit, temporal consistency  
- **[Wan-Streamer v0.1: End-to-end Real-time Interactive Foundation Models](https://arxiv.org/abs/2606.25041v3)**  
  Authors: Lianghua Huang, Zhi-Fan Wu, Wei Wang, Yupeng Shi, Mengyang Feng, Junjie He, Chen-Wei Xie, Yu Liu, Jingren Zhou, Ang Wang, Bang Zhang, Baole Ai, Chen Liang, Cheng Yu, Chongyang Zhong, Jinwei Qi, Kai Zhu, Pandeng Li, Peng Zhang, Wenyuan Zhang, Xinhua Cheng, Yitong Huang, Yun Zheng, Yuzheng Wang, Zoubin Bi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.25041v3.pdf)  
  Keywords: audio-driven, interactive, streaming, avatar  
- **[InteractiveAvatar: Real-Time Streaming Video Generation for Consistent and Intent-Aware Avatars](https://arxiv.org/abs/2606.22905v2)**  
  Authors: Quanyue Song, Yishan He, Yanfei Zhang, Shihao Cheng, Zhixiang He, Zhizhi Guo, Chi Zhang, Xuelong Li, Caigui Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.22905v2.pdf)  
  Keywords: streaming, video generation, autoregressive, distillation, interactive, avatar, temporal consistency, audio-driven  
- **[Generative Relightable Avatars](https://arxiv.org/abs/2606.22718v1)**  
  Authors: Kunwar Maheep Singh, Christian Theobalt, Rishabh Dabral  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.22718v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://vcai.mpi-inf.mpg.de/projects/GRA)  
  Keywords: long video, evaluation, video diffusion, avatar, physics, controllable, dynamics, video-to-video, physical, diffusion model  
- **[T-MOR: Learning Motion-Aware Skeleton Representations for Human Action Recognition](https://arxiv.org/abs/2606.21607v1)**  
  Authors: Di Yang, Mahmoud Ali, Quan Kong, Gianpiero Francesca, Francois Bremond  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.21607v1.pdf)  
  Keywords: human motion, benchmark, multi-modal, dit, physical  
- **[Avatar V: Scaling Video-Reference Avatar Video Generation](https://arxiv.org/abs/2606.13872v1)**  
  Authors: Benjamin Liang, Ce Chen, Desmond Lin, Ivan Somov, Jiajun Zhao, Jiewei Yuan, Jingfeng Zhang, Junhao Huang, Nik Nolte, Pedram Haqiqi, Penghan Wang, Rong Yan, Rui Zhang, Sam Prokopchuk, Sivan Wang, Viktor Goriachko, Yi Ren, Yuanming Li, Yutao Chen, Zhenhui Ye, Zhibin Hong, Zilong Nie, Zujin Guo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13872v1.pdf)  
  Keywords: flow matching, video generation, evaluation, benchmark, distillation, style, avatar, super-resolution, dit, acceleration, identity, dynamics  

### Image-to-Video Generation

- **[CineMobile: On-Device Image-to-Video Diffusion for Cinematic Camera Motion Generation](https://arxiv.org/abs/2607.03803v1)**  
  Authors: Xuyao Huang, Zelai Deng, Xu Wang, Xizhong Xiao, Zhijie Deng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.03803v1.pdf)  
  Keywords: denoising, efficient, architecture, video generation, distillation, video diffusion, dit, diffusion transformer, image-to-video  
- **[OrbitQuant: Data-Agnostic Quantization for Image and Video Diffusion Transformers](https://arxiv.org/abs/2607.02461v1)**  
  Authors: Donghyun Lee, Jitesh Chavan, Duy Nguyen, Sam Huang, Liming Jiang, Priyadarshini Panda, Timo Mertens, Saurabh Shukla  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.02461v1.pdf)  
  Keywords: video generation, video diffusion, dit, image to video, diffusion transformer  
- **[QWERTY: Training-Free Motion Control via Query-Warped Video Diffusion Transformers](https://arxiv.org/abs/2607.01869v1)**  
  Authors: Kyobin Choo, Youngmin Kim, Hyunkyung Han, Geunrip Park, Chanyoung Kim, Sunyoung Jung, Seong Jae Hwang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.01869v1.pdf)  
  Keywords: trajectory, video diffusion, dit, diffusion transformer, motion control, diffusion model, image-to-video  
- **[Anti-Prompt: Image Protection against Text-Guided Image-to-Video Generation](https://arxiv.org/abs/2607.01499v1)**  
  Authors: Yeonghwan Song, Chanhui Lee, Jinsoo Park, Jeany Son  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.01499v1.pdf)  
  Keywords: denoising, architecture, video generation, evaluation, dit, temporal consistency, i2v, image-to-video  
- **[TrajLoc: Trajectory-Attention Localization for Multi-Object Motion Control](https://arxiv.org/abs/2607.00861v1)**  
  Authors: Omer Sela, Inbar Huberman-Spiegelglas, Michael Rotman, Sagie Benaim, Avi Ben-Cohen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.00861v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://sela-omer.github.io/traj-loc)  
  Keywords: evaluation, trajectory, dit, motion control, identity, i2v, image-to-video  
- **[3D Scene-Adaptive Trajectory-Controllable Human Image Animation with Camera Movement](https://arxiv.org/abs/2606.30514v2)**  
  Authors: Deyin Liu, Jicheng Xu, Lin Yuanbo Wu, Xiaowei Zhao, Xiatian Zhu, Zhe Jin, Anjan Dutta  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.30514v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://robinhood256100.github.io/web-disp)  
  Keywords: human motion, video generation, benchmark, image animation, trajectory, dit, camera control, controllable  
- **[OmniDance: Multimodal Driven Dance Video Generation with Large-scale Internet Data](https://arxiv.org/abs/2606.30019v1)**  
  Authors: Kaixing Yang, Jiashu Zhu, Xulong Tang, Ziqiao Peng, Xiangyue Zhang, Chubin Chen, Puwei Wang, Jiahong Wu, Xiangxiang Chu, Hongyan Liu, Jun He  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.30019v1.pdf) | [![GitHub](https://img.shields.io/github/stars/AMAP-ML/OmniDance?style=social)](https://github.com/AMAP-ML/OmniDance)  
  Keywords: human motion, architecture, video generation, dit, dynamics, i2v  
- **[PhysisForcing: Physics Reinforced World Simulator for Robotic Manipulation](https://arxiv.org/abs/2606.28128v1)**  
  Authors: Peiwen Zhang, Yufan Deng, Shangkun Sun, Juncheng Ma, Duomin Wang, Jonas Du, Zilin Pan, Ye Huang, Hao Liang, Songyan Huang, Ruihua Zhang, Enze Xie, Ming-Yu Liu, Daquan Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.28128v1.pdf)  
  Keywords: video generation, world simulator, trajectory, simulation, dit, physics, world model, physical, i2v  
- **[TRUST: Efficient Abdominal Trauma Recognition via Image-to-Ultrasound-Video Transfer Learning](https://arxiv.org/abs/2606.27777v1)**  
  Authors: Enguang Wang, Hao Zhou, Shuo Gao, Tuo Liu, Guangquan Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.27777v1.pdf)  
  Keywords: efficient, dit, dynamics, sound, image-to-video  
- **[VPA-Guard: Defending and Benchmarking Image-to-Video Generation Against Visual Prompt Attacks](https://arxiv.org/abs/2606.25592v1)**  
  Authors: Yining Sun, Haoyu Kang, Jiajun Wu, Heng Zhang, Danyang Zhang, Zhenjun Zhao, Haochen Han, Fangming Liu, Wai Kin Victor Chan, Alex Jinpeng Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.25592v1.pdf)  
  Keywords: video generation, benchmark, interactive, dit, dynamics, i2v, image-to-video  

### Long Video Generation

*Showing the latest 50 out of 132 papers*

- **[MV-Forcing: Long Multi-View Video Generation via 4D-Grounded Spatio-Temporal Self-Forcing](https://arxiv.org/abs/2607.05376v1)**  
  Authors: Gal Fiebelman, Hadar Averbuch-Elor, Sagie Benaim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.05376v1.pdf)  
  Keywords: denoising, video generation, autoregressive, distillation, video diffusion, multi-view video, diffusion model  
- **[Consistent and Editable: A Balanced Framework for Text-Guided Video Editing](https://arxiv.org/abs/2607.05056v1)**  
  Authors: Tao Jin, Li Xiao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.05056v1.pdf)  
  Keywords: dit, temporal consistency, diffusion model, video editing  
- **[Flex-Forcing: Towards a Unified Autoregressive and Bidirectional Video Diffusion Model](https://arxiv.org/abs/2607.03509v1)**  
  Authors: Xinyin Ma, Julius Berner, Chao Liu, Arash Vahdat, Weili Nie, Xinchao Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.03509v1.pdf)  
  Keywords: denoising, efficient, video generation, streaming, benchmark, autoregressive, video diffusion, diffusion model  
- **[Track the Noise, Move the World:3D-Grounded Motion-Consistent Noise for Controllable Video Generation](https://arxiv.org/abs/2607.02798v1)**  
  Authors: Long Vu, Tan Ngo, Animesh Karnewar, Amir Habibian, Binh-Son Hua, Hung Bui, Minh Hoai Nguyen, Phong Nguyen-Ha  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.02798v1.pdf)  
  Keywords: denoising, video generation, benchmark, video diffusion, dit, temporal consistency, latent video, motion control, controllable, diffusion model, text-to-video  
- **[ICDepth: Taming Video Diffusion Models for Video Depth Estimation via In-Context Conditioning](https://arxiv.org/abs/2607.01677v1)**  
  Authors: Xuanhua He, Jiaxin Xie, Mingzhe Zheng, Qifeng Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.01677v1.pdf)  
  Keywords: benchmark, video diffusion, dit, diffusion transformer, temporal consistency, diffusion model, text-to-video  
- **[Anti-Prompt: Image Protection against Text-Guided Image-to-Video Generation](https://arxiv.org/abs/2607.01499v1)**  
  Authors: Yeonghwan Song, Chanhui Lee, Jinsoo Park, Jeany Son  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.01499v1.pdf)  
  Keywords: denoising, architecture, video generation, evaluation, dit, temporal consistency, i2v, image-to-video  
- **[Pano2World: End-to-End 3D Generation via Unified Multi-View Sequences](https://arxiv.org/abs/2607.00832v2)**  
  Authors: Zhenjia Li, Jinrang Jia, Yifeng Shi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.00832v2.pdf)  
  Keywords: denoising, video generation, benchmark, trajectory, temporal consistency, diffusion model  
- **[Towards Memory-Efficient Autoregressive Video Generation via Instance-Specific Parametric Absorption](https://arxiv.org/abs/2607.00712v1)**  
  Authors: Xiaomeng Fu, Jia Li, Yiming Hu, Yong Wang, Hayden Kwok-Hay So, Jiao Dai, Xiangxiang Chu, Jizhong Han  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.00712v1.pdf)  
  Keywords: efficient, long video, architecture, streaming, video generation, autoregressive, identity  
- **[MemLearner: Learning to Query Context memory for Video World Models](https://arxiv.org/abs/2606.31734v1)**  
  Authors: Jiwen Yu, Jianxiong Gao, Jianhong Bai, Yiran Qin, Kaiyi Huang, Quande Liu, Xintao Wang, Pengfei Wan, Kun Gai, Xihui Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.31734v1.pdf)  
  Keywords: efficient, long video, video generation, interactive, dit, world model  
- **[Bridging Video Understanding and Generation in a Unified Framework](https://arxiv.org/abs/2606.31326v1)**  
  Authors: Yuqi Wang, Runyi Li, Ruoyu Feng, Renjie Chen, Wenfeng Lin, Mingyu Guo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.31326v1.pdf)  
  Keywords: architecture, video generation, benchmark, autoregressive, dynamics  

### Personalization & Customization

*Showing the latest 50 out of 88 papers*

- **[Aura: Consistent Multi-Subject Video Generation via VLM-Grounded Semantic Alignment](https://arxiv.org/abs/2607.04311v1)**  
  Authors: Zixiang Zhou, Zhentao Yu, Yifeng Ma, Hongmei Wang, Wenqing Yu, Cong Wang, Zilin Yang, Rui Chen, Jiarong Ou, Yezhou Liu, Yuan Zhou, Qinglin Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.04311v1.pdf)  
  Keywords: video generation, video synthesis, dit, diffusion transformer, identity, controllable, dynamics, subject-driven  
- **[G$^2$TAM: Geometry Grounded Track Anything Model](https://arxiv.org/abs/2607.03789v1)**  
  Authors: Chenming Zhu, Peizhou Cao, Jingli Lin, Wenbo Hu, Yunlong Ran, Jiangmiao Pang, Tai Wang, Xihui Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.03789v1.pdf)  
  Keywords: benchmark, interactive, identity, evaluation  
- **[TrajLoc: Trajectory-Attention Localization for Multi-Object Motion Control](https://arxiv.org/abs/2607.00861v1)**  
  Authors: Omer Sela, Inbar Huberman-Spiegelglas, Michael Rotman, Sagie Benaim, Avi Ben-Cohen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.00861v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://sela-omer.github.io/traj-loc)  
  Keywords: evaluation, trajectory, dit, motion control, identity, i2v, image-to-video  
- **[Towards Memory-Efficient Autoregressive Video Generation via Instance-Specific Parametric Absorption](https://arxiv.org/abs/2607.00712v1)**  
  Authors: Xiaomeng Fu, Jia Li, Yiming Hu, Yong Wang, Hayden Kwok-Hay So, Jiao Dai, Xiangxiang Chu, Jizhong Han  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.00712v1.pdf)  
  Keywords: efficient, long video, architecture, streaming, video generation, autoregressive, identity  
- **[GeoEdit: Geometry-Aware Object Editing via Dual-Branch Denoising](https://arxiv.org/abs/2606.30003v1)**  
  Authors: Yi He, Jiangming Wang, Xinyu Wang, Mark Fong, Songchun Zhang, Yuxuan Xue, Hai-Tao Zheng, Yue Ma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.30003v1.pdf) | [![GitHub](https://img.shields.io/github/stars/Heey731/GeoEdit?style=social)](https://github.com/Heey731/GeoEdit)  
  Keywords: denoising, evaluation, benchmark, video diffusion, dit, identity, physical  
- **[Semantic-Aware, Physics-Informed, Geometry-Grounded Weather Video Synthesis](https://arxiv.org/abs/2606.29020v1)**  
  Authors: Chenghao Qian, Nedko Savov, Lingdong Kong, Yeying Jin, Rui Song, Wenjing Li, Zhun Zhong, Jiaqi Ma, Gustav Markkula, Luc Van Gool  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.29020v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://jumponthemoon.github.io/w-crafter)  
  Keywords: autonomous driving, video synthesis, simulation, dit, physics, identity, dynamics, physical  
- **[A Good Talk Does not Look Like a Summary, It Teaches You! Measuring Takeaways from Paper-to-Video Talks](https://arxiv.org/abs/2606.28531v1)**  
  Authors: Ishani Mondal, Aparna Garimella, Ananya Sai, Pannaga Shivaswamy, Jordan Boyd-Graber  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.28531v1.pdf)  
  Keywords: concept, video generation, education, evaluation  
- **[EMOSH: Expressive Motion and Shape Disentanglement for Human Animation](https://arxiv.org/abs/2606.28026v1)**  
  Authors: Dongbin Zhang, Hao Liu, Binquan Dai, Kangjie Chen, Chuming Wang, Chen Li, Jing Lyu, Haoqian Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.28026v1.pdf)  
  Keywords: video generation, avatar, human animation, dit, identity, controllable, gesture  
- **[RayPE: Ray-Space Positional Encoding for 3D-Aware Video Generation](https://arxiv.org/abs/2606.27345v2)**  
  Authors: Minghao Yin, Jiahao Lu, Wenbo Hu, Wang Zhao, Shan Ying, Kai Han  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.27345v2.pdf)  
  Keywords: video generation, 3d-aware, video diffusion, dit, camera control, diffusion transformer, identity  
- **[NaviCache: Test-Time Self-Calibration Caching for Video Generation](https://arxiv.org/abs/2606.26795v1)**  
  Authors: Zheqi Lv, Zhibo Zhu, Jinke Wang, Qi Tian, Shengyu Zhang, Zhengyu Chen, Chengxi Zang, Zhou Zhao, Fei Wu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.26795v1.pdf)  
  Keywords: architecture, video generation, concept, trajectory, video diffusion, acceleration, diffusion model  

### Physical Understanding

*Showing the latest 50 out of 158 papers*

- **[FlowMark: Mask-Guided Video Watermarking](https://arxiv.org/abs/2607.05261v1)**  
  Authors: Vishal Asnani, Shruti Agarwal, John Collomosse  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.05261v1.pdf)  
  Keywords: dit, architecture, dynamics  
- **[DSWAM: A Dual-System World Action Foundation Model for Fine-Grained Robot Manipulation](https://arxiv.org/abs/2607.04927v1)**  
  Authors: Jian Zhu, Jianjun Zhang, Taiyi Su, Tianbin Liu, Zhangyuan Wang, Kai Xie, Zitai Huang, Chong Ma, Youzhang He, Tianjian Wang, Hanyang Wang, Weihao Ding, Yi Xu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.04927v1.pdf)  
  Keywords: video generation, evaluation, acceleration, world model, physical  
- **[Video Generation Models Are Inherent Lighting Estimators](https://arxiv.org/abs/2607.04674v1)**  
  Authors: Ziqi Cai, Shuchen Weng, Kaiqi Liu, Zifeng Wang, Zhiquan Zhang, Minggui Teng, Han Jiang, Boxin Shi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.04674v1.pdf)  
  Keywords: efficient, video generation, video diffusion, video inpainting, physical, diffusion model  
- **[Enhancing Video Physical Consistency via Role-aware Joint Training and Modality-decoupled Denoising](https://arxiv.org/abs/2607.04653v1)**  
  Authors: Guangting Zheng, Haojing Chen, Hao Li, Jingtao Zhang, Zhen Yang, Xiaosong Jia, Xue Yang, Shaofeng Zhang, Yanyong Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.04653v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://tom-zgt.github.io/VPT)  
  Keywords: denoising, benchmark, video diffusion, t2v, physics, dynamics, physical, diffusion model  
- **[Mask2Real-WM: Segmentation Masks as a Sim-to-Real Bridge for Controllable Dexterous World Models](https://arxiv.org/abs/2607.04546v1)**  
  Authors: Riccardo O. Feingold, Davide Liconti, Chenyu Yang, Robert K. Katzschmann  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.04546v1.pdf)  
  Keywords: evaluation, benchmark, video diffusion, simulation, dit, action-conditioned, controllable, dynamics, world model, physical  
- **[Aura: Consistent Multi-Subject Video Generation via VLM-Grounded Semantic Alignment](https://arxiv.org/abs/2607.04311v1)**  
  Authors: Zixiang Zhou, Zhentao Yu, Yifeng Ma, Hongmei Wang, Wenqing Yu, Cong Wang, Zilin Yang, Rui Chen, Jiarong Ou, Yezhou Liu, Yuan Zhou, Qinglin Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.04311v1.pdf)  
  Keywords: video generation, video synthesis, dit, diffusion transformer, identity, controllable, dynamics, subject-driven  
- **[Worldscape-MoE: A Unified Mixture-of-Experts World Model for Scalable Heterogeneous Action Control](https://arxiv.org/abs/2607.03964v1)**  
  Authors: Jianjie Fang, Yongyan Xu, Ziyou Wang, Chen Gao, Yuchao Huang, Zhaolu Wang, Rongze Tang, Mingyuan Jia, Baining Zhao, Weichen Zhang, Xin Zhang, Haisheng Su, Yu Shang, Wei Wu, Xinlei Chen, Yong Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.03964v1.pdf)  
  Keywords: video generation, interactive, dit, diffusion transformer, controllable, dynamics, world model, physical  
- **[ProxyUp: Training-Free Proxy-Conditioned Video Generation for Controllable Dynamics](https://arxiv.org/abs/2607.03732v1)**  
  Authors: Zanwei Zhou, Jiazhong Cen, Jiemin Fang, Yumeng He, Chen Yang, Sikuang Li, Fanpeng Meng, Zhikuan Bao, Wei Shen, Qi Tian  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.03732v1.pdf)  
  Keywords: video generation, video editing, simulation, dit, physics, controllable, dynamics, physical  
- **[SafeGuard: A Multi-Agent Perception-Reasoning Framework for Social-Risk AI-Generated Video Detection](https://arxiv.org/abs/2607.03069v1)**  
  Authors: Wenlin Wu, Sheng Zhou, Peipei Song, Wenhao Wang, Junbin Xiao, Xun Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.03069v1.pdf)  
  Keywords: benchmark, physical, video generation, evaluation  
- **[WorldDirector: Building Controllable World Simulators with Persistent Dynamic Memory](https://arxiv.org/abs/2607.02517v1)**  
  Authors: Hanlin Wang, Hao Ouyang, Qiuyu Wang, Wen Wang, Qingyan Bai, Ka Leong Cheng, Yue Yu, Yixuan Li, Yihao Meng, Zichen Liu, Yanhong Zeng, Yujun Shen, Qifeng Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.02517v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://worlddirector.github.io)  
  Keywords: video generation, world simulator, controllable, dynamics, world model, physical  

### Surveys & Benchmarks

*Showing the latest 50 out of 232 papers*

- **[DSWAM: A Dual-System World Action Foundation Model for Fine-Grained Robot Manipulation](https://arxiv.org/abs/2607.04927v1)**  
  Authors: Jian Zhu, Jianjun Zhang, Taiyi Su, Tianbin Liu, Zhangyuan Wang, Kai Xie, Zitai Huang, Chong Ma, Youzhang He, Tianjian Wang, Hanyang Wang, Weihao Ding, Yi Xu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.04927v1.pdf)  
  Keywords: video generation, evaluation, acceleration, world model, physical  
- **[Enhancing Video Physical Consistency via Role-aware Joint Training and Modality-decoupled Denoising](https://arxiv.org/abs/2607.04653v1)**  
  Authors: Guangting Zheng, Haojing Chen, Hao Li, Jingtao Zhang, Zhen Yang, Xiaosong Jia, Xue Yang, Shaofeng Zhang, Yanyong Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.04653v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://tom-zgt.github.io/VPT)  
  Keywords: denoising, benchmark, video diffusion, t2v, physics, dynamics, physical, diffusion model  
- **[Lights, Camera, Carbon: Architectural Scaling Laws for Video Generation Energy Consumption](https://arxiv.org/abs/2607.04553v1)**  
  Authors: Nidhal Jegham, Boris Gamazaychikov, Sasha Luccioni  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.04553v1.pdf)  
  Keywords: efficient, architecture, video generation, benchmark, video diffusion, t2v, dit, diffusion model, text-to-video  
- **[Mask2Real-WM: Segmentation Masks as a Sim-to-Real Bridge for Controllable Dexterous World Models](https://arxiv.org/abs/2607.04546v1)**  
  Authors: Riccardo O. Feingold, Davide Liconti, Chenyu Yang, Robert K. Katzschmann  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.04546v1.pdf)  
  Keywords: evaluation, benchmark, video diffusion, simulation, dit, action-conditioned, controllable, dynamics, world model, physical  
- **[G$^2$TAM: Geometry Grounded Track Anything Model](https://arxiv.org/abs/2607.03789v1)**  
  Authors: Chenming Zhu, Peizhou Cao, Jingli Lin, Wenbo Hu, Yunlong Ran, Jiangmiao Pang, Tai Wang, Xihui Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.03789v1.pdf)  
  Keywords: benchmark, interactive, identity, evaluation  
- **[Flex-Forcing: Towards a Unified Autoregressive and Bidirectional Video Diffusion Model](https://arxiv.org/abs/2607.03509v1)**  
  Authors: Xinyin Ma, Julius Berner, Chao Liu, Arash Vahdat, Weili Nie, Xinchao Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.03509v1.pdf)  
  Keywords: denoising, efficient, video generation, streaming, benchmark, autoregressive, video diffusion, diffusion model  
- **[SafeGuard: A Multi-Agent Perception-Reasoning Framework for Social-Risk AI-Generated Video Detection](https://arxiv.org/abs/2607.03069v1)**  
  Authors: Wenlin Wu, Sheng Zhou, Peipei Song, Wenhao Wang, Junbin Xiao, Xun Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.03069v1.pdf)  
  Keywords: benchmark, physical, video generation, evaluation  
- **[Natural Language Camera Movement Understanding](https://arxiv.org/abs/2607.03043v1)**  
  Authors: Yuwen Tan, Joey Huang, Jin Huang, Haoxiang Li, Boqing Gong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.03043v1.pdf)  
  Keywords: benchmark, video generation  
- **[Track the Noise, Move the World:3D-Grounded Motion-Consistent Noise for Controllable Video Generation](https://arxiv.org/abs/2607.02798v1)**  
  Authors: Long Vu, Tan Ngo, Animesh Karnewar, Amir Habibian, Binh-Son Hua, Hung Bui, Minh Hoai Nguyen, Phong Nguyen-Ha  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.02798v1.pdf)  
  Keywords: denoising, video generation, benchmark, video diffusion, dit, temporal consistency, latent video, motion control, controllable, diffusion model, text-to-video  
- **[NeoMap: Training-free Novel-View Synthesis from Single Images and Videos](https://arxiv.org/abs/2607.01962v1)**  
  Authors: Jinxi Li, Tianyi Zhang, Yafei Yang, Zihui Zhang, Peng Huang, Koon Wing Macgyver Lin, Bo Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.01962v1.pdf)  
  Keywords: denoising, video synthesis, benchmark, dit, novel view  

### Text-to-Video Generation

*Showing the latest 50 out of 70 papers*

- **[Enhancing Video Physical Consistency via Role-aware Joint Training and Modality-decoupled Denoising](https://arxiv.org/abs/2607.04653v1)**  
  Authors: Guangting Zheng, Haojing Chen, Hao Li, Jingtao Zhang, Zhen Yang, Xiaosong Jia, Xue Yang, Shaofeng Zhang, Yanyong Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.04653v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://tom-zgt.github.io/VPT)  
  Keywords: denoising, benchmark, video diffusion, t2v, physics, dynamics, physical, diffusion model  
- **[Lights, Camera, Carbon: Architectural Scaling Laws for Video Generation Energy Consumption](https://arxiv.org/abs/2607.04553v1)**  
  Authors: Nidhal Jegham, Boris Gamazaychikov, Sasha Luccioni  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.04553v1.pdf)  
  Keywords: efficient, architecture, video generation, benchmark, video diffusion, t2v, dit, diffusion model, text-to-video  
- **[HyperVAttention: Efficient Sparse Attention with Spatio-Temporal Clustering for Video Diffusion](https://arxiv.org/abs/2607.03012v1)**  
  Authors: Dongyeun Lee, Amir Zandieh, Vahab Mirrokni, Junmo Kim, Insu Han  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.03012v1.pdf)  
  Keywords: denoising, efficient, video generation, video diffusion, dit, diffusion transformer, text-to-video  
- **[Track the Noise, Move the World:3D-Grounded Motion-Consistent Noise for Controllable Video Generation](https://arxiv.org/abs/2607.02798v1)**  
  Authors: Long Vu, Tan Ngo, Animesh Karnewar, Amir Habibian, Binh-Son Hua, Hung Bui, Minh Hoai Nguyen, Phong Nguyen-Ha  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.02798v1.pdf)  
  Keywords: denoising, video generation, benchmark, video diffusion, dit, temporal consistency, latent video, motion control, controllable, diffusion model, text-to-video  
- **[ICDepth: Taming Video Diffusion Models for Video Depth Estimation via In-Context Conditioning](https://arxiv.org/abs/2607.01677v1)**  
  Authors: Xuanhua He, Jiaxin Xie, Mingzhe Zheng, Qifeng Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.01677v1.pdf)  
  Keywords: benchmark, video diffusion, dit, diffusion transformer, temporal consistency, diffusion model, text-to-video  
- **[Your Data Manifold is Secretly a Reward Model: Shell-LCC for Text-to-Video Generation](https://arxiv.org/abs/2606.30248v1)**  
  Authors: Shihao Zhang, Yuguang Yan, Junzhe Zhang, Wei Zhao, Bohan Wang, Hanwang Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.30248v1.pdf)  
  Keywords: diffusion model, video generation, text-to-video, t2v  
- **[Disco-LoRA: Disentangled Composition of Content, Style, and Motion for Multi-concept Video Customization](https://arxiv.org/abs/2606.26668v1)**  
  Authors: Xuancheng Xu, Gengyun Jia, Bing-Kun Bao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.26668v1.pdf)  
  Keywords: video generation, concept, customization, benchmark, style, t2v, identity, controllable, text-to-video  
- **[SharQ: Bridging Activation Sparsity and FP4 Quantization for LLM Inference](https://arxiv.org/abs/2606.26587v1)**  
  Authors: Haoqian Meng, Yilun Luo, Yafei Zhao, Wenyuan Liu, Huaqing Zheng, Xindian Ma, Peng Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.26587v1.pdf) | [![GitHub](https://img.shields.io/github/stars/actypedef/SharQ?style=social)](https://github.com/actypedef/SharQ)  
  Keywords: video generation, t2v  
- **[DomainShuttle: Freeform Open Domain Subject-driven Text-to-video Generation](https://arxiv.org/abs/2606.26058v1)**  
  Authors: Nan Chen, Yiyang Cai, Rongchang Xie, Junwen Pan, Cheng Chen, Weinan Jia, Zhuowei Chen, Wen Zhou, Zhenbang Sun, Wenhan Luo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.26058v1.pdf)  
  Keywords: video generation, style, personalization, dit, subject-driven, text-to-video  
- **[Causal-rCM: A Unified Teacher-Forcing and Self-Forcing Open Recipe for Autoregressive Diffusion Distillation in Streaming Video Generation and Interactive World Models](https://arxiv.org/abs/2606.25473v1)**  
  Authors: Kaiwen Zheng, Guande He, Min Zhao, Jintao Zhang, Huayu Chen, Jianfei Chen, Chen-Hsuan Lin, Ming-Yu Liu, Jun Zhu, Qianli Ma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.25473v1.pdf)  
  Keywords: video generation, streaming, autoregressive, distillation, interactive, video diffusion, t2v, dit, diffusion transformer, action-conditioned, world model, physical  

### Video Editing

- **[Consistent and Editable: A Balanced Framework for Text-Guided Video Editing](https://arxiv.org/abs/2607.05056v1)**  
  Authors: Tao Jin, Li Xiao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.05056v1.pdf)  
  Keywords: dit, temporal consistency, diffusion model, video editing  
- **[ProxyUp: Training-Free Proxy-Conditioned Video Generation for Controllable Dynamics](https://arxiv.org/abs/2607.03732v1)**  
  Authors: Zanwei Zhou, Jiazhong Cen, Jiemin Fang, Yumeng He, Chen Yang, Sikuang Li, Fanpeng Meng, Zhikuan Bao, Wei Shen, Qi Tian  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.03732v1.pdf)  
  Keywords: video generation, video editing, simulation, dit, physics, controllable, dynamics, physical  
- **[LiveEdit: Towards Real-Time Diffusion-Based Streaming Video Editing](https://arxiv.org/abs/2606.26740v1)**  
  Authors: Xinyu Wang, Chongbo Zhao, Fangneng Zhan, Yue Ma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.26740v1.pdf)  
  Keywords: efficient, streaming, video generation, evaluation, benchmark, distillation, interactive, video editing, dit  
- **[Vera: A Layered Diffusion Model for Content-Preserving Video Editing](https://arxiv.org/abs/2606.23610v1)**  
  Authors: Hongkai Zheng, Ta-Ying Cheng, Benjamin Klein, Yisong Yue, Zhuoning Yuan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.23610v1.pdf)  
  Keywords: architecture, video generation, benchmark, video diffusion, video editing, dit, creative, dynamics, diffusion model, text-to-video  
- **[SteerVTE: Seamless Video Text Editing with Style and Glyph Control](https://arxiv.org/abs/2606.23254v1)**  
  Authors: Kai Zeng, Moran Li, Zhengwei Wang, Yingchen Yu, Yiheng Lin, Ruichuan An, Ming Lu, Qi She, Wentao Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.23254v1.pdf)  
  Keywords: style, video diffusion, video editing, dit, image to video, diffusion transformer, diffusion model  
- **[Generative Relightable Avatars](https://arxiv.org/abs/2606.22718v1)**  
  Authors: Kunwar Maheep Singh, Christian Theobalt, Rishabh Dabral  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.22718v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://vcai.mpi-inf.mpg.de/projects/GRA)  
  Keywords: long video, evaluation, video diffusion, avatar, physics, controllable, dynamics, video-to-video, physical, diffusion model  
- **[ReGenHuman: Re-Generating Human Appearances for Realistic Full-Body Video Anonymization](https://arxiv.org/abs/2606.14972v1)**  
  Authors: Adam Sun, Eshaan Barkataki, Arnold Milstein, Gordon Wetzstein, Ehsan Adeli  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.14972v1.pdf)  
  Keywords: video-to-video, dit, video diffusion, identity  
- **[Lip Forcing: Few-Step Autoregressive Diffusion for Real-time Lip Synchronization](https://arxiv.org/abs/2606.11180v1)**  
  Authors: Paul Hyunbin Cho, Jinhyuk Jang, SeokYoung Lee, Joungbin Lee, Siyoon Jin, Heeseong Shin, Jung Yi, Yunjin Park, Chulmin Park, Seungryong Kim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.11180v1.pdf)  
  Keywords: denoising, streaming, autoregressive, trajectory, video diffusion, dit, video-to-video, diffusion model  
- **[CoVEBench: Can Video Editing Models Handle Complex Instructions?](https://arxiv.org/abs/2606.08415v2)**  
  Authors: Jiangtao Wu, Jiaming Wang, Yiwen He, Yuanxing Zhang, Shihao Li, Dunyuan Liu, Xuedong Zhao, Jialu Chen, Zekun Moore Wang, Jiaheng Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.08415v2.pdf)  
  Keywords: benchmark, dit, style, video editing  
- **[TIDE: Task-Isolated Diffusion for Unified Video Editing and Generation](https://arxiv.org/abs/2606.08260v1)**  
  Authors: Qi Liu, Gang Yue, Mingyu Yin, Lisai Zhang, Yidi Wu, Yaole Wang, Yaohui Wang, Chang Yao, Jingyuan Chen, Lin Ma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.08260v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://LittleWork123.github.io/tide)  
  Keywords: video generation, benchmark, video editing, dit, diffusion transformer  

### Video Inpainting & Completion

- **[Video Generation Models Are Inherent Lighting Estimators](https://arxiv.org/abs/2607.04674v1)**  
  Authors: Ziqi Cai, Shuchen Weng, Kaiqi Liu, Zifeng Wang, Zhiquan Zhang, Minggui Teng, Han Jiang, Boxin Shi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.04674v1.pdf)  
  Keywords: efficient, video generation, video diffusion, video inpainting, physical, diffusion model  
- **[ImageWAM: Do World Action Models Really Need Video Generation, or Just Image Editing?](https://arxiv.org/abs/2606.19531v1)**  
  Authors: Yuyang Zhang, Wenyao Zhang, Zekun Qi, He Zhang, Haitao Lin, Jingbo Zhang, Yao Mu, Xiaokang Yang, Wenjun Zeng, Xin Jin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.19531v1.pdf)  
  Keywords: denoising, video generation, video prediction, dit, world model  
- **[R2RDreamer: 3D-aware Data Augmentation for Spatially-generalized 2D Manipulation Policies](https://arxiv.org/abs/2606.17040v1)**  
  Authors: Xiuwei Xu, Haowen Sun, Angyuan Ma, Yiwei Zhang, Zhenyu Wu, Xiaofeng Wang, Bingyao Yu, Zheng Zhu, Jie Zhou, Jiwen Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17040v1.pdf)  
  Keywords: video completion, style, 3d-aware, simulation, dit, controllable, image-to-video  
- **[PointAction: 3D Points as Universal Action Representations for Robot Control](https://arxiv.org/abs/2606.03943v1)**  
  Authors: Mutian Tong, Han Jiang, Qiao Feng, Lingjie Liu, Jiatao Gu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.03943v1.pdf)  
  Keywords: 4d generation, video generation, video diffusion, simulation, video prediction, dynamics, diffusion model  
- **[World Models: A Comprehensive Survey of Architectures, Methodologies, Reasoning Paradigms, and Applications](https://arxiv.org/abs/2606.00133v1)**  
  Authors: Arif Hassan Zidan, Yi Pan, Hanqi Jiang, Ruiyu Yan, Wei Ruan, Zihao Wu, Lifeng Chen, Weihang You, Xinliang Li, Bowen Chen, Huawen Hu, Peilong Wang, Sizhuang Liu, Jing Zhang, Siyuan Li, Zhengliang Liu, Yu Bao, Lin Zhao, Lichao Sun, Dajiang Zhu, Xiang Li, Jinglei Lv, Quanzheng Li, Wei Liu, Tianming Liu, Wei Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.00133v1.pdf)  
  Keywords: architecture, video generation, evaluation, autonomous driving, benchmark, interactive, education, video prediction, physics, medical, dynamics, world model, robotics, survey  
- **[Full-4D: Generating Full-Scope 4D Scenes from a Single-View Video](https://arxiv.org/abs/2605.25500v1)**  
  Authors: Tingxi Chen, Ke Hao, Yabo Chen, Zhengxue Cheng, Rong Xie, Li Song, Haibin Huang, Chi Zhang, Xuelong Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25500v1.pdf)  
  Keywords: flow matching, 4d generation, video synthesis, distillation, interactive, video diffusion, dit, video interpolation, multi-view video, physical, diffusion model  
- **[CRONOS: Benchmarking Counterfactual Physical Consistency in Video Models](https://arxiv.org/abs/2605.23699v1)**  
  Authors: León Begiristain, Olaf Dünkel, Adam Kortylewski  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.23699v1.pdf)  
  Keywords: evaluation, benchmark, video prediction, dit, dynamics, world model, physical  
- **[GEM-4D: Geometry-Enhanced Video World Models for Robot Manipulation](https://arxiv.org/abs/2605.22882v3)**  
  Authors: Kaichen Zhou, Yuzhen Chen, Fangneng Zhan, Hang Hua, Grace Chen, Xinhai Chang, Ao Qu, Yilun Du, Zhuang Liu, Paul Pu Liang, Mengyu Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.22882v3.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://gem-4d.github.io)  
  Keywords: architecture, simulation, video prediction, dit, dynamics, world model, physical  
- **[Goodbye Drift: Anchored Tree Sampling for Long-Horizon Video-to-Video Generation](https://arxiv.org/abs/2605.20476v1)**  
  Authors: Matthew Bendel, Stephen W. Bailey, Mithilesh Vaidya, Sumukh Badam, Xingzhe He  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20476v1.pdf)  
  Keywords: video generation, autoregressive, distillation, style, t2v, dit, outpainting, video-to-video  
- **[Nano World Models: A Minimalist Implementation of Future Video Prediction](https://arxiv.org/abs/2605.23993v2)**  
  Authors: Siqiao Huang, Partha Kaushik, Michael Chen, Hengkai Pan, Kaiwen Geng, Omar Chehab, Fernando Moreno-Pino, Max Simchowitz  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.23993v2.pdf)  
  Keywords: architecture, video generation, evaluation, autoregressive, interactive, simulation, video prediction, dit, world model  

### Video Super-Resolution & Enhancement

*Showing the latest 50 out of 70 papers*

- **[MV-Forcing: Long Multi-View Video Generation via 4D-Grounded Spatio-Temporal Self-Forcing](https://arxiv.org/abs/2607.05376v1)**  
  Authors: Gal Fiebelman, Hadar Averbuch-Elor, Sagie Benaim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.05376v1.pdf)  
  Keywords: denoising, video generation, autoregressive, distillation, video diffusion, multi-view video, diffusion model  
- **[Enhancing Video Physical Consistency via Role-aware Joint Training and Modality-decoupled Denoising](https://arxiv.org/abs/2607.04653v1)**  
  Authors: Guangting Zheng, Haojing Chen, Hao Li, Jingtao Zhang, Zhen Yang, Xiaosong Jia, Xue Yang, Shaofeng Zhang, Yanyong Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.04653v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://tom-zgt.github.io/VPT)  
  Keywords: denoising, benchmark, video diffusion, t2v, physics, dynamics, physical, diffusion model  
- **[CineMobile: On-Device Image-to-Video Diffusion for Cinematic Camera Motion Generation](https://arxiv.org/abs/2607.03803v1)**  
  Authors: Xuyao Huang, Zelai Deng, Xu Wang, Xizhong Xiao, Zhijie Deng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.03803v1.pdf)  
  Keywords: denoising, efficient, architecture, video generation, distillation, video diffusion, dit, diffusion transformer, image-to-video  
- **[Flex-Forcing: Towards a Unified Autoregressive and Bidirectional Video Diffusion Model](https://arxiv.org/abs/2607.03509v1)**  
  Authors: Xinyin Ma, Julius Berner, Chao Liu, Arash Vahdat, Weili Nie, Xinchao Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.03509v1.pdf)  
  Keywords: denoising, efficient, video generation, streaming, benchmark, autoregressive, video diffusion, diffusion model  
- **[HyperVAttention: Efficient Sparse Attention with Spatio-Temporal Clustering for Video Diffusion](https://arxiv.org/abs/2607.03012v1)**  
  Authors: Dongyeun Lee, Amir Zandieh, Vahab Mirrokni, Junmo Kim, Insu Han  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.03012v1.pdf)  
  Keywords: denoising, efficient, video generation, video diffusion, dit, diffusion transformer, text-to-video  
- **[Track the Noise, Move the World:3D-Grounded Motion-Consistent Noise for Controllable Video Generation](https://arxiv.org/abs/2607.02798v1)**  
  Authors: Long Vu, Tan Ngo, Animesh Karnewar, Amir Habibian, Binh-Son Hua, Hung Bui, Minh Hoai Nguyen, Phong Nguyen-Ha  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.02798v1.pdf)  
  Keywords: denoising, video generation, benchmark, video diffusion, dit, temporal consistency, latent video, motion control, controllable, diffusion model, text-to-video  
- **[NeoMap: Training-free Novel-View Synthesis from Single Images and Videos](https://arxiv.org/abs/2607.01962v1)**  
  Authors: Jinxi Li, Tianyi Zhang, Yafei Yang, Zihui Zhang, Peng Huang, Koon Wing Macgyver Lin, Bo Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.01962v1.pdf)  
  Keywords: denoising, video synthesis, benchmark, dit, novel view  
- **[Anti-Prompt: Image Protection against Text-Guided Image-to-Video Generation](https://arxiv.org/abs/2607.01499v1)**  
  Authors: Yeonghwan Song, Chanhui Lee, Jinsoo Park, Jeany Son  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.01499v1.pdf)  
  Keywords: denoising, architecture, video generation, evaluation, dit, temporal consistency, i2v, image-to-video  
- **[Pano2World: End-to-End 3D Generation via Unified Multi-View Sequences](https://arxiv.org/abs/2607.00832v2)**  
  Authors: Zhenjia Li, Jinrang Jia, Yifeng Shi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.00832v2.pdf)  
  Keywords: denoising, video generation, benchmark, trajectory, temporal consistency, diffusion model  
- **[RotateAttention: RoPE-Aware Rotation and Range Rectification for INT4 Quantized Attention in Video Generation](https://arxiv.org/abs/2607.02584v1)**  
  Authors: Yaofu Liu, Wanli Lan, Jinxi Li, Binhang Yuan, Harry Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.02584v1.pdf)  
  Keywords: denoising, efficient, video generation, dit, acceleration  

### World Models & Simulation

*Showing the latest 50 out of 128 papers*

- **[DSWAM: A Dual-System World Action Foundation Model for Fine-Grained Robot Manipulation](https://arxiv.org/abs/2607.04927v1)**  
  Authors: Jian Zhu, Jianjun Zhang, Taiyi Su, Tianbin Liu, Zhangyuan Wang, Kai Xie, Zitai Huang, Chong Ma, Youzhang He, Tianjian Wang, Hanyang Wang, Weihao Ding, Yi Xu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.04927v1.pdf)  
  Keywords: video generation, evaluation, acceleration, world model, physical  
- **[Mask2Real-WM: Segmentation Masks as a Sim-to-Real Bridge for Controllable Dexterous World Models](https://arxiv.org/abs/2607.04546v1)**  
  Authors: Riccardo O. Feingold, Davide Liconti, Chenyu Yang, Robert K. Katzschmann  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.04546v1.pdf)  
  Keywords: evaluation, benchmark, video diffusion, simulation, dit, action-conditioned, controllable, dynamics, world model, physical  
- **[Worldscape-MoE: A Unified Mixture-of-Experts World Model for Scalable Heterogeneous Action Control](https://arxiv.org/abs/2607.03964v1)**  
  Authors: Jianjie Fang, Yongyan Xu, Ziyou Wang, Chen Gao, Yuchao Huang, Zhaolu Wang, Rongze Tang, Mingyuan Jia, Baining Zhao, Weichen Zhang, Xin Zhang, Haisheng Su, Yu Shang, Wei Wu, Xinlei Chen, Yong Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.03964v1.pdf)  
  Keywords: video generation, interactive, dit, diffusion transformer, controllable, dynamics, world model, physical  
- **[G$^2$TAM: Geometry Grounded Track Anything Model](https://arxiv.org/abs/2607.03789v1)**  
  Authors: Chenming Zhu, Peizhou Cao, Jingli Lin, Wenbo Hu, Yunlong Ran, Jiangmiao Pang, Tai Wang, Xihui Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.03789v1.pdf)  
  Keywords: benchmark, interactive, identity, evaluation  
- **[ProxyUp: Training-Free Proxy-Conditioned Video Generation for Controllable Dynamics](https://arxiv.org/abs/2607.03732v1)**  
  Authors: Zanwei Zhou, Jiazhong Cen, Jiemin Fang, Yumeng He, Chen Yang, Sikuang Li, Fanpeng Meng, Zhikuan Bao, Wei Shen, Qi Tian  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.03732v1.pdf)  
  Keywords: video generation, video editing, simulation, dit, physics, controllable, dynamics, physical  
- **[Vidu S1: A Real-Time Interactive Video Generation Model](https://arxiv.org/abs/2607.03118v1)**  
  Authors: Jintao Zhang, Kai Jiang, Jintao Chen, Xu Wang, Yang Luo, Yuji Wang, Dechuang Chen, Jungang Li, Chengyang Ye, Marco Chen, Hongzhou Zhu, Min Zhao, Yuxuan Jiang, Zhengkun Huang, Chendong Xiang, Kaiwen Zheng, Haoxu Wang, Xiaohang Wang, Qi Jia, Xin Chen, Yimin Chen, Youhe Jiang, Fangcheng Fu, Zhijie Deng, Fan Bao, Jianfei Chen, Jun Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.03118v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://vidu.com/vidu-stream)  
  Keywords: interactive, video generation  
- **[WorldDirector: Building Controllable World Simulators with Persistent Dynamic Memory](https://arxiv.org/abs/2607.02517v1)**  
  Authors: Hanlin Wang, Hao Ouyang, Qiuyu Wang, Wen Wang, Qingyan Bai, Ka Leong Cheng, Yue Yu, Yixuan Li, Yihao Meng, Zichen Liu, Yanhong Zeng, Yujun Shen, Qifeng Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.02517v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://worlddirector.github.io)  
  Keywords: video generation, world simulator, controllable, dynamics, world model, physical  
- **[RetailSMV: Exocentric vs. Egocentric Adaptation of Foundation Video World Models in Retail](https://arxiv.org/abs/2607.00310v1)**  
  Authors: Amirreza Rouhi, Rajat Aggarwal, Parikshit Sakurikar, Anoop M. Namboodiri, Sashi P. Reddi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.00310v1.pdf)  
  Keywords: efficient, world simulator, video diffusion, world model, diffusion model  
- **[MemLearner: Learning to Query Context memory for Video World Models](https://arxiv.org/abs/2606.31734v1)**  
  Authors: Jiwen Yu, Jianxiong Gao, Jianhong Bai, Yiran Qin, Kaiyi Huang, Quande Liu, Xintao Wang, Pengfei Wan, Kun Gai, Xihui Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.31734v1.pdf)  
  Keywords: efficient, long video, video generation, interactive, dit, world model  
- **[UnfoldArt: Zero-Shot Recovery of Full Articulated 3D Objects from Text or Image](https://arxiv.org/abs/2606.30608v2)**  
  Authors: Mohamed el Amine Boudjoghra, Ivan Laptev, Angela Dai  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.30608v2.pdf)  
  Keywords: dit, interactive, robotics  



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
