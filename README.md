# Awesome Video Diffusions [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of latest research papers, projects and resources related to Video Diffusion Models and Video Generation. Content is automatically updated daily.

> Last Update: 2026-06-13 03:46:42

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

- [3D-aware Video Generation](#3d-aware-video-generation) (21 papers) - Video generation with 3D awareness, multi-view consistency, and 4D content creation
- [Applications](#applications) (53 papers) - Domain-specific applications of video diffusion models
- [Architecture & Efficiency](#architecture-&-efficiency) (358 papers) - Architectural innovations (DiT, UNet), flow matching, and training/inference efficiency
- [Audio & Multi-modal](#audio-&-multi-modal) (34 papers) - Audio-driven and multi-modal conditioned video generation
- [Controllable Generation](#controllable-generation) (123 papers) - Controllable video generation with motion, camera, pose, or layout guidance
- [Human & Character Animation](#human-&-character-animation) (23 papers) - Human-centric video generation including talking heads, dance, and character animation
- [Image-to-Video Generation](#image-to-video-generation) (40 papers) - Methods for animating still images into videos
- [Long Video Generation](#long-video-generation) (135 papers) - Generating temporally consistent long-form videos beyond short clips
- [Personalization & Customization](#personalization-&-customization) (85 papers) - Personalized video generation with custom subjects, identities, or styles
- [Physical Understanding](#physical-understanding) (141 papers) - Physics-aware video generation and dynamics modeling
- [Surveys & Benchmarks](#surveys-&-benchmarks) (236 papers) - Survey papers, benchmarks, and evaluation metrics for video generation
- [Text-to-Video Generation](#text-to-video-generation) (54 papers) - Foundation models and methods for generating videos from text prompts
- [Video Editing](#video-editing) (29 papers) - Diffusion-based video editing, style transfer, and manipulation
- [Video Inpainting & Completion](#video-inpainting-&-completion) (9 papers) - Video inpainting, completion, outpainting, and temporal prediction
- [Video Super-Resolution & Enhancement](#video-super-resolution-&-enhancement) (74 papers) - Video quality improvement, upscaling, restoration, and frame interpolation
- [World Models & Simulation](#world-models-&-simulation) (124 papers) - Video generation as world simulators and interactive environment generation



## Table of Contents

- [Categorized Papers](#categorized-papers)
- [Classic Papers](#classic-papers)
- [Open Source Projects](#open-source-projects)
- [Applications](#applications)
- [Tutorials & Blogs](#tutorials--blogs)





## Categorized Papers

### 3D-aware Video Generation

- **[Flex4DHuman: Flexible Multi-view Video Diffusion for 4D Human Reconstruction](https://arxiv.org/abs/2606.13655v1)**  
  Authors: Jen-Hao Cheng, Yipeng Wang, Hao Zhang, Gengshan Yang, Jenq-Neng Hwang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13655v1.pdf)  
  Keywords: architecture, simulation, diffusion model, text-to-video, multi-view video, video diffusion, dit  
- **[Latent Spatial Memory for Video World Models](https://arxiv.org/abs/2606.09828v1)**  
  Authors: Weijie Wang, Haoyu Zhao, Yifan Yang, Feng Chen, Zeyu Zhang, Yefei He, Zicheng Duan, Donny Y. Chen, Yuqing Yang, Bohan Zhuang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.09828v1.pdf)  
  Keywords: world model, diffusion model, novel view, depth-guided, video generation  
- **[CP4D: Compositional Physics-aware 4D Scene Generation](https://arxiv.org/abs/2606.09187v1)**  
  Authors: Hanxin Zhu, Cong Wang, Tianyu He, Long Chen, Xin Jin, Chen Gao, Zhibo Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.09187v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://anonymous.4open.science/w/CP4D)  
  Keywords: dynamics, physics, diffusion model, 4d generation, physical, physics-aware, interactive, video diffusion  
- **[RigPAPR: Rig-Based Animation of Static Neural Point Clouds from a Fixed-Viewpoint Video](https://arxiv.org/abs/2606.06685v1)**  
  Authors: Shichong Peng, Yanshu Zhang, Ke Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.06685v1.pdf)  
  Keywords: novel view, i2v, image-to-video  
- **[PointAction: 3D Points as Universal Action Representations for Robot Control](https://arxiv.org/abs/2606.03943v1)**  
  Authors: Mutian Tong, Han Jiang, Qiao Feng, Lingjie Liu, Jiatao Gu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.03943v1.pdf)  
  Keywords: dynamics, simulation, diffusion model, 4d generation, video generation, video prediction, video diffusion  
- **[RoboDream: Compositional World Models for Scalable Robot Data Synthesis](https://arxiv.org/abs/2606.02577v1)**  
  Authors: Junjie Ye, Rong Xue, Basile Van Hoorick, Runhao Li, Harshitha Rajaprakash, Pavel Tokmakov, Muhammad Zubair Irshad, Vitor Guizilini, Yue Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.02577v1.pdf)  
  Keywords: world model, diffusion model, novel view, physical, trajectory, video diffusion, dit  
- **[Towards 3D-Aware Video Diffusion Models: Render-Free Human Motion Control with Mesh Tokenization](https://arxiv.org/abs/2606.02000v1)**  
  Authors: Jingyun Liang, Min Wei, Shikai Li, Yizeng Han, Hangjie Yuan, Lei Sun, Weihua Chen, Fan Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.02000v1.pdf)  
  Keywords: architecture, 3d-aware, diffusion model, motion control, benchmark, human motion, trajectory, video generation, video diffusion, dit  
- **[Effective Multi-sensor Conditioning for Street-view Novel-view Synthesis](https://arxiv.org/abs/2606.01590v1)**  
  Authors: Zhengfei Kuang, Adam Sun, Liyuan Zhu, Tong Wu, Shengqu Cai, Jonathan Tremblay, Iro Armeni, Ehsan Adeli, Lior Yariv, Gordon Wetzstein  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.01590v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://streetnvs.github.io)  
  Keywords: diffusion model, novel view, trajectory, video diffusion, dit  
- **[Real2SAM2Real: Generative 3D Caches as Complementary Context for Video Diffusion](https://arxiv.org/abs/2606.00299v1)**  
  Authors: Jiayi Wu, Haoming Cai, Cornelia Fermuller, Christopher Metzler, Yiannis Aloimonos  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.00299v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://jiayi-wu-leo.github.io/real2sam2real)  
  Keywords: dynamics, 3d-aware, diffusion model, temporal consistency, video diffusion, dit  
- **[Robust Dreamer: Deviation-Aware Latent Gaussian Memory for Action-Controlled AR Video Generation](https://arxiv.org/abs/2605.30855v2)**  
  Authors: Hanlin Chen, Jiaxin Wei, Xibin Song, Yifu Wang, Steve Wang, Hongdong Li, Pan Ji, Gim Hee Lee  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30855v2.pdf)  
  Keywords: denoising, simulation, autoregressive, 3d-aware, image-to-video, video generation, interactive, dit  

### Applications

*Showing the latest 50 out of 53 papers*

- **[World Model Self-Distillation: Training World Models to Solve General Tasks](https://arxiv.org/abs/2606.12072v1)**  
  Authors: Sebastian Stapf, Pablo Acuaviva Huertos, Aram Davtyan, Paolo Favaro  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.12072v1.pdf)  
  Keywords: world model, evaluation, diffusion model, distillation, robotics, benchmark, video diffusion, dit  
- **[CineDance: Towards Next-Generation Multi-Shot Long-Form Cinematic Audio-Video Generation](https://arxiv.org/abs/2606.09639v2)**  
  Authors: Yuheng Chen, Teng Hu, Yuji Wang, Qingdong He, Zhucun Xue, Qianyu Zhou, Jason Li, Lizhuang Ma, Jiangning Zhang, Dacheng Tao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.09639v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://aliothchen.github.io/projects/CineDance)  
  Keywords: long-form, video generation, film, evaluation  
- **[CapRL++: Unified Reinforcement Learning with Verifiable Rewards for Dense Image and Video Captioning](https://arxiv.org/abs/2606.09393v1)**  
  Authors: Penghui Yang, Long Xing, Xiaoyi Dong, Yuhang Zang, Yuhang Cao, Yibin Wang, Yujie Zhou, Jiazi Bu, Jianze Liang, Qidong Huang, Jiaqi Wang, Feng Wu, Dahua Lin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.09393v1.pdf)  
  Keywords: creative, benchmark, evaluation, dit  
- **[LongSpace: Exploring Long-Horizon Spatial Memory from Perception to Recall in Video](https://arxiv.org/abs/2606.05677v1)**  
  Authors: Shiqiang Lang, Jing Liu, Haoyang He, Peiwen Sun, Yuanteng Chen, Tao Liu, Lan Yang, Longteng Guo, Honggang Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.05677v1.pdf)  
  Keywords: autonomous driving, long video, layout, benchmark  
- **[Auteur: Language-Driven Cinematographic Framing for Human-Centric Video Generation](https://arxiv.org/abs/2606.01900v1)**  
  Authors: Muhammed Burak Kizil, Enes Sanli, Niloy J. Mitra, Xuelin Chen, Erkut Erdem, Aykut Erdem, Duygu Ceylan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.01900v1.pdf)  
  Keywords: video generation, film, camera control, human motion  
- **[PAI-Studio: Cinematic Video Background Replacement with Camera-Aware Motion](https://arxiv.org/abs/2606.01399v1)**  
  Authors: Heyuan Gao, Bangxun Tang, Yiren Song, Guian Fang, Zijian He, Jie Yang, Mike Zheng Shou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.01399v1.pdf)  
  Keywords: dynamics, architecture, diffusion transformer, video synthesis, evaluation, identity, film, dit  
- **[AlbedoEdit: Unified Instance-Level Video Editing with Albedo Guidance](https://arxiv.org/abs/2606.01362v1)**  
  Authors: Xilong Zhou, Bao-Huy Nguyen, Zheng Zeng, Jacob Munkberg, Jon Hasselgren, Thomas Leimkühler, Nima Kalantari, Miloš Hašan, Christian Theobalt  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.01362v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://vcai.mpi-inf.mpg.de/projects/AlbedoEdit)  
  Keywords: video editing, creative, dit  
- **[SKIP: Sparse Keyframe Interpolation Paradigm for Efficient Embodied World Models](https://arxiv.org/abs/2606.00664v1)**  
  Authors: Ziheng He, Yixiang Chen, Ning Yang, Zhanqian Wu, Qisen Ma, Yuan Xu, Jiabing Yang, Peiyan Li, Xiangnan Wu, Xiaofeng Wang, Zheng Zhu, Jing Liu, Nianfeng Liu, Yan Huang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.00664v1.pdf)  
  Keywords: world model, action-conditioned, simulation, diffusion model, robotics, efficient, frame interpolation, video diffusion, dit  
- **[Foundation VAEs for 3D CT Reconstruction, Augmentation, and Generation](https://arxiv.org/abs/2605.30893v1)**  
  Authors: Qi Chen, Shuhan Ding, Yu Gu, Nan Liu, Jiang Bian, Alan Yuille, Zongwei Zhou, Jingjing Fu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30893v1.pdf) | [![GitHub](https://img.shields.io/github/stars/qic999/Foundation-VAE?style=social)](https://github.com/qic999/Foundation-VAE)  
  Keywords: diffusion model, medical, dit  
- **[World Models: A Comprehensive Survey of Architectures, Methodologies, Reasoning Paradigms, and Applications](https://arxiv.org/abs/2606.00133v1)**  
  Authors: Arif Hassan Zidan, Yi Pan, Hanqi Jiang, Ruiyu Yan, Wei Ruan, Zihao Wu, Lifeng Chen, Weihang You, Xinliang Li, Bowen Chen, Huawen Hu, Peilong Wang, Sizhuang Liu, Jing Zhang, Siyuan Li, Zhengliang Liu, Yu Bao, Lin Zhao, Lichao Sun, Dajiang Zhu, Xiang Li, Jinglei Lv, Quanzheng Li, Wei Liu, Tianming Liu, Wei Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.00133v1.pdf)  
  Keywords: interactive, education, dynamics, architecture, medical, world model, survey, evaluation, physics, robotics, benchmark, video generation, video prediction, autonomous driving  

### Architecture & Efficiency

*Showing the latest 50 out of 358 papers*

- **[Flex4DHuman: Flexible Multi-view Video Diffusion for 4D Human Reconstruction](https://arxiv.org/abs/2606.13655v1)**  
  Authors: Jen-Hao Cheng, Yipeng Wang, Hao Zhang, Gengshan Yang, Jenq-Neng Hwang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13655v1.pdf)  
  Keywords: architecture, simulation, diffusion model, text-to-video, multi-view video, video diffusion, dit  
- **[World Tracing: Generative Pixel-Aligned Geometry Beyond the Visible](https://arxiv.org/abs/2606.13652v1)**  
  Authors: Hao Zhang, Mohamed El Banani, Jen-Hao Cheng, Paul Zhang, Yi Hua, Ben Mildenhall, Christoph Lassner, Narendra Ahuja, Gengshan Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13652v1.pdf)  
  Keywords: diffusion transformer, video synthesis, denoising, flow matching, benchmark, dit  
- **[GF-DiT: Scheduling Parallelism for Diffusion Transformer Serving](https://arxiv.org/abs/2606.13501v1)**  
  Authors: Xinwei Qiang, Yifan Hu, Shixuan Sun, Jing Yang, Han Zhao, Chen Chen, Yu Feng, Jingwen Leng, Minyi Guo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13501v1.pdf)  
  Keywords: architecture, diffusion transformer, trajectory, video generation, efficient, video diffusion, dit  
- **[HYDRA-X: Native Unified Multimodal Models with Holistic Visual Tokenizers](https://arxiv.org/abs/2606.13289v1)**  
  Authors: Guozhen Zhang, Xuerui Qiu, Yutao Cui, Tianhui Song, Changlin Li, Junzhe Li, Tao Huang, Xiao Zhang, Yang Li, Jianbing Wu, Miles Yang, Zhao Zhong, Liefeng Bo, Limin Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13289v1.pdf)  
  Keywords: efficient, dit  
- **[TetherCache: Stabilizing Autoregressive Long-Form Video Generation with Gated Recall and Trusted Alignment](https://arxiv.org/abs/2606.13035v1)**  
  Authors: Yu Meng, Xiangyang Luo, Letian Li, Wenyuan Jiang, Chen Gao, Xinlei Chen, Yong Li, Xiao-Ping Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13035v1.pdf)  
  Keywords: streaming, long video, diffusion model, autoregressive, long-form, video generation, video diffusion, dit  
- **[MSUE: Multi-Modal Soccer Understanding Expert](https://arxiv.org/abs/2606.12106v1)**  
  Authors: Litao Li, Yibo Yu, Yufeng Hu, Zhuo Yang, Jiali Wen, Yixin Chen, Yixi Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.12106v1.pdf)  
  Keywords: long-form, multi-modal, architecture, benchmark  
- **[World Model Self-Distillation: Training World Models to Solve General Tasks](https://arxiv.org/abs/2606.12072v1)**  
  Authors: Sebastian Stapf, Pablo Acuaviva Huertos, Aram Davtyan, Paolo Favaro  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.12072v1.pdf)  
  Keywords: world model, evaluation, diffusion model, distillation, robotics, benchmark, video diffusion, dit  
- **[SpecLoR: Spectral Lookahead Rectification for Motion-Coherent Text-to-Video Generation](https://arxiv.org/abs/2606.11969v1)**  
  Authors: Xu Zhang, Yu Lu, Ruijie Quan, Zhaozheng Chen, Bohan Wang, Yi Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.11969v1.pdf)  
  Keywords: flow matching, text-to-video, benchmark, physical, video generation, dit  
- **[Plan-and-Verify Video Reward Reasoning with Spatio-Temporal Scene Graph Grounding](https://arxiv.org/abs/2606.11838v1)**  
  Authors: Hyomin Kim, Junghye Kim, Joanie Hayoun Chung, Yoonjin Oh, Kyungjae Lee, Sungbin Lim, Sungwoong Kim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.11838v1.pdf)  
  Keywords: text-to-video, dit, t2v  
- **[A Comprehensive Ecosystem for Open-Domain Customized Video Generation](https://arxiv.org/abs/2606.11783v1)**  
  Authors: Jingxu Zhang, Yuqian Hong, Daneul Kim, Kai Qiu, Qi Dai, Jianmin Bao, Yifan Yang, Xiaoyan Sun, Chong Luo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.11783v1.pdf)  
  Keywords: diffusion transformer, identity, benchmark, video generation, efficient, dit  

### Audio & Multi-modal

- **[ReFree: Towards Realistic Co-Speech Video Generation via Reward-Free RL and Multilevel Speech Guidance](https://arxiv.org/abs/2606.13304v1)**  
  Authors: Salaheldin Mohamed, M. Hamza Mughal, Rishabh Dabral, Christian Theobalt  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13304v1.pdf)  
  Keywords: video generation, speech-driven, evaluation  
- **[MSUE: Multi-Modal Soccer Understanding Expert](https://arxiv.org/abs/2606.12106v1)**  
  Authors: Litao Li, Yibo Yu, Yufeng Hu, Zhuo Yang, Jiali Wen, Yixin Chen, Yixi Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.12106v1.pdf)  
  Keywords: long-form, multi-modal, architecture, benchmark  
- **[Conan-embedding-v3: Fusing Modality-Specific Models for Omni-Modal Embedding](https://arxiv.org/abs/2606.09331v1)**  
  Authors: Shiyu Li, Zhiyuan Hu, Yifan Wang, Peiming Li, Zheng Wei, Yang Tang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.09331v1.pdf)  
  Keywords: dynamics, multi-modal, architecture  
- **[EgoPressDiff: Multimodal Video Diffusion for Egocentric UV-Domain Hand-Pressure Estimation](https://arxiv.org/abs/2606.06872v1)**  
  Authors: Yuan Zeng, Zilue Gao, Yujia Shi, Zongqing Lu, Wenming Yang, QingMin Liao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.06872v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://egopressdiff.github.io)  
  Keywords: multi-modal, physical, efficient, video diffusion, dit  
- **[Mamba-Enhanced Implicit Motion Learning for Audio-Driven Portrait Animation](https://arxiv.org/abs/2606.03402v2)**  
  Authors: Xuan Wei, Jiahui Chen, Kaiheng Li, Mingyu Shao, Qingqi Hong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.03402v2.pdf)  
  Keywords: dynamics, architecture, audio-driven, diffusion model, gesture, human motion, benchmark, video generation, human animation  
- **[Inference-Time Scaling for Joint Audio-Video Generation](https://arxiv.org/abs/2606.03183v1)**  
  Authors: Jaemin Jung, Kyeongha Rho, Inkyu Shin, Joon Son Chung  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.03183v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://jung-jaemin.github.io/ITS-AVGen-Proj)  
  Keywords: sound, video generation, benchmark  
- **[Cohort-Scale Neural Atlases of Ultrasound Video](https://arxiv.org/abs/2606.00890v1)**  
  Authors: Zhuorui Zhang, Roger Pallarès-López, Xuan Wu, Praneeth Namburi, Brian W. Anthony  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.00890v1.pdf)  
  Keywords: sound  
- **[LongCat-Video-Avatar 1.5 Technical Report](https://arxiv.org/abs/2605.26486v1)**  
  Authors: Meituan LongCat Team, Xunliang Cai, Meng Cheng, Feng Gao, Zhe Kong, Jiamu Li, Le Li, Weiheng Li, Hongyu Liu, Shuai Tan, Xiaoming Wei, Tianyu Yang, Yong Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.26486v1.pdf)  
  Keywords: audio-driven, evaluation, identity, avatar, distillation, benchmark, video generation, dit  
- **[StreamChar: Long-Horizon Streaming Character Audio-Video Generation with Decoupled Orchestration](https://arxiv.org/abs/2605.25659v1)**  
  Authors: Linrui Tian, Qi Wang, Bang Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25659v1.pdf)  
  Keywords: audio-driven, streaming, denoising, autoregressive, identity, distillation, video generation, efficient, dit  
- **[Test-Time Self-Adaptive Conditioning for Stable Audio-Driven Talking-Head Generation](https://arxiv.org/abs/2605.25488v1)**  
  Authors: Zhicheng Zhang, Lei Wang, Yu Zhang, Yongsheng Gao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25488v1.pdf)  
  Keywords: dynamics, audio-driven, identity, benchmark, video generation, dit  

### Controllable Generation

*Showing the latest 50 out of 123 papers*

- **[GF-DiT: Scheduling Parallelism for Diffusion Transformer Serving](https://arxiv.org/abs/2606.13501v1)**  
  Authors: Xinwei Qiang, Yifan Hu, Shixuan Sun, Jing Yang, Han Zhao, Chen Chen, Yu Feng, Jingwen Leng, Minyi Guo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13501v1.pdf)  
  Keywords: architecture, diffusion transformer, trajectory, video generation, efficient, video diffusion, dit  
- **[Lip Forcing: Few-Step Autoregressive Diffusion for Real-time Lip Synchronization](https://arxiv.org/abs/2606.11180v1)**  
  Authors: Paul Hyunbin Cho, Jinhyuk Jang, SeokYoung Lee, Joungbin Lee, Siyoon Jin, Heeseong Shin, Jung Yi, Yunjin Park, Chulmin Park, Seungryong Kim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.11180v1.pdf)  
  Keywords: streaming, video-to-video, denoising, autoregressive, diffusion model, trajectory, video diffusion, dit  
- **[Flow-DPPO: Divergence Proximal Policy Optimization for Flow Matching Models](https://arxiv.org/abs/2606.11025v1)**  
  Authors: Bowen Ping, Xiangxin Zhou, Penghui Qi, Minnan Luo, Liefeng Bo, Tianyu Pang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.11025v1.pdf) | [![GitHub](https://img.shields.io/github/stars/Tencent-Hunyuan/UniRL?style=social)](https://github.com/Tencent-Hunyuan/UniRL)  
  Keywords: denoising, flow matching, style, trajectory, video generation  
- **[HarmoView: Harmonizing Multi-View Constraints for Identity-Consistent Video Generation](https://arxiv.org/abs/2606.10839v1)**  
  Authors: Cong Wang, Zhentao Yu, Hongmei Wang, Weicong Liang, Zixiang Zhou, Zilin Yang, Jiarong Ou, Rui Chen, Yuan Zhou, Qinglin Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.10839v1.pdf)  
  Keywords: evaluation, identity, layout, t2v, benchmark, video generation, dit  
- **[Making Time Editable in Video Diffusion Transformers](https://arxiv.org/abs/2606.10183v1)**  
  Authors: Konstantin Kuklev, Viacheslav Vasilev, Alexander Kunitsyn, Andrei Ivaniuta, Denis Dimitrov  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.10183v1.pdf)  
  Keywords: dynamics, diffusion transformer, video generation, controllable, video diffusion, dit  
- **[BiWM: Advancing Open-Source Interactive Video World Models with Bidirectional Autoregression](https://arxiv.org/abs/2606.10135v2)**  
  Authors: Shaohao Rui, Xiaofeng Mao, Zhanyu Zhang, Peijia Lin, Yansong Zhu, Yibo Zhang, Haibin Wan, Weijie Ma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.10135v2.pdf)  
  Keywords: dynamics, camera control, world model, simulation, autoregressive, diffusion model, distillation, style, controllable, interactive, video diffusion  
- **[Latent Spatial Memory for Video World Models](https://arxiv.org/abs/2606.09828v1)**  
  Authors: Weijie Wang, Haoyu Zhao, Yifan Yang, Feng Chen, Zeyu Zhang, Yefei He, Zicheng Duan, Donny Y. Chen, Yuqing Yang, Bohan Zhuang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.09828v1.pdf)  
  Keywords: world model, diffusion model, novel view, depth-guided, video generation  
- **[MilliVid: Hierarchical Latents for Long-Range Consistency in Video Generation](https://arxiv.org/abs/2606.09056v1)**  
  Authors: Ishaan Preetam Chandratreya, David Charatan, Basile Van Hoorick, Sergey Zakharov, Vitor Guizilini, Phillip Isola, Vincent Sitzmann  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.09056v1.pdf)  
  Keywords: video generation, diffusion model, layout, video diffusion  
- **[DisCo: World Models with Discrete Camera Motion Control](https://arxiv.org/abs/2606.07967v1)**  
  Authors: Hongrui Huang, Junke Wang, Quanhao Li, Yu-Gang Jiang, Zuxuan Wu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.07967v1.pdf)  
  Keywords: world model, motion control, benchmark, video generation, controllable, interactive, dit  
- **[Streaming Video Generation with Streaming Force Control](https://arxiv.org/abs/2606.07508v1)**  
  Authors: Hanhui Wang, Yiming Xie, Haiwen Feng, Zhaoyang Lv, Shenlong Wang, Huaizu Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.07508v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://neu-vi.github.io/StreamForce)  
  Keywords: streaming, autoregressive, distillation, physical, video generation, controllable  

### Human & Character Animation

- **[CULTURESCORE: Evaluating Cultural Faithfulness in Video Generation Models](https://arxiv.org/abs/2606.07311v1)**  
  Authors: Anku Rani, Wei Dai, Shravan Nayak, Pattie Maes, Mahdi M. Kalayeh, Paul Pu Liang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.07311v1.pdf)  
  Keywords: video generation, identity, gesture, evaluation  
- **[Resonant Minds: Closed-Loop Social Avatars with Theory of Mind](https://arxiv.org/abs/2606.05896v1)**  
  Authors: Jianxu Shangguan, Jing Xu, Hang Ye, Xiaoxuan Ma, Yizhou Wang, Wentao Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.05896v1.pdf)  
  Keywords: dynamics, evaluation, avatar, video generation, controllable, talking head  
- **[Mamba-Enhanced Implicit Motion Learning for Audio-Driven Portrait Animation](https://arxiv.org/abs/2606.03402v2)**  
  Authors: Xuan Wei, Jiahui Chen, Kaiheng Li, Mingyu Shao, Qingqi Hong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.03402v2.pdf)  
  Keywords: dynamics, architecture, audio-driven, diffusion model, gesture, human motion, benchmark, video generation, human animation  
- **[Towards 3D-Aware Video Diffusion Models: Render-Free Human Motion Control with Mesh Tokenization](https://arxiv.org/abs/2606.02000v1)**  
  Authors: Jingyun Liang, Min Wei, Shikai Li, Yizeng Han, Hangjie Yuan, Lei Sun, Weihua Chen, Fan Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.02000v1.pdf)  
  Keywords: architecture, 3d-aware, diffusion model, motion control, benchmark, human motion, trajectory, video generation, video diffusion, dit  
- **[Auteur: Language-Driven Cinematographic Framing for Human-Centric Video Generation](https://arxiv.org/abs/2606.01900v1)**  
  Authors: Muhammed Burak Kizil, Enes Sanli, Niloy J. Mitra, Xuelin Chen, Erkut Erdem, Aykut Erdem, Duygu Ceylan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.01900v1.pdf)  
  Keywords: video generation, film, camera control, human motion  
- **[Archon: A Unified Multimodal Model for Holistic Digital Human Generation](https://arxiv.org/abs/2605.30311v1)**  
  Authors: Chong Bao, Shichen Liu, Lijun Yu, David Futschik, Stylianos Moschoglou, Shefali Srivastava, Ziqian Bai, Feitong Tan, Guofeng Zhang, Zhaopeng Cui, Sean Fanello, Yinda Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30311v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://zju3dv.github.io/archon)  
  Keywords: dynamics, autoregressive, avatar, efficient, video diffusion  
- **[LongCat-Video-Avatar 1.5 Technical Report](https://arxiv.org/abs/2605.26486v1)**  
  Authors: Meituan LongCat Team, Xunliang Cai, Meng Cheng, Feng Gao, Zhe Kong, Jiamu Li, Le Li, Weiheng Li, Hongyu Liu, Shuai Tan, Xiaoming Wei, Tianyu Yang, Yong Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.26486v1.pdf)  
  Keywords: audio-driven, evaluation, identity, avatar, distillation, benchmark, video generation, dit  
- **[RoMo: A Large-Scale, Richly Organized Dataset and Semantic Taxonomy for Human Motion Generation](https://arxiv.org/abs/2605.26241v1)**  
  Authors: Jiahao Zhang, Joseph Liu, Young-Yoon Lee, Seonghyeon Moon, Victor Zordan, Guy Tevet, Karen Liu, Stephen Gould, Oren Jacob, Haomiao Jiang, Mubbasir Kapadia, Yizhak Ben-Shabat  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.26241v1.pdf)  
  Keywords: human motion, evaluation  
- **[iTryOn: Mastering Interactive Video Virtual Try-On with Spatial-Semantic Guidance](https://arxiv.org/abs/2605.21431v1)**  
  Authors: Jun Zheng, Zhengze Xu, Mengting Chen, Jing Wang, Jinsong Lan, Xiaoyong Zhu, Kaifu Zhang, Bo Zheng, Xiaodan Liang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.21431v1.pdf)  
  Keywords: dynamics, diffusion transformer, virtual try-on, benchmark, temporal consistency, controllable, interactive, video diffusion, dit  
- **[EverAnimate: Minute-Scale Human Animation via Latent Flow Restoration](https://arxiv.org/abs/2605.15042v1)**  
  Authors: Wuyang Li, Yang Gao, Mariam Hassan, Lan Feng, Wentao Pan, Po-Chien Luan, Alexandre Alahi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.15042v1.pdf)  
  Keywords: flow matching, identity, long-form, human motion, video generation, efficient, human animation  

### Image-to-Video Generation

- **[RigPAPR: Rig-Based Animation of Static Neural Point Clouds from a Fixed-Viewpoint Video](https://arxiv.org/abs/2606.06685v1)**  
  Authors: Shichong Peng, Yanshu Zhang, Ke Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.06685v1.pdf)  
  Keywords: novel view, i2v, image-to-video  
- **[Physics in 2-Steps: Locking Motion Priors Before Visual Refinement Erases Them](https://arxiv.org/abs/2606.06361v1)**  
  Authors: Woojung Han, Seil Kang, Youngjun Jun, Min-Hung Chen, Fu-En Yang, Seong Jae Hwang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.06361v1.pdf)  
  Keywords: denoising, physics, diffusion model, image-to-video, physical, trajectory, video diffusion  
- **[V2V-Bench: A Comprehensive Benchmark for Video-to-Video Generation Evaluation](https://arxiv.org/abs/2606.05665v1)**  
  Authors: Tao Liu, Leela Krishna, Gouti Pavan Kumar, Sreeja K, Vishav Garg  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.05665v1.pdf)  
  Keywords: i2v, evaluation, video-to-video, t2v, benchmark, video generation, dit  
- **[AAD-1: Asymmetric Adversarial Distillation for One-Step Autoregressive Video Generation](https://arxiv.org/abs/2606.03972v2)**  
  Authors: Haobo Li, Yanhong Zeng, Yunhong Lu, Jiapeng Zhu, Hao Ouyang, Qiuyu Wang, Ka Leong Cheng, Yujun Shen, Zhipeng Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.03972v2.pdf)  
  Keywords: architecture, autoregressive, distillation, image-to-video, video generation  
- **[Cosmos 3: Omnimodal World Models for Physical AI](https://arxiv.org/abs/2606.02800v2)**  
  Authors: NVIDIA, :, Aditi, Niket Agarwal, Arslan Ali, Jon Allen, Martin Antolini, Adeline Aubame, Alisson Azzolini, Junjie Bai, Maciej Bala, Yogesh Balaji, Josh Bapst, Aarti Basant, Mukesh Beladiya, Mohammad Qazim Bhat, Zaid Pervaiz Bhat, Dan Blick, Vanni Brighella, Han Cai, Tiffany Cai, Eric Cameracci, Jiaxin Cao, Yulong Cao, Mark Carlson, Carlos Casanova, Ting-Yun Chang, Yan Chang, Yu-Wei Chao, Prithvijit Chattopadhyay, Roshan Chaudhari, Chieh-Yun Chen, Junyu Chen, Ke Chen, Qizhi Chen, Wenkai Chen, Xiaotong Chen, Yu Chen, An-Chieh Cheng, Click Cheng, Xiu Chia, Jeana Choi, Chaeyeon Chung, Wenyan Cong, Yin Cui, Magdalena Dadela, Nalin Dadhich, Wenliang Dai, Joyjit Daw, Alperen Degirmenci, Rodrigo Vieira Del Monte, Robert Denomme, Sameer Dharur, Marco Di Lucca, Ke Ding, Wenhao Ding, Yifan Ding, Yuzhu Dong, Nicole Drumheller, Yilun Du, Aigul Dzhumamuratova, Aleksandr Efitorov, Hamid Eghbalzadeh, Naomi Eigbe, Imad El Hanafi, Hassan Eslami, Benedikt Falk, Jiaojiao Fan, Jim Fan, Amol Fasale, Sergiy Fefilatyev, Liang Feng, Francesco Ferroni, Sanja Fidler, Xiao Fu, Vikram Fugro, Prashant Gaikwad, TJ Galda, Katelyn Gao, Yihuai Gao, Wenhang Ge, Sreyan Ghosh, Arushi Goel, Vivek Goel, Akash Gokul, Rama Govindaraju, Jinwei Gu, Miguel Guerrero, Elfie Guo, Aryaman Gupta, Siddharth Gururani, Hugo Hadfield, Song Han, Ankur Handa, Zekun Hao, Mohammad Harrim, Ali Hassani, Nathan Hayes-Roth, Yufan He, Chris Helvig, Cyrus Hogg, Madison Huang, Michael Huang, Sophia Huang, Yufan Huang, Jacob Huffman, DeLesley Hutchins, Suneel Indupuru, Boris Ivanovic, Arihant Jain, Joel Jang, Ryan Ji, Yanan Jian, Dongfu Jiang, Jingyi Jin, Atharva Joshi, Nikhilesh Joshi, Pranjali Joshi, Andy Ju, Jaehun Jung, Weiwei Kang, Scott Kassekert, Jan Kautz, Ashna Khetan, Julia Kiczka, Slawek Kierat, Gwanghyun Kim, Kuno Kim, Sunny Kim, Kezhi Kong, Xin Kong, Zhifeng Kong, Tomasz Kornuta, Egor Krivov, Hui Kuang, Saurav Kumar, Chia-Wen Kuo, George Kurian, Wojciech Kutak, JF Lafleche, Himangshu Lahkar, Omar Laymoun, Jayjun Lee, Sanggil Lee, Gabriele Leone, Boyi Li, Freya Li, Jiajun Li, Jinfeng Li, Ling Li, Pengcheng Li, Shangru Li, Tingle Li, Xiaolong Li, Xuan Li, Zhaoshuo Li, Zhiqi Li, Hao Liang, Maosheng Liao, Chen-Hsuan Lin, Tsung-Yi Lin, Ming-Yu Liu, Sifei Liu, Zihan Liu, Hai Loc Lu, Xiangyu Lu, Alice Luo, Ruipu Luo, Wenjie Luo, Jiangran Lyu, Martin Ding Ma, Nic Ma, Qianli Ma, Dawid Majchrowski, Louis Marcoux, Miguel Martin, Qing Miao, Ashkan Mirzaei, Shreyas Misra, Kaichun Mo, Durra Mohsin, Hyejin Moon, Pawel Morkisz, Saeid Motiian, Kirill Motkov, Seungjun Nah, Yashraj Narang, Deepak Narayanan, Thabang Ngazimbi, Julian Ouyang, Shubham Pachori, David Page, Yatian Pang, Sehwi Park, Mahesh Patekar, Mostofa Patwary, Marco Pavone, Trung Pham, Wei Ping, Soha Pouya, Shrimai Prabhumoye, Varun Praveen, Delin Qu, Hesam Rabeti, Morteza Ramezanali, Marilyn Reeb, Xuanchi Ren, Kristen Rumley, Wojciech Rymer, Jun Saito, Yeongho Seol, John Shao, Piyush Shekdar, Tianwei Shen, Humphrey Shi, Min Shi, Stella Shi, Kevin Shih, Mohammad Shoeybi, Mateusz Sieniawski, Shuran Song, Alexander Sotelo, Amir Sotoodeh, Sunil Srinivasa, Vignesh Srinivasakumar, Bartosz Stefaniak, Rahul Heinrich Steiger, Shangkun Sun, Jiaxiang Tang, Shitao Tang, Yangyang Tang, Yue Tang, Tolou Tavakkoli, Kayley Ting, Krzysztof Tomala, Wei-Cheng Tseng, Jibin Varghese, Sergei Vasilev, Thomas Volk, Raju Wagwani, Roger Waleffe, Andrew Z. Wang, Boxiang Wang, Haoxiang Wang, Qiao Wang, Shihao Wang, Shijie Wang, Ting-Chun Wang, Yan Wang, Yu Wang, Rohit Watve, David Wehr, Fangyin Wei, Xinshuo Weng, Jay Zhangjie Wu, Kedi Wu, Hongchi Xia, Summer Xiao, Tianjun Xiao, Kevin Xie, Daguang Xu, Jiashu Xu, Mengyao Xu, Ruqing Xu, Xingqian Xu, Yao Xu, Dinghao Yang, Dong Yang, Hans Yang, Xiaodong Yang, Xuning Yang, Yichu Yang, Yurong You, Zhiding Yu, Hao Yuan, Simon Yuen, Xiaohui Zeng, Pengcuo Zeren, Cindy Zha, Haotian Zhang, Jenny Zhang, Jing Zhang, Liangkai Zhang, Paris Zhang, Shun Zhang, Xuanmeng Zhang, Zhizheng Zhang, Ann Zhao, Yilin Zhao, Yuliya Zhautouskaya, Charles Zhou, Fengzhe Zhou, Shilin Zhu, Yuke Zhu, Dima Zhylko, Artur Zolkowski  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.02800v2.pdf) | [![GitHub](https://img.shields.io/github/stars/nvidia/cosmos?style=social)](https://github.com/nvidia/cosmos) | [![Project](https://img.shields.io/badge/-Project-blue)](https://research.nvidia.com/labs/cosmos-lab/cosmos3) | [![HuggingFace](https://img.shields.io/badge/-HuggingFace-yellow)](https://huggingface.co/collections/nvidia/cosmos3)  
  Keywords: architecture, world simulator, evaluation, world model, image-to-video, benchmark, physical  
- **[From Zero to Hero: Training-Free Custom Concept Spawning in World Models](https://arxiv.org/abs/2606.02575v1)**  
  Authors: Kiymet Akdemir, Pinar Yanardag  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.02575v1.pdf)  
  Keywords: concept, world model, simulation, autoregressive, identity, image-to-video, video generation, controllable, interactive, dit  
- **[OptiWorld: Optimal Control for Video World Generation under Physical Constraints](https://arxiv.org/abs/2606.00499v1)**  
  Authors: Yu Yuan, Jianhao Yuan, Xijun Wang, Daiqing Li, Liu He, Lu Ling, Stanley H. Chan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.00499v1.pdf)  
  Keywords: dynamics, world model, image-to-video, physical, trajectory, video generation, efficient, dit  
- **[Robust Dreamer: Deviation-Aware Latent Gaussian Memory for Action-Controlled AR Video Generation](https://arxiv.org/abs/2605.30855v2)**  
  Authors: Hanlin Chen, Jiaxin Wei, Xibin Song, Yifu Wang, Steve Wang, Hongdong Li, Pan Ji, Gim Hee Lee  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30855v2.pdf)  
  Keywords: denoising, simulation, autoregressive, 3d-aware, image-to-video, video generation, interactive, dit  
- **[minWM: A Full-Stack Open-Source Framework for Real-Time Interactive Video World Models](https://arxiv.org/abs/2605.30263v1)**  
  Authors: Min Zhao, Hongzhou Zhu, Bokai Yan, Zihan Zhou, Yimin Chen, Wenqiang Sun, Kaiwen Zheng, Guande He, Xiao Yang, Chongxuan Li, Fan Bao, Jun Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30263v1.pdf) | [![GitHub](https://img.shields.io/github/stars/shengshu-ai/minWM?style=social)](https://github.com/shengshu-ai/minWM)  
  Keywords: i2v, architecture, camera control, world model, streaming, autoregressive, diffusion model, t2v, distillation, style, trajectory, video generation, controllable, interactive, video diffusion, dit  
- **[LiveSVG: Zero-Shot SVG Animation via Video Generation](https://arxiv.org/abs/2605.30174v1)**  
  Authors: Matan Levy, Ran Margolin, Bar Cavia, Dvir Samuel, Yael Pritch, Shmuel Peleg, Alex Rav Acha, Ariel Shamir, Dani Lischinski  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30174v1.pdf)  
  Keywords: evaluation, diffusion model, distillation, image-to-video, benchmark, video generation, video diffusion, dit  

### Long Video Generation

*Showing the latest 50 out of 135 papers*

- **[TetherCache: Stabilizing Autoregressive Long-Form Video Generation with Gated Recall and Trusted Alignment](https://arxiv.org/abs/2606.13035v1)**  
  Authors: Yu Meng, Xiangyang Luo, Letian Li, Wenyuan Jiang, Chen Gao, Xinlei Chen, Yong Li, Xiao-Ping Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13035v1.pdf)  
  Keywords: streaming, long video, diffusion model, autoregressive, long-form, video generation, video diffusion, dit  
- **[MSUE: Multi-Modal Soccer Understanding Expert](https://arxiv.org/abs/2606.12106v1)**  
  Authors: Litao Li, Yibo Yu, Yufeng Hu, Zhuo Yang, Jiali Wen, Yixin Chen, Yixi Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.12106v1.pdf)  
  Keywords: long-form, multi-modal, architecture, benchmark  
- **[Next Forcing: Causal World Modeling with Multi-Chunk Prediction](https://arxiv.org/abs/2606.11187v1)**  
  Authors: Gangwei Xu, Qihang Zhang, Jiaming Zhou, Xing Zhu, Yujun Shen, Xin Yang, Yinghao Xu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.11187v1.pdf)  
  Keywords: dynamics, world model, acceleration, denoising, autoregressive, benchmark, physical, video generation  
- **[Lip Forcing: Few-Step Autoregressive Diffusion for Real-time Lip Synchronization](https://arxiv.org/abs/2606.11180v1)**  
  Authors: Paul Hyunbin Cho, Jinhyuk Jang, SeokYoung Lee, Joungbin Lee, Siyoon Jin, Heeseong Shin, Jung Yi, Yunjin Park, Chulmin Park, Seungryong Kim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.11180v1.pdf)  
  Keywords: streaming, video-to-video, denoising, autoregressive, diffusion model, trajectory, video diffusion, dit  
- **[FadeMem: Distance-Aware Memory Consolidation for Autoregressive Video Diffusion](https://arxiv.org/abs/2606.10671v1)**  
  Authors: Yu Lu, Junjie Yang, Piotr Koniusz, YuXin Song, Yi Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.10671v1.pdf)  
  Keywords: dynamics, long video, identity, autoregressive, video diffusion  
- **[BiWM: Advancing Open-Source Interactive Video World Models with Bidirectional Autoregression](https://arxiv.org/abs/2606.10135v2)**  
  Authors: Shaohao Rui, Xiaofeng Mao, Zhanyu Zhang, Peijia Lin, Yansong Zhu, Yibo Zhang, Haibin Wan, Weijie Ma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.10135v2.pdf)  
  Keywords: dynamics, camera control, world model, simulation, autoregressive, diffusion model, distillation, style, controllable, interactive, video diffusion  
- **[CineDance: Towards Next-Generation Multi-Shot Long-Form Cinematic Audio-Video Generation](https://arxiv.org/abs/2606.09639v2)**  
  Authors: Yuheng Chen, Teng Hu, Yuji Wang, Qingdong He, Zhucun Xue, Qianyu Zhou, Jason Li, Lizhuang Ma, Jiangning Zhang, Dacheng Tao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.09639v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://aliothchen.github.io/projects/CineDance)  
  Keywords: long-form, video generation, film, evaluation  
- **[OmniGen-AR: AutoRegressive Any-to-Image Generation](https://arxiv.org/abs/2606.09156v1)**  
  Authors: Junke Wang, Xun Wang, Qiushan Guo, Peize Sun, Weilin Huang, Zuxuan Wu, Yu-Gang Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.09156v1.pdf)  
  Keywords: architecture, autoregressive, text-to-video, benchmark, video generation, dit  
- **[Ultra Flash: Scaling Real-Time Streaming Video Generation to High Resolutions](https://arxiv.org/abs/2606.09150v1)**  
  Authors: Luxury, Jie Huang, Zihao Fan, Xiaoxiao Ma, Yuming Li, Jun-hao Zhuang, Zeyue Xue, Siming Fu, Haoran Li, Mingchen Zhong, Guohui Zhang, Shichen Ma, Yijun Liu, Jiaqi Shi, Yanwen Ma, Yaofeng Su, Haoyu Wang, Yaowei Li, Songchun Zhang, Weiyang Jin, Yuxuan Bian, Shiyi Zhang, Haojun Xu, Shuai Lu, Xin Han, Wei Tang, Haoyang Huang, Nan Duan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.09150v1.pdf)  
  Keywords: architecture, streaming, autoregressive, diffusion model, t2v, distillation, super-resolution, video generation, efficient, video diffusion  
- **[BioVid: Autoregressive Video Generation with Biological Behavior Semantic Comprehension](https://arxiv.org/abs/2606.08674v2)**  
  Authors: Tsung-Wei Pan, Jung-Hua Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.08674v2.pdf)  
  Keywords: video generation, autoregressive  

### Personalization & Customization

*Showing the latest 50 out of 85 papers*

- **[A Comprehensive Ecosystem for Open-Domain Customized Video Generation](https://arxiv.org/abs/2606.11783v1)**  
  Authors: Jingxu Zhang, Yuqian Hong, Daneul Kim, Kai Qiu, Qi Dai, Jianmin Bao, Yifan Yang, Xiaoyan Sun, Chong Luo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.11783v1.pdf)  
  Keywords: diffusion transformer, identity, benchmark, video generation, efficient, dit  
- **[ARGUS: Stacked Multi-View Identity Mosaic Injection for Subject-Preserving Video Generation](https://arxiv.org/abs/2606.11670v1)**  
  Authors: Zijie Meng, Jiwen Liu, Yufei Liu, Chengzhuo Tong, Xiaoqiang Liu, Yuanxing Zhang, Yulong Xu, Pengfei Wan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.11670v1.pdf)  
  Keywords: video generation, identity, benchmark, dit  
- **[Flow-DPPO: Divergence Proximal Policy Optimization for Flow Matching Models](https://arxiv.org/abs/2606.11025v1)**  
  Authors: Bowen Ping, Xiangxin Zhou, Penghui Qi, Minnan Luo, Liefeng Bo, Tianyu Pang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.11025v1.pdf) | [![GitHub](https://img.shields.io/github/stars/Tencent-Hunyuan/UniRL?style=social)](https://github.com/Tencent-Hunyuan/UniRL)  
  Keywords: denoising, flow matching, style, trajectory, video generation  
- **[HarmoView: Harmonizing Multi-View Constraints for Identity-Consistent Video Generation](https://arxiv.org/abs/2606.10839v1)**  
  Authors: Cong Wang, Zhentao Yu, Hongmei Wang, Weicong Liang, Zixiang Zhou, Zilin Yang, Jiarong Ou, Rui Chen, Yuan Zhou, Qinglin Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.10839v1.pdf)  
  Keywords: evaluation, identity, layout, t2v, benchmark, video generation, dit  
- **[FadeMem: Distance-Aware Memory Consolidation for Autoregressive Video Diffusion](https://arxiv.org/abs/2606.10671v1)**  
  Authors: Yu Lu, Junjie Yang, Piotr Koniusz, YuXin Song, Yi Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.10671v1.pdf)  
  Keywords: dynamics, long video, identity, autoregressive, video diffusion  
- **[BiWM: Advancing Open-Source Interactive Video World Models with Bidirectional Autoregression](https://arxiv.org/abs/2606.10135v2)**  
  Authors: Shaohao Rui, Xiaofeng Mao, Zhanyu Zhang, Peijia Lin, Yansong Zhu, Yibo Zhang, Haibin Wan, Weijie Ma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.10135v2.pdf)  
  Keywords: dynamics, camera control, world model, simulation, autoregressive, diffusion model, distillation, style, controllable, interactive, video diffusion  
- **[LiteVSR: Lightweight Adaptation of Frozen Diffusion Transformers for Video Super-Resolution](https://arxiv.org/abs/2606.09250v1)**  
  Authors: Yu Cao, Ziquan Liu, Zhensong Zhang, Jiankang Deng, Shaogang Gong, Jifei Song  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.09250v1.pdf)  
  Keywords: architecture, diffusion transformer, denoising, flow matching, style, super-resolution  
- **[CoVEBench: Can Video Editing Models Handle Complex Instructions?](https://arxiv.org/abs/2606.08415v2)**  
  Authors: Jiangtao Wu, Jiaming Wang, Yiwen He, Yuanxing Zhang, Shihao Li, Dunyuan Liu, Xuedong Zhao, Jialu Chen, Zekun Moore Wang, Jiaheng Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.08415v2.pdf)  
  Keywords: style, video editing, benchmark, dit  
- **[CULTURESCORE: Evaluating Cultural Faithfulness in Video Generation Models](https://arxiv.org/abs/2606.07311v1)**  
  Authors: Anku Rani, Wei Dai, Shravan Nayak, Pattie Maes, Mahdi M. Kalayeh, Paul Pu Liang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.07311v1.pdf)  
  Keywords: video generation, identity, gesture, evaluation  
- **[Activation Steering of Video Generation Models via Reduced-Order Linear Optimal Control](https://arxiv.org/abs/2606.04775v1)**  
  Authors: Jihoon Hong, Alice Chan, Qiyue Dai, Julian Skifstad, Glen Chou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.04775v1.pdf)  
  Keywords: concept, dynamics, t2v, text-to-video, benchmark, video generation  

### Physical Understanding

*Showing the latest 50 out of 141 papers*

- **[RepWAM: World Action Modeling with Representation Visual-Action Tokenizers](https://arxiv.org/abs/2606.13674v1)**  
  Authors: Junke Wang, Qihang Zhang, Shuai Yang, Yiming Luo, Yujun Shen, Zuxuan Wu, Yu-Gang Jiang, Yinghao Xu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13674v1.pdf) | [![GitHub](https://img.shields.io/github/stars/wdrink/RepWAM?style=social)](https://github.com/wdrink/RepWAM)  
  Keywords: simulation, video generation, dynamics, benchmark  
- **[SpecLoR: Spectral Lookahead Rectification for Motion-Coherent Text-to-Video Generation](https://arxiv.org/abs/2606.11969v1)**  
  Authors: Xu Zhang, Yu Lu, Ruijie Quan, Zhaozheng Chen, Bohan Wang, Yi Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.11969v1.pdf)  
  Keywords: flow matching, text-to-video, benchmark, physical, video generation, dit  
- **[Next Forcing: Causal World Modeling with Multi-Chunk Prediction](https://arxiv.org/abs/2606.11187v1)**  
  Authors: Gangwei Xu, Qihang Zhang, Jiaming Zhou, Xing Zhu, Yujun Shen, Xin Yang, Yinghao Xu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.11187v1.pdf)  
  Keywords: dynamics, world model, acceleration, denoising, autoregressive, benchmark, physical, video generation  
- **[FadeMem: Distance-Aware Memory Consolidation for Autoregressive Video Diffusion](https://arxiv.org/abs/2606.10671v1)**  
  Authors: Yu Lu, Junjie Yang, Piotr Koniusz, YuXin Song, Yi Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.10671v1.pdf)  
  Keywords: dynamics, long video, identity, autoregressive, video diffusion  
- **[Making Time Editable in Video Diffusion Transformers](https://arxiv.org/abs/2606.10183v1)**  
  Authors: Konstantin Kuklev, Viacheslav Vasilev, Alexander Kunitsyn, Andrei Ivaniuta, Denis Dimitrov  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.10183v1.pdf)  
  Keywords: dynamics, diffusion transformer, video generation, controllable, video diffusion, dit  
- **[BiWM: Advancing Open-Source Interactive Video World Models with Bidirectional Autoregression](https://arxiv.org/abs/2606.10135v2)**  
  Authors: Shaohao Rui, Xiaofeng Mao, Zhanyu Zhang, Peijia Lin, Yansong Zhu, Yibo Zhang, Haibin Wan, Weijie Ma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.10135v2.pdf)  
  Keywords: dynamics, camera control, world model, simulation, autoregressive, diffusion model, distillation, style, controllable, interactive, video diffusion  
- **[Do Video Foundation Models Understand Intuitive Physics? A Layerwise Probing Analysis](https://arxiv.org/abs/2606.09646v1)**  
  Authors: Samuele Punzo, Niccolò Caselli, Ippokratis Pantelidis, Francesco Massafra, Salvatore Lo Sardo, Mohammadreza Salehi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.09646v1.pdf)  
  Keywords: dynamics, benchmark, physics  
- **[Conan-embedding-v3: Fusing Modality-Specific Models for Omni-Modal Embedding](https://arxiv.org/abs/2606.09331v1)**  
  Authors: Shiyu Li, Zhiyuan Hu, Yifan Wang, Peiming Li, Zheng Wei, Yang Tang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.09331v1.pdf)  
  Keywords: dynamics, multi-modal, architecture  
- **[EgoTactile: Learning Grasp Pressure for Everyday Objects from Egocentric Video](https://arxiv.org/abs/2606.09243v1)**  
  Authors: Yuan Zeng, Yujia Shi, Tiao Tan, Xingting Li, Yaqi Qin, Zongqing Lu, Wenming Yang, Jing-Hao Xue, Qingmin Liao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.09243v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://egotactile.github.io)  
  Keywords: physical, benchmark, video diffusion, dit  
- **[CP4D: Compositional Physics-aware 4D Scene Generation](https://arxiv.org/abs/2606.09187v1)**  
  Authors: Hanxin Zhu, Cong Wang, Tianyu He, Long Chen, Xin Jin, Chen Gao, Zhibo Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.09187v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://anonymous.4open.science/w/CP4D)  
  Keywords: dynamics, physics, diffusion model, 4d generation, physical, physics-aware, interactive, video diffusion  

### Surveys & Benchmarks

*Showing the latest 50 out of 236 papers*

- **[RepWAM: World Action Modeling with Representation Visual-Action Tokenizers](https://arxiv.org/abs/2606.13674v1)**  
  Authors: Junke Wang, Qihang Zhang, Shuai Yang, Yiming Luo, Yujun Shen, Zuxuan Wu, Yu-Gang Jiang, Yinghao Xu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13674v1.pdf) | [![GitHub](https://img.shields.io/github/stars/wdrink/RepWAM?style=social)](https://github.com/wdrink/RepWAM)  
  Keywords: simulation, video generation, dynamics, benchmark  
- **[World Tracing: Generative Pixel-Aligned Geometry Beyond the Visible](https://arxiv.org/abs/2606.13652v1)**  
  Authors: Hao Zhang, Mohamed El Banani, Jen-Hao Cheng, Paul Zhang, Yi Hua, Ben Mildenhall, Christoph Lassner, Narendra Ahuja, Gengshan Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13652v1.pdf)  
  Keywords: diffusion transformer, video synthesis, denoising, flow matching, benchmark, dit  
- **[ReFree: Towards Realistic Co-Speech Video Generation via Reward-Free RL and Multilevel Speech Guidance](https://arxiv.org/abs/2606.13304v1)**  
  Authors: Salaheldin Mohamed, M. Hamza Mughal, Rishabh Dabral, Christian Theobalt  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13304v1.pdf)  
  Keywords: video generation, speech-driven, evaluation  
- **[MSUE: Multi-Modal Soccer Understanding Expert](https://arxiv.org/abs/2606.12106v1)**  
  Authors: Litao Li, Yibo Yu, Yufeng Hu, Zhuo Yang, Jiali Wen, Yixin Chen, Yixi Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.12106v1.pdf)  
  Keywords: long-form, multi-modal, architecture, benchmark  
- **[World Model Self-Distillation: Training World Models to Solve General Tasks](https://arxiv.org/abs/2606.12072v1)**  
  Authors: Sebastian Stapf, Pablo Acuaviva Huertos, Aram Davtyan, Paolo Favaro  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.12072v1.pdf)  
  Keywords: world model, evaluation, diffusion model, distillation, robotics, benchmark, video diffusion, dit  
- **[SpecLoR: Spectral Lookahead Rectification for Motion-Coherent Text-to-Video Generation](https://arxiv.org/abs/2606.11969v1)**  
  Authors: Xu Zhang, Yu Lu, Ruijie Quan, Zhaozheng Chen, Bohan Wang, Yi Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.11969v1.pdf)  
  Keywords: flow matching, text-to-video, benchmark, physical, video generation, dit  
- **[A Comprehensive Ecosystem for Open-Domain Customized Video Generation](https://arxiv.org/abs/2606.11783v1)**  
  Authors: Jingxu Zhang, Yuqian Hong, Daneul Kim, Kai Qiu, Qi Dai, Jianmin Bao, Yifan Yang, Xiaoyan Sun, Chong Luo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.11783v1.pdf)  
  Keywords: diffusion transformer, identity, benchmark, video generation, efficient, dit  
- **[ARGUS: Stacked Multi-View Identity Mosaic Injection for Subject-Preserving Video Generation](https://arxiv.org/abs/2606.11670v1)**  
  Authors: Zijie Meng, Jiwen Liu, Yufei Liu, Chengzhuo Tong, Xiaoqiang Liu, Yuanxing Zhang, Yulong Xu, Pengfei Wan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.11670v1.pdf)  
  Keywords: video generation, identity, benchmark, dit  
- **[AVIS: Adaptive Test-Time Scaling for Vision-Language Models](https://arxiv.org/abs/2606.11576v1)**  
  Authors: Ahmadreza Jeddi, Minh Ngoc Le, Amirhossein Kazerouni, Hakki Can Karaimer, Hue Nguyen, Iqbal Mohomed, Michael Brudno, Alex Levinshtein, Konstantinos G. Derpanis, Babak Taati, Radek Grzeszczuk  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.11576v1.pdf)  
  Keywords: benchmark  
- **[Next Forcing: Causal World Modeling with Multi-Chunk Prediction](https://arxiv.org/abs/2606.11187v1)**  
  Authors: Gangwei Xu, Qihang Zhang, Jiaming Zhou, Xing Zhu, Yujun Shen, Xin Yang, Yinghao Xu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.11187v1.pdf)  
  Keywords: dynamics, world model, acceleration, denoising, autoregressive, benchmark, physical, video generation  

### Text-to-Video Generation

*Showing the latest 50 out of 54 papers*

- **[Flex4DHuman: Flexible Multi-view Video Diffusion for 4D Human Reconstruction](https://arxiv.org/abs/2606.13655v1)**  
  Authors: Jen-Hao Cheng, Yipeng Wang, Hao Zhang, Gengshan Yang, Jenq-Neng Hwang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13655v1.pdf)  
  Keywords: architecture, simulation, diffusion model, text-to-video, multi-view video, video diffusion, dit  
- **[SpecLoR: Spectral Lookahead Rectification for Motion-Coherent Text-to-Video Generation](https://arxiv.org/abs/2606.11969v1)**  
  Authors: Xu Zhang, Yu Lu, Ruijie Quan, Zhaozheng Chen, Bohan Wang, Yi Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.11969v1.pdf)  
  Keywords: flow matching, text-to-video, benchmark, physical, video generation, dit  
- **[Plan-and-Verify Video Reward Reasoning with Spatio-Temporal Scene Graph Grounding](https://arxiv.org/abs/2606.11838v1)**  
  Authors: Hyomin Kim, Junghye Kim, Joanie Hayoun Chung, Yoonjin Oh, Kyungjae Lee, Sungbin Lim, Sungwoong Kim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.11838v1.pdf)  
  Keywords: text-to-video, dit, t2v  
- **[HarmoView: Harmonizing Multi-View Constraints for Identity-Consistent Video Generation](https://arxiv.org/abs/2606.10839v1)**  
  Authors: Cong Wang, Zhentao Yu, Hongmei Wang, Weicong Liang, Zixiang Zhou, Zilin Yang, Jiarong Ou, Rui Chen, Yuan Zhou, Qinglin Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.10839v1.pdf)  
  Keywords: evaluation, identity, layout, t2v, benchmark, video generation, dit  
- **[OmniGen-AR: AutoRegressive Any-to-Image Generation](https://arxiv.org/abs/2606.09156v1)**  
  Authors: Junke Wang, Xun Wang, Qiushan Guo, Peize Sun, Weilin Huang, Zuxuan Wu, Yu-Gang Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.09156v1.pdf)  
  Keywords: architecture, autoregressive, text-to-video, benchmark, video generation, dit  
- **[Ultra Flash: Scaling Real-Time Streaming Video Generation to High Resolutions](https://arxiv.org/abs/2606.09150v1)**  
  Authors: Luxury, Jie Huang, Zihao Fan, Xiaoxiao Ma, Yuming Li, Jun-hao Zhuang, Zeyue Xue, Siming Fu, Haoran Li, Mingchen Zhong, Guohui Zhang, Shichen Ma, Yijun Liu, Jiaqi Shi, Yanwen Ma, Yaofeng Su, Haoyu Wang, Yaowei Li, Songchun Zhang, Weiyang Jin, Yuxuan Bian, Shiyi Zhang, Haojun Xu, Shuai Lu, Xin Han, Wei Tang, Haoyang Huang, Nan Duan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.09150v1.pdf)  
  Keywords: architecture, streaming, autoregressive, diffusion model, t2v, distillation, super-resolution, video generation, efficient, video diffusion  
- **[V2V-Bench: A Comprehensive Benchmark for Video-to-Video Generation Evaluation](https://arxiv.org/abs/2606.05665v1)**  
  Authors: Tao Liu, Leela Krishna, Gouti Pavan Kumar, Sreeja K, Vishav Garg  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.05665v1.pdf)  
  Keywords: i2v, evaluation, video-to-video, t2v, benchmark, video generation, dit  
- **[Do Models Share Safety Representations? Cross-Model Steering for Safe Visual Generation](https://arxiv.org/abs/2606.05290v1)**  
  Authors: Tobia Poppi, Silvia Cappelletti, Sara Sarto, Florian Schiffers, Garin Kessler, Marcella Cornia, Lorenzo Baraldi, Rita Cucchiara  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.05290v1.pdf)  
  Keywords: text-to-video, video generation, architecture  
- **[Activation Steering of Video Generation Models via Reduced-Order Linear Optimal Control](https://arxiv.org/abs/2606.04775v1)**  
  Authors: Jihoon Hong, Alice Chan, Qiyue Dai, Julian Skifstad, Glen Chou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.04775v1.pdf)  
  Keywords: concept, dynamics, t2v, text-to-video, benchmark, video generation  
- **[Spatial-Temporal Decoupled Reference Conditioning for Identity-Preserving Text-to-Video Generation](https://arxiv.org/abs/2606.02441v1)**  
  Authors: Yuheng Chen, Teng Hu, Yuji Wang, Qingdong He, Lizhuang Ma, Jiangning Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.02441v1.pdf)  
  Keywords: identity, layout, text-to-video, temporal consistency, video generation, dit  

### Video Editing

- **[Lip Forcing: Few-Step Autoregressive Diffusion for Real-time Lip Synchronization](https://arxiv.org/abs/2606.11180v1)**  
  Authors: Paul Hyunbin Cho, Jinhyuk Jang, SeokYoung Lee, Joungbin Lee, Siyoon Jin, Heeseong Shin, Jung Yi, Yunjin Park, Chulmin Park, Seungryong Kim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.11180v1.pdf)  
  Keywords: streaming, video-to-video, denoising, autoregressive, diffusion model, trajectory, video diffusion, dit  
- **[CoVEBench: Can Video Editing Models Handle Complex Instructions?](https://arxiv.org/abs/2606.08415v2)**  
  Authors: Jiangtao Wu, Jiaming Wang, Yiwen He, Yuanxing Zhang, Shihao Li, Dunyuan Liu, Xuedong Zhao, Jialu Chen, Zekun Moore Wang, Jiaheng Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.08415v2.pdf)  
  Keywords: style, video editing, benchmark, dit  
- **[TIDE: Task-Isolated Diffusion for Unified Video Editing and Generation](https://arxiv.org/abs/2606.08260v1)**  
  Authors: Qi Liu, Gang Yue, Mingyu Yin, Lisai Zhang, Yidi Wu, Yaole Wang, Yaohui Wang, Chang Yao, Jingyuan Chen, Lin Ma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.08260v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://LittleWork123.github.io/tide)  
  Keywords: diffusion transformer, video editing, benchmark, video generation, dit  
- **[LoomVideo: Unifying Multimodal Inputs into Video Generation and Editing](https://arxiv.org/abs/2606.06042v2)**  
  Authors: Jianzong Wu, Hao Lian, Jiongfan Yang, Dachao Hao, Ye Tian, Yunhai Tong, Jingyuan Zhu, Biaolong Chen, Qiaosong Qi, Aixi Zhang, Wanggui He, Mushui Liu, Jinlong Liu, Pipei Huang, Hao Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.06042v2.pdf)  
  Keywords: architecture, diffusion transformer, acceleration, video editing, benchmark, video generation, efficient, dit  
- **[V2V-Bench: A Comprehensive Benchmark for Video-to-Video Generation Evaluation](https://arxiv.org/abs/2606.05665v1)**  
  Authors: Tao Liu, Leela Krishna, Gouti Pavan Kumar, Sreeja K, Vishav Garg  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.05665v1.pdf)  
  Keywords: i2v, evaluation, video-to-video, t2v, benchmark, video generation, dit  
- **[Bootstrap Your Generator: Unpaired Visual Editing with Flow Matching](https://arxiv.org/abs/2606.03911v1)**  
  Authors: Yoad Tewel, Yuval Atzmon, Gal Chechik, Lior Wolf  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.03911v1.pdf)  
  Keywords: flow matching, video editing, evaluation, dit  
- **[AlbedoEdit: Unified Instance-Level Video Editing with Albedo Guidance](https://arxiv.org/abs/2606.01362v1)**  
  Authors: Xilong Zhou, Bao-Huy Nguyen, Zheng Zeng, Jacob Munkberg, Jon Hasselgren, Thomas Leimkühler, Nima Kalantari, Miloš Hašan, Christian Theobalt  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.01362v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://vcai.mpi-inf.mpg.de/projects/AlbedoEdit)  
  Keywords: video editing, creative, dit  
- **[DeltaCam: Differential Intrinsic Camera Modeling for Video Generation](https://arxiv.org/abs/2605.25266v1)**  
  Authors: Debabrata Mandal, Zhihan Peng, Yujie Wang, Praneeth Chakravarthula  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25266v1.pdf)  
  Keywords: dynamics, video-to-video, video style transfer, style, video generation, controllable, video diffusion, dit  
- **[Geo-Align: Video Generation Alignment via Metric Geometry Reward](https://arxiv.org/abs/2605.23903v1)**  
  Authors: Zizun Li, Haoyu Guo, Runzhe Teng, Chunhua Shen, Tong He  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.23903v1.pdf)  
  Keywords: camera control, video-to-video, physical, video generation, dit  
- **[SimInsert: Seamless Video Object Insertion via Regional Sparse Attention Fusion](https://arxiv.org/abs/2605.23245v1)**  
  Authors: Xinyu Chen, Yuyi Qian, Jiang Lin, Shenyi Wang, Gao Wang, Zhiqiu Zhang, Jizhi Zhang, Mingjie Wang, Qiang Tang, Qian Wang, Song Wu, Zili Yi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.23245v1.pdf)  
  Keywords: denoising, video editing, diffusion model, image-to-video, trajectory, efficient, interactive, video diffusion, dit  

### Video Inpainting & Completion

- **[PointAction: 3D Points as Universal Action Representations for Robot Control](https://arxiv.org/abs/2606.03943v1)**  
  Authors: Mutian Tong, Han Jiang, Qiao Feng, Lingjie Liu, Jiatao Gu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.03943v1.pdf)  
  Keywords: dynamics, simulation, diffusion model, 4d generation, video generation, video prediction, video diffusion  
- **[World Models: A Comprehensive Survey of Architectures, Methodologies, Reasoning Paradigms, and Applications](https://arxiv.org/abs/2606.00133v1)**  
  Authors: Arif Hassan Zidan, Yi Pan, Hanqi Jiang, Ruiyu Yan, Wei Ruan, Zihao Wu, Lifeng Chen, Weihang You, Xinliang Li, Bowen Chen, Huawen Hu, Peilong Wang, Sizhuang Liu, Jing Zhang, Siyuan Li, Zhengliang Liu, Yu Bao, Lin Zhao, Lichao Sun, Dajiang Zhu, Xiang Li, Jinglei Lv, Quanzheng Li, Wei Liu, Tianming Liu, Wei Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.00133v1.pdf)  
  Keywords: interactive, education, dynamics, architecture, medical, world model, survey, evaluation, physics, robotics, benchmark, video generation, video prediction, autonomous driving  
- **[Full-4D: Generating Full-Scope 4D Scenes from a Single-View Video](https://arxiv.org/abs/2605.25500v1)**  
  Authors: Tingxi Chen, Ke Hao, Yabo Chen, Zhengxue Cheng, Rong Xie, Li Song, Haibin Huang, Chi Zhang, Xuelong Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25500v1.pdf)  
  Keywords: video synthesis, flow matching, diffusion model, distillation, video interpolation, 4d generation, physical, interactive, multi-view video, video diffusion, dit  
- **[CRONOS: Benchmarking Counterfactual Physical Consistency in Video Models](https://arxiv.org/abs/2605.23699v1)**  
  Authors: León Begiristain, Olaf Dünkel, Adam Kortylewski  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.23699v1.pdf)  
  Keywords: dynamics, world model, evaluation, benchmark, physical, video prediction, dit  
- **[GEM-4D: Geometry-Enhanced Video World Models for Robot Manipulation](https://arxiv.org/abs/2605.22882v3)**  
  Authors: Kaichen Zhou, Yuzhen Chen, Fangneng Zhan, Hang Hua, Grace Chen, Xinhai Chang, Ao Qu, Yilun Du, Zhuang Liu, Paul Pu Liang, Mengyu Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.22882v3.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://gem-4d.github.io)  
  Keywords: dynamics, architecture, world model, simulation, physical, video prediction, dit  
- **[Goodbye Drift: Anchored Tree Sampling for Long-Horizon Video-to-Video Generation](https://arxiv.org/abs/2605.20476v1)**  
  Authors: Matthew Bendel, Stephen W. Bailey, Mithilesh Vaidya, Sumukh Badam, Xingzhe He  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20476v1.pdf)  
  Keywords: video-to-video, autoregressive, t2v, distillation, style, outpainting, video generation, dit  
- **[Nano World Models: A Minimalist Implementation of Future Video Prediction](https://arxiv.org/abs/2605.23993v2)**  
  Authors: Siqiao Huang, Partha Kaushik, Michael Chen, Hengkai Pan, Kaiwen Geng, Omar Chehab, Fernando Moreno-Pino, Max Simchowitz  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.23993v2.pdf)  
  Keywords: interactive, architecture, world model, evaluation, simulation, autoregressive, video generation, video prediction, dit  
- **[Relit-LiVE: Relight Video by Jointly Learning Environment Video](https://arxiv.org/abs/2605.06658v1)**  
  Authors: Weiqing Xiao, Hong Li, Xiuyu Yang, Houyuan Chen, Wenyi Li, Tianqi Liu, Shaocong Xu, Chongjie Ye, Hao Zhao, Beibei Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.06658v1.pdf) | [![GitHub](https://img.shields.io/github/stars/zhuxing0/Relit-LiVE?style=social)](https://github.com/zhuxing0/Relit-LiVE)  
  Keywords: streaming, diffusion model, benchmark, physical, video prediction, video diffusion, dit  
- **[Quaternion Nonlinear Transform-Induced Nuclear Norm for Low-Rank Tensor Completion](https://arxiv.org/abs/2605.01467v1)**  
  Authors: Biswarup Karmakar, Ratikanta Behera  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.01467v1.pdf)  
  Keywords: video inpainting, efficient, benchmark  

### Video Super-Resolution & Enhancement

*Showing the latest 50 out of 74 papers*

- **[World Tracing: Generative Pixel-Aligned Geometry Beyond the Visible](https://arxiv.org/abs/2606.13652v1)**  
  Authors: Hao Zhang, Mohamed El Banani, Jen-Hao Cheng, Paul Zhang, Yi Hua, Ben Mildenhall, Christoph Lassner, Narendra Ahuja, Gengshan Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13652v1.pdf)  
  Keywords: diffusion transformer, video synthesis, denoising, flow matching, benchmark, dit  
- **[Next Forcing: Causal World Modeling with Multi-Chunk Prediction](https://arxiv.org/abs/2606.11187v1)**  
  Authors: Gangwei Xu, Qihang Zhang, Jiaming Zhou, Xing Zhu, Yujun Shen, Xin Yang, Yinghao Xu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.11187v1.pdf)  
  Keywords: dynamics, world model, acceleration, denoising, autoregressive, benchmark, physical, video generation  
- **[Lip Forcing: Few-Step Autoregressive Diffusion for Real-time Lip Synchronization](https://arxiv.org/abs/2606.11180v1)**  
  Authors: Paul Hyunbin Cho, Jinhyuk Jang, SeokYoung Lee, Joungbin Lee, Siyoon Jin, Heeseong Shin, Jung Yi, Yunjin Park, Chulmin Park, Seungryong Kim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.11180v1.pdf)  
  Keywords: streaming, video-to-video, denoising, autoregressive, diffusion model, trajectory, video diffusion, dit  
- **[Flow-DPPO: Divergence Proximal Policy Optimization for Flow Matching Models](https://arxiv.org/abs/2606.11025v1)**  
  Authors: Bowen Ping, Xiangxin Zhou, Penghui Qi, Minnan Luo, Liefeng Bo, Tianyu Pang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.11025v1.pdf) | [![GitHub](https://img.shields.io/github/stars/Tencent-Hunyuan/UniRL?style=social)](https://github.com/Tencent-Hunyuan/UniRL)  
  Keywords: denoising, flow matching, style, trajectory, video generation  
- **[LiteVSR: Lightweight Adaptation of Frozen Diffusion Transformers for Video Super-Resolution](https://arxiv.org/abs/2606.09250v1)**  
  Authors: Yu Cao, Ziquan Liu, Zhensong Zhang, Jiankang Deng, Shaogang Gong, Jifei Song  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.09250v1.pdf)  
  Keywords: architecture, diffusion transformer, denoising, flow matching, style, super-resolution  
- **[Ultra Flash: Scaling Real-Time Streaming Video Generation to High Resolutions](https://arxiv.org/abs/2606.09150v1)**  
  Authors: Luxury, Jie Huang, Zihao Fan, Xiaoxiao Ma, Yuming Li, Jun-hao Zhuang, Zeyue Xue, Siming Fu, Haoran Li, Mingchen Zhong, Guohui Zhang, Shichen Ma, Yijun Liu, Jiaqi Shi, Yanwen Ma, Yaofeng Su, Haoyu Wang, Yaowei Li, Songchun Zhang, Weiyang Jin, Yuxuan Bian, Shiyi Zhang, Haojun Xu, Shuai Lu, Xin Han, Wei Tang, Haoyang Huang, Nan Duan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.09150v1.pdf)  
  Keywords: architecture, streaming, autoregressive, diffusion model, t2v, distillation, super-resolution, video generation, efficient, video diffusion  
- **[Physics in 2-Steps: Locking Motion Priors Before Visual Refinement Erases Them](https://arxiv.org/abs/2606.06361v1)**  
  Authors: Woojung Han, Seil Kang, Youngjun Jun, Min-Hung Chen, Fu-En Yang, Seong Jae Hwang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.06361v1.pdf)  
  Keywords: denoising, physics, diffusion model, image-to-video, physical, trajectory, video diffusion  
- **[RhymeFlow: Training-Free Acceleration for Video Generation with Asynchronous Denoising Flow Scheduling](https://arxiv.org/abs/2606.06309v1)**  
  Authors: Chensheng Dai, Shengjun Zhang, Yifan Li, Zhang Zhang, Zheng Zhu, Yueqi Duan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.06309v1.pdf)  
  Keywords: diffusion transformer, video synthesis, acceleration, denoising, trajectory, video generation, dit  
- **[ReCache: Learning Budget-Aware Caching Schedules for Diffusion Models via REINFORCE](https://arxiv.org/abs/2606.06060v1)**  
  Authors: Mishan Aliev, Eva Neudachina, Ilya Bykov, Aleksandr Oganov, Kirill Struminsky, Aibek Alanov, Denis Rakitin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.06060v1.pdf) | [![GitHub](https://img.shields.io/github/stars/thecrazymage/ReCache?style=social)](https://github.com/thecrazymage/ReCache)  
  Keywords: controllable, diffusion model, denoising, trajectory  
- **[The Invisible Hand of Physics: When Video Diffusion Models Know More Than They Show](https://arxiv.org/abs/2606.05328v1)**  
  Authors: Parsa Esmati, Somjit Nath, Katja Hofmann, Derek Nowrouzezahrai, Samira Ebrahimi Kahou, Majid Mirmehdi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.05328v1.pdf)  
  Keywords: diffusion transformer, world simulator, denoising, physics, diffusion model, physical, video diffusion  

### World Models & Simulation

*Showing the latest 50 out of 124 papers*

- **[RepWAM: World Action Modeling with Representation Visual-Action Tokenizers](https://arxiv.org/abs/2606.13674v1)**  
  Authors: Junke Wang, Qihang Zhang, Shuai Yang, Yiming Luo, Yujun Shen, Zuxuan Wu, Yu-Gang Jiang, Yinghao Xu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13674v1.pdf) | [![GitHub](https://img.shields.io/github/stars/wdrink/RepWAM?style=social)](https://github.com/wdrink/RepWAM)  
  Keywords: simulation, video generation, dynamics, benchmark  
- **[Flex4DHuman: Flexible Multi-view Video Diffusion for 4D Human Reconstruction](https://arxiv.org/abs/2606.13655v1)**  
  Authors: Jen-Hao Cheng, Yipeng Wang, Hao Zhang, Gengshan Yang, Jenq-Neng Hwang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13655v1.pdf)  
  Keywords: architecture, simulation, diffusion model, text-to-video, multi-view video, video diffusion, dit  
- **[Making Foresight Actionable: Repurposing Representation Alignment in World Action Models](https://arxiv.org/abs/2606.12217v1)**  
  Authors: Lu Qiu, Yizhuo Li, Yi Chen, Yuying Ge, Yixiao Ge, Xihui Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.12217v1.pdf)  
  Keywords: video generation, world model, video diffusion  
- **[World Model Self-Distillation: Training World Models to Solve General Tasks](https://arxiv.org/abs/2606.12072v1)**  
  Authors: Sebastian Stapf, Pablo Acuaviva Huertos, Aram Davtyan, Paolo Favaro  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.12072v1.pdf)  
  Keywords: world model, evaluation, diffusion model, distillation, robotics, benchmark, video diffusion, dit  
- **[Next Forcing: Causal World Modeling with Multi-Chunk Prediction](https://arxiv.org/abs/2606.11187v1)**  
  Authors: Gangwei Xu, Qihang Zhang, Jiaming Zhou, Xing Zhu, Yujun Shen, Xin Yang, Yinghao Xu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.11187v1.pdf)  
  Keywords: dynamics, world model, acceleration, denoising, autoregressive, benchmark, physical, video generation  
- **[BiWM: Advancing Open-Source Interactive Video World Models with Bidirectional Autoregression](https://arxiv.org/abs/2606.10135v2)**  
  Authors: Shaohao Rui, Xiaofeng Mao, Zhanyu Zhang, Peijia Lin, Yansong Zhu, Yibo Zhang, Haibin Wan, Weijie Ma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.10135v2.pdf)  
  Keywords: dynamics, camera control, world model, simulation, autoregressive, diffusion model, distillation, style, controllable, interactive, video diffusion  
- **[Latent Spatial Memory for Video World Models](https://arxiv.org/abs/2606.09828v1)**  
  Authors: Weijie Wang, Haoyu Zhao, Yifan Yang, Feng Chen, Zeyu Zhang, Yefei He, Zicheng Duan, Donny Y. Chen, Yuqing Yang, Bohan Zhuang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.09828v1.pdf)  
  Keywords: world model, diffusion model, novel view, depth-guided, video generation  
- **[Echo-Memory: A Controlled Study of Memory in Action World Models](https://arxiv.org/abs/2606.09803v1)**  
  Authors: Wayne King, Zeyue Xue, Yuxuan Bian, Jie Huang, Haoran Li, Yaowei Li, Yaofeng Su, Yuming Li, Haoyu Wang, Shiyi Zhang, Songchun Zhang, Yuwei Niu, Sihan Xu, Junhao Zhuang, Haoyang Huang, Nan Duan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.09803v1.pdf)  
  Keywords: world model, action-conditioned, evaluation, video diffusion, dit  
- **[CP4D: Compositional Physics-aware 4D Scene Generation](https://arxiv.org/abs/2606.09187v1)**  
  Authors: Hanxin Zhu, Cong Wang, Tianyu He, Long Chen, Xin Jin, Chen Gao, Zhibo Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.09187v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://anonymous.4open.science/w/CP4D)  
  Keywords: dynamics, physics, diffusion model, 4d generation, physical, physics-aware, interactive, video diffusion  
- **[DisCo: World Models with Discrete Camera Motion Control](https://arxiv.org/abs/2606.07967v1)**  
  Authors: Hongrui Huang, Junke Wang, Quanhao Li, Yu-Gang Jiang, Zuxuan Wu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.07967v1.pdf)  
  Keywords: world model, motion control, benchmark, video generation, controllable, interactive, dit  



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
