# Awesome Video Diffusions [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of latest research papers, projects and resources related to Video Diffusion Models and Video Generation. Content is automatically updated daily.

> Last Update: 2026-06-22 04:16:28

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

- [3D-aware Video Generation](#3d-aware-video-generation) (22 papers) - Video generation with 3D awareness, multi-view consistency, and 4D content creation
- [Applications](#applications) (57 papers) - Domain-specific applications of video diffusion models
- [Architecture & Efficiency](#architecture-&-efficiency) (361 papers) - Architectural innovations (DiT, UNet), flow matching, and training/inference efficiency
- [Audio & Multi-modal](#audio-&-multi-modal) (29 papers) - Audio-driven and multi-modal conditioned video generation
- [Controllable Generation](#controllable-generation) (133 papers) - Controllable video generation with motion, camera, pose, or layout guidance
- [Human & Character Animation](#human-&-character-animation) (21 papers) - Human-centric video generation including talking heads, dance, and character animation
- [Image-to-Video Generation](#image-to-video-generation) (44 papers) - Methods for animating still images into videos
- [Long Video Generation](#long-video-generation) (137 papers) - Generating temporally consistent long-form videos beyond short clips
- [Personalization & Customization](#personalization-&-customization) (87 papers) - Personalized video generation with custom subjects, identities, or styles
- [Physical Understanding](#physical-understanding) (147 papers) - Physics-aware video generation and dynamics modeling
- [Surveys & Benchmarks](#surveys-&-benchmarks) (236 papers) - Survey papers, benchmarks, and evaluation metrics for video generation
- [Text-to-Video Generation](#text-to-video-generation) (59 papers) - Foundation models and methods for generating videos from text prompts
- [Video Editing](#video-editing) (27 papers) - Diffusion-based video editing, style transfer, and manipulation
- [Video Inpainting & Completion](#video-inpainting-&-completion) (11 papers) - Video inpainting, completion, outpainting, and temporal prediction
- [Video Super-Resolution & Enhancement](#video-super-resolution-&-enhancement) (75 papers) - Video quality improvement, upscaling, restoration, and frame interpolation
- [World Models & Simulation](#world-models-&-simulation) (131 papers) - Video generation as world simulators and interactive environment generation



## Table of Contents

- [Categorized Papers](#categorized-papers)
- [Classic Papers](#classic-papers)
- [Open Source Projects](#open-source-projects)
- [Applications](#applications)
- [Tutorials & Blogs](#tutorials--blogs)





## Categorized Papers

### 3D-aware Video Generation

- **[OmniDrive: An LLM-Choreographed Multi-Agent World Model with Unified Latent Co-Compression for Multi-View Driving Video Generation](https://arxiv.org/abs/2606.17536v1)**  
  Authors: Zijie Meng, Yufei Liu, Chengqian Ma, Zhiyu Li, Jiyuan Liu, Wenhua Nie, Bingcai Wei, Shuqin Chen, Weichen Xu, Jiquan Yuan, Miao Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17536v1.pdf)  
  Keywords: world model, autonomous driving, controllable, dit, layout, video generation, multi-view video  
- **[R2RDreamer: 3D-aware Data Augmentation for Spatially-generalized 2D Manipulation Policies](https://arxiv.org/abs/2606.17040v1)**  
  Authors: Xiuwei Xu, Haowen Sun, Angyuan Ma, Yiwei Zhang, Zhenyu Wu, Xiaofeng Wang, Bingyao Yu, Zheng Zhu, Jie Zhou, Jiwen Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17040v1.pdf)  
  Keywords: controllable, dit, style, 3d-aware, video completion, image-to-video, simulation  
- **[Flex4DHuman: Flexible Multi-view Video Diffusion for 4D Human Reconstruction](https://arxiv.org/abs/2606.13655v2)**  
  Authors: Jen-Hao Cheng, Yipeng Wang, Hao Zhang, Gengshan Yang, Jenq-Neng Hwang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13655v2.pdf)  
  Keywords: architecture, text-to-video, video diffusion, dit, diffusion model, simulation, multi-view video  
- **[Latent Spatial Memory for Video World Models](https://arxiv.org/abs/2606.09828v1)**  
  Authors: Weijie Wang, Haoyu Zhao, Yifan Yang, Feng Chen, Zeyu Zhang, Yefei He, Zicheng Duan, Donny Y. Chen, Yuqing Yang, Bohan Zhuang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.09828v1.pdf)  
  Keywords: world model, depth-guided, diffusion model, novel view, video generation  
- **[CP4D: Compositional Physics-aware 4D Scene Generation](https://arxiv.org/abs/2606.09187v1)**  
  Authors: Hanxin Zhu, Cong Wang, Tianyu He, Long Chen, Xin Jin, Chen Gao, Zhibo Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.09187v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://anonymous.4open.science/w/CP4D)  
  Keywords: dynamics, video diffusion, physics, 4d generation, interactive, diffusion model, physical, physics-aware  
- **[RigPAPR: Rig-Based Animation of Static Neural Point Clouds from a Fixed-Viewpoint Video](https://arxiv.org/abs/2606.06685v1)**  
  Authors: Shichong Peng, Yanshu Zhang, Ke Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.06685v1.pdf)  
  Keywords: novel view, image-to-video, i2v  
- **[PointAction: 3D Points as Universal Action Representations for Robot Control](https://arxiv.org/abs/2606.03943v1)**  
  Authors: Mutian Tong, Han Jiang, Qiao Feng, Lingjie Liu, Jiatao Gu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.03943v1.pdf)  
  Keywords: dynamics, video diffusion, video generation, video prediction, 4d generation, diffusion model, simulation  
- **[RoboDream: Compositional World Models for Scalable Robot Data Synthesis](https://arxiv.org/abs/2606.02577v1)**  
  Authors: Junjie Ye, Rong Xue, Basile Van Hoorick, Runhao Li, Harshitha Rajaprakash, Pavel Tokmakov, Muhammad Zubair Irshad, Vitor Guizilini, Yue Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.02577v1.pdf)  
  Keywords: world model, video diffusion, dit, diffusion model, physical, novel view, trajectory  
- **[Towards 3D-Aware Video Diffusion Models: Render-Free Human Motion Control with Mesh Tokenization](https://arxiv.org/abs/2606.02000v1)**  
  Authors: Jingyun Liang, Min Wei, Shikai Li, Yizeng Han, Hangjie Yuan, Lei Sun, Weihua Chen, Fan Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.02000v1.pdf)  
  Keywords: benchmark, architecture, trajectory, video diffusion, dit, motion control, diffusion model, 3d-aware, video generation, human motion  
- **[Effective Multi-sensor Conditioning for Street-view Novel-view Synthesis](https://arxiv.org/abs/2606.01590v1)**  
  Authors: Zhengfei Kuang, Adam Sun, Liyuan Zhu, Tong Wu, Shengqu Cai, Jonathan Tremblay, Iro Armeni, Ehsan Adeli, Lior Yariv, Gordon Wetzstein  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.01590v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://streetnvs.github.io)  
  Keywords: video diffusion, dit, diffusion model, novel view, trajectory  

### Applications

*Showing the latest 50 out of 57 papers*

- **[Bridging Creative Intent and Visual Quality: Creator-Driven Recurrent Video Generation with Agentic Feedback Loops](https://arxiv.org/abs/2606.18591v1)**  
  Authors: Denis Savytski, Aiden Lei, Heding Liu, Warren Yang, Sihan Liang, Alexander Liu, Zhe Zhao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.18591v1.pdf)  
  Keywords: creative, film, evaluation, dit, video generation  
- **[OmniDrive: An LLM-Choreographed Multi-Agent World Model with Unified Latent Co-Compression for Multi-View Driving Video Generation](https://arxiv.org/abs/2606.17536v1)**  
  Authors: Zijie Meng, Yufei Liu, Chengqian Ma, Zhiyu Li, Jiyuan Liu, Wenhua Nie, Bingcai Wei, Shuqin Chen, Weichen Xu, Jiquan Yuan, Miao Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17536v1.pdf)  
  Keywords: world model, autonomous driving, controllable, dit, layout, video generation, multi-view video  
- **[Qwen-RobotWorld Technical Report: Unifying Embodied World Modeling through Language-Conditioned Video Generation](https://arxiv.org/abs/2606.17030v3)**  
  Authors: Jie Zhang, Xiaoyue Chen, Anzhe Chen, Dayiheng Liu, Deqing Li, Gengze Zhou, Hale Yin, Haoqi Yuan, Haoyang Li, Jiahao Li, Jiazhao Zhang, Jingren Zhou, Kaiyuan Gao, Kun Yan, Lihan Jiang, Ningyuan Tang, Pei Lin, Qihang Peng, Shengming Yin, Tianhe Wu, Tianyi Yan, Xiao Xu, Yan Shu, Yanran Zhang, Ye Wang, Yi Wang, Yilei Chen, Yixian Xu, Yiyang Huang, Yuxiang Chen, Zekai Zhang, Zhendong Wang, Zixing Lei, Zhixuan Liang, Zihao Liu, Zikai Zhou, Chenxu Lv, Xiong-Hui Chen, Chenfei Wu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17030v3.pdf)  
  Keywords: world model, benchmark, autonomous driving, evaluation, dit, physical, diffusion transformer, video generation  
- **[RealityBridge: Bridging Editable 3D Gaussian Splatting Driving Simulations and Real-World Videos](https://arxiv.org/abs/2606.16278v1)**  
  Authors: Zhenhua Wu, Yun Pang, Mingkun Chang, Yuwei Ning, Liangzhi Wang, Yi Xiao, Guanbin Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16278v1.pdf)  
  Keywords: autonomous driving, controllable, dit, temporal consistency, simulation, video generation, autoregressive  
- **[Metis: A Generalizable and Efficient World-Action Model for Autonomous Driving and Urban Navigation](https://arxiv.org/abs/2606.15869v1)**  
  Authors: Jingyu Li, Zhe Liu, Dongnan Hu, Junjie Wu, Zipei Ma, Wenxiao Wu, Chao Han, Zhihui Hao, Zhikang Liu, Kun Zhan, Jiankang Deng, Xiatian Zhu, Li Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.15869v1.pdf)  
  Keywords: autonomous driving, benchmark, architecture, efficient, video generation  
- **[CausalDrive: Real-time Causal World Models for Autonomous Driving](https://arxiv.org/abs/2606.15341v1)**  
  Authors: Tianyi Yan, Huan Zheng, Dubing Chen, Meizhi Qu, Yingying Shen, Lijun Zhou, Mingfei Tu, Bing Wang, Guang Chen, Hangjun Ye, Haiyang Sun, Cheng-zhong Xu, Jianbing Shen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.15341v1.pdf)  
  Keywords: world model, autonomous driving, action-conditioned, architecture, evaluation, controllable, dit, layout, interactive, distillation, simulation, trajectory, autoregressive  
- **[Temporal Backtracking Search for Test-time Generative Video Reasoning](https://arxiv.org/abs/2606.13861v1)**  
  Authors: Sejoon Jun, Zheng Ding, Huangyuan Su, Weirui Ye, Yilun Du  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13861v1.pdf)  
  Keywords: robotics, efficient, video generation, dit, denoising  
- **[World Model Self-Distillation: Training World Models to Solve General Tasks](https://arxiv.org/abs/2606.12072v1)**  
  Authors: Sebastian Stapf, Pablo Acuaviva Huertos, Aram Davtyan, Paolo Favaro  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.12072v1.pdf)  
  Keywords: world model, robotics, benchmark, evaluation, video diffusion, dit, diffusion model, distillation  
- **[CineDance: Towards Next-Generation Multi-Shot Long-Form Cinematic Audio-Video Generation](https://arxiv.org/abs/2606.09639v2)**  
  Authors: Yuheng Chen, Teng Hu, Yuji Wang, Qingdong He, Zhucun Xue, Qianyu Zhou, Jason Li, Lizhuang Ma, Jiangning Zhang, Dacheng Tao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.09639v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://aliothchen.github.io/projects/CineDance)  
  Keywords: long-form, evaluation, video generation, film  
- **[CapRL++: Unified Reinforcement Learning with Verifiable Rewards for Dense Image and Video Captioning](https://arxiv.org/abs/2606.09393v1)**  
  Authors: Penghui Yang, Long Xing, Xiaoyi Dong, Yuhang Zang, Yuhang Cao, Yibin Wang, Yujie Zhou, Jiazi Bu, Jianze Liang, Qidong Huang, Jiaqi Wang, Feng Wu, Dahua Lin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.09393v1.pdf)  
  Keywords: creative, evaluation, benchmark, dit  

### Architecture & Efficiency

*Showing the latest 50 out of 361 papers*

- **[S-Agent: Spatial Tool-Use Elicits Reasoning for Spatial Intelligence](https://arxiv.org/abs/2606.20515v1)**  
  Authors: Yalun Dai, Hao Li, Shulin Tian, Runmao Yao, Yuhao Dong, Fangzhou Hong, Zhaoxi Chen, Fangfu Liu, Baoliang Tian, Dingwen Zhang, Tao Wang, Kim-Hui Yap, Ziwei Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.20515v1.pdf)  
  Keywords: benchmark, dit  
- **[DataMagic: Transforming Tabular Data into Data Insight Video](https://arxiv.org/abs/2606.20388v1)**  
  Authors: Yupeng Xie, Chen Ma, Zhenyang Wang, Liangwei Wang, Jiayi Zhu, Chuxuan Zeng, Zhouan Shen, Boyan Li, Yuyu Luo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.20388v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://datamagic-home.github.io/) | [![Dataset](https://img.shields.io/badge/-Dataset-orange)](https://datamagic-home.github.io)  
  Keywords: architecture, evaluation, video generation, interactive  
- **[The Hidden Evolution of Disguised Visual Context inside the VLM](https://arxiv.org/abs/2606.20077v1)**  
  Authors: Wish Suharitdamrong, Tony Alex, Muhammad Awais, Sara Atito  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.20077v1.pdf)  
  Keywords: architecture, benchmark, dit  
- **[SketchKeyAnime: Reference-anchored Sparse Key-Sketch Animation Synthesis](https://arxiv.org/abs/2606.19958v1)**  
  Authors: Meixi Li, Xianlin Zhang, Yue Zhang, Xueming Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.19958v1.pdf)  
  Keywords: video generation, controllable, video diffusion, dit  
- **[TeleMorpher: Toward Robust Simultaneous Motion-Location Editing](https://arxiv.org/abs/2606.19676v1)**  
  Authors: Haengbok Chung  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.19676v1.pdf)  
  Keywords: evaluation, controllable, dit, diffusion model, video generation  
- **[ImageWAM: Do World Action Models Really Need Video Generation, or Just Image Editing?](https://arxiv.org/abs/2606.19531v1)**  
  Authors: Yuyang Zhang, Wenyao Zhang, Zekun Qi, He Zhang, Haitao Lin, Jingbo Zhang, Yao Mu, Xiaokang Yang, Wenjun Zeng, Xin Jin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.19531v1.pdf)  
  Keywords: world model, dit, video prediction, denoising, video generation  
- **[LooseControlVideo: Directorial Video Control using Spatial Blocking](https://arxiv.org/abs/2606.19495v1)**  
  Authors: Shariq Farooq Bhat, Niloy J. Mitra, Kalyan Sunkavalli  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.19495v1.pdf)  
  Keywords: benchmark, dynamics, evaluation, text-to-video, video generation, dit, layout, trajectory  
- **[Cinematic Compositing Using Character-Environment-Harmonized Video Generation Models](https://arxiv.org/abs/2606.20233v1)**  
  Authors: Tianyi Xiang, Mingming He, Li Ma, Jing Liao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.20233v1.pdf)  
  Keywords: architecture, controllable, video diffusion, video generation, efficient, dit, interactive, physical, denoising  
- **[Taming I2V models for Image HOI Editing: A Cognitive Benchmark and Agentic Self-Correcting Framework](https://arxiv.org/abs/2606.19073v1)**  
  Authors: Jiayi Gao, Qingchao Chen, Yuxin Peng, Yang Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.19073v1.pdf) | [![GitHub](https://img.shields.io/github/stars/oceanflowlab/HOI-Edit?style=social)](https://github.com/oceanflowlab/HOI-Edit)  
  Keywords: image-to-video, benchmark, i2v, dit  
- **[Physics-IQ Verified](https://arxiv.org/abs/2606.18943v1)**  
  Authors: Tim Rädsch, Yuki M Asano, Hilde Kuehne, Stefan Bauer, Priyank Jaini, Robert Geirhos, Carsten T. Lüth  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.18943v1.pdf) | [![GitHub](https://img.shields.io/github/stars/google-deepmind/physics-iq-benchmark?style=social)](https://github.com/google-deepmind/physics-iq-benchmark)  
  Keywords: world model, benchmark, physics, dit, physical, image-to-video, video generation  

### Audio & Multi-modal

- **[PermaVid: Consistent Video Generation Across Edits via Disentangled Context Memory](https://arxiv.org/abs/2606.16449v2)**  
  Authors: Shuai Yang, Bingjie Gao, Ziwei Liu, Jiaqi Wang, Dahua Lin, Tong Wu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16449v2.pdf)  
  Keywords: multi-modal, layout, video generation, dit  
- **[ReFree: Towards Realistic Co-Speech Video Generation via Reward-Free RL and Multilevel Speech Guidance](https://arxiv.org/abs/2606.13304v1)**  
  Authors: Salaheldin Mohamed, M. Hamza Mughal, Rishabh Dabral, Christian Theobalt  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13304v1.pdf)  
  Keywords: speech-driven, evaluation, video generation  
- **[MSUE: Multi-Modal Soccer Understanding Expert](https://arxiv.org/abs/2606.12106v1)**  
  Authors: Litao Li, Yibo Yu, Yufeng Hu, Zhuo Yang, Jiali Wen, Yixin Chen, Yixi Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.12106v1.pdf)  
  Keywords: architecture, long-form, benchmark, multi-modal  
- **[Conan-embedding-v3: Fusing Modality-Specific Models for Omni-Modal Embedding](https://arxiv.org/abs/2606.09331v1)**  
  Authors: Shiyu Li, Zhiyuan Hu, Yifan Wang, Peiming Li, Zheng Wei, Yang Tang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.09331v1.pdf)  
  Keywords: architecture, multi-modal, dynamics  
- **[EgoPressDiff: Multimodal Video Diffusion for Egocentric UV-Domain Hand-Pressure Estimation](https://arxiv.org/abs/2606.06872v1)**  
  Authors: Yuan Zeng, Zilue Gao, Yujia Shi, Zongqing Lu, Wenming Yang, QingMin Liao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.06872v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://egopressdiff.github.io)  
  Keywords: multi-modal, efficient, video diffusion, dit, physical  
- **[Mamba-Enhanced Implicit Motion Learning for Audio-Driven Portrait Animation](https://arxiv.org/abs/2606.03402v2)**  
  Authors: Xuan Wei, Jiahui Chen, Kaiheng Li, Mingyu Shao, Qingqi Hong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.03402v2.pdf)  
  Keywords: gesture, benchmark, dynamics, architecture, audio-driven, diffusion model, human animation, video generation, human motion  
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
  Keywords: benchmark, audio-driven, evaluation, identity, dit, distillation, video generation, avatar  
- **[StreamChar: Long-Horizon Streaming Character Audio-Video Generation with Decoupled Orchestration](https://arxiv.org/abs/2605.25659v1)**  
  Authors: Linrui Tian, Qi Wang, Bang Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25659v1.pdf)  
  Keywords: audio-driven, identity, efficient, dit, streaming, denoising, distillation, video generation, autoregressive  

### Controllable Generation

*Showing the latest 50 out of 133 papers*

- **[SketchKeyAnime: Reference-anchored Sparse Key-Sketch Animation Synthesis](https://arxiv.org/abs/2606.19958v1)**  
  Authors: Meixi Li, Xianlin Zhang, Yue Zhang, Xueming Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.19958v1.pdf)  
  Keywords: video generation, controllable, video diffusion, dit  
- **[TeleMorpher: Toward Robust Simultaneous Motion-Location Editing](https://arxiv.org/abs/2606.19676v1)**  
  Authors: Haengbok Chung  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.19676v1.pdf)  
  Keywords: evaluation, controllable, dit, diffusion model, video generation  
- **[LooseControlVideo: Directorial Video Control using Spatial Blocking](https://arxiv.org/abs/2606.19495v1)**  
  Authors: Shariq Farooq Bhat, Niloy J. Mitra, Kalyan Sunkavalli  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.19495v1.pdf)  
  Keywords: benchmark, dynamics, evaluation, text-to-video, video generation, dit, layout, trajectory  
- **[Cinematic Compositing Using Character-Environment-Harmonized Video Generation Models](https://arxiv.org/abs/2606.20233v1)**  
  Authors: Tianyi Xiang, Mingming He, Li Ma, Jing Liao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.20233v1.pdf)  
  Keywords: architecture, controllable, video diffusion, video generation, efficient, dit, interactive, physical, denoising  
- **[Future Dynamic 3D Reconstruction: A 3D World Model with Disentangled Ego-Motion](https://arxiv.org/abs/2606.18250v1)**  
  Authors: Nils Morbitzer, Jonathan Evers, Artem Savkin, Thomas Stauner, Nassir Navab, Federico Tombari, Stefano Gasperini  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.18250v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://fr3d-wm.github.io)  
  Keywords: world model, video synthesis, dynamics, physical, distillation, trajectory  
- **[EgoCS-400K: An Egocentric Gameplay Dataset for World Models](https://arxiv.org/abs/2606.18180v1)**  
  Authors: Rongjin Guo, Dong Liang, Yuhao Liu, Fang Liu, Tianyu Huang, Gerhard P. Hancke, Rynson W. H. Lau  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.18180v1.pdf)  
  Keywords: world model, action-conditioned, controllable, video generation, dit, interactive, simulation  
- **[OmniDrive: An LLM-Choreographed Multi-Agent World Model with Unified Latent Co-Compression for Multi-View Driving Video Generation](https://arxiv.org/abs/2606.17536v1)**  
  Authors: Zijie Meng, Yufei Liu, Chengqian Ma, Zhiyu Li, Jiyuan Liu, Wenhua Nie, Bingcai Wei, Shuqin Chen, Weichen Xu, Jiquan Yuan, Miao Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17536v1.pdf)  
  Keywords: world model, autonomous driving, controllable, dit, layout, video generation, multi-view video  
- **[SierpinskiCam: Camera-Controlled Video Retaking with Sierpinski Triangle Pattern Cues](https://arxiv.org/abs/2606.17310v1)**  
  Authors: Suttisak Wizadwongsa, Hyelin Nam, Supasorn Suwajanakorn, Jeong Joon Park  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17310v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://hyelinnam.github.io/SierpinskiCam)  
  Keywords: camera control, video diffusion, dit, diffusion model, trajectory  
- **[R2RDreamer: 3D-aware Data Augmentation for Spatially-generalized 2D Manipulation Policies](https://arxiv.org/abs/2606.17040v1)**  
  Authors: Xiuwei Xu, Haowen Sun, Angyuan Ma, Yiwei Zhang, Zhenyu Wu, Xiaofeng Wang, Bingyao Yu, Zheng Zhu, Jie Zhou, Jiwen Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17040v1.pdf)  
  Keywords: controllable, dit, style, 3d-aware, video completion, image-to-video, simulation  
- **[DreamX-World 1.0: A General-Purpose Interactive World Model](https://arxiv.org/abs/2606.16993v1)**  
  Authors: DreamX Team, Yancheng Bai, Rui Chen, Xiangxiang Chu, Rujing Dang, Hao Dou, Bingjie Gao, Qiwen Gu, Siyu Hong, Jiachen Lei, Geng Li, Jifan Li, Ruimin Lin, Qingfeng Shi, Bingze Song, Lei Sun, Jing Tang, Ruitian Tian, Jun Wang, Jiahong Wu, Pengfei Zhang, Shen Zhang, Jiashu Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16993v1.pdf)  
  Keywords: world model, camera control, evaluation, controllable, dit, style, interactive, distillation, image-to-video, autoregressive  

### Human & Character Animation

- **[Avatar V: Scaling Video-Reference Avatar Video Generation](https://arxiv.org/abs/2606.13872v1)**  
  Authors: Benjamin Liang, Ce Chen, Desmond Lin, Ivan Somov, Jiajun Zhao, Jiewei Yuan, Jingfeng Zhang, Junhao Huang, Nik Nolte, Pedram Haqiqi, Penghan Wang, Rong Yan, Rui Zhang, Sam Prokopchuk, Sivan Wang, Viktor Goriachko, Yi Ren, Yuanming Li, Yutao Chen, Zhenhui Ye, Zhibin Hong, Zilong Nie, Zujin Guo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13872v1.pdf)  
  Keywords: benchmark, dynamics, evaluation, acceleration, identity, dit, style, distillation, super-resolution, video generation, avatar, flow matching  
- **[CULTURESCORE: Evaluating Cultural Faithfulness in Video Generation Models](https://arxiv.org/abs/2606.07311v1)**  
  Authors: Anku Rani, Wei Dai, Shravan Nayak, Pattie Maes, Mahdi M. Kalayeh, Paul Pu Liang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.07311v1.pdf)  
  Keywords: gesture, evaluation, video generation, identity  
- **[Resonant Minds: Closed-Loop Social Avatars with Theory of Mind](https://arxiv.org/abs/2606.05896v1)**  
  Authors: Jianxu Shangguan, Jing Xu, Hang Ye, Xiaoxuan Ma, Yizhou Wang, Wentao Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.05896v1.pdf)  
  Keywords: talking head, dynamics, evaluation, controllable, video generation, avatar  
- **[Mamba-Enhanced Implicit Motion Learning for Audio-Driven Portrait Animation](https://arxiv.org/abs/2606.03402v2)**  
  Authors: Xuan Wei, Jiahui Chen, Kaiheng Li, Mingyu Shao, Qingqi Hong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.03402v2.pdf)  
  Keywords: gesture, benchmark, dynamics, architecture, audio-driven, diffusion model, human animation, video generation, human motion  
- **[Towards 3D-Aware Video Diffusion Models: Render-Free Human Motion Control with Mesh Tokenization](https://arxiv.org/abs/2606.02000v1)**  
  Authors: Jingyun Liang, Min Wei, Shikai Li, Yizeng Han, Hangjie Yuan, Lei Sun, Weihua Chen, Fan Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.02000v1.pdf)  
  Keywords: benchmark, architecture, trajectory, video diffusion, dit, motion control, diffusion model, 3d-aware, video generation, human motion  
- **[Auteur: Language-Driven Cinematographic Framing for Human-Centric Video Generation](https://arxiv.org/abs/2606.01900v2)**  
  Authors: Muhammed Burak Kizil, Enes Sanli, Niloy J. Mitra, Xuelin Chen, Erkut Erdem, Aykut Erdem, Duygu Ceylan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.01900v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://cyberiada.github.io/Auteur)  
  Keywords: camera control, video generation, human motion, film  
- **[Archon: A Unified Multimodal Model for Holistic Digital Human Generation](https://arxiv.org/abs/2605.30311v1)**  
  Authors: Chong Bao, Shichen Liu, Lijun Yu, David Futschik, Stylianos Moschoglou, Shefali Srivastava, Ziqian Bai, Feitong Tan, Guofeng Zhang, Zhaopeng Cui, Sean Fanello, Yinda Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30311v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://zju3dv.github.io/archon)  
  Keywords: dynamics, efficient, video diffusion, avatar, autoregressive  
- **[LongCat-Video-Avatar 1.5 Technical Report](https://arxiv.org/abs/2605.26486v1)**  
  Authors: Meituan LongCat Team, Xunliang Cai, Meng Cheng, Feng Gao, Zhe Kong, Jiamu Li, Le Li, Weiheng Li, Hongyu Liu, Shuai Tan, Xiaoming Wei, Tianyu Yang, Yong Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.26486v1.pdf)  
  Keywords: benchmark, audio-driven, evaluation, identity, dit, distillation, video generation, avatar  
- **[RoMo: A Large-Scale, Richly Organized Dataset and Semantic Taxonomy for Human Motion Generation](https://arxiv.org/abs/2605.26241v1)**  
  Authors: Jiahao Zhang, Joseph Liu, Young-Yoon Lee, Seonghyeon Moon, Victor Zordan, Guy Tevet, Karen Liu, Stephen Gould, Oren Jacob, Haomiao Jiang, Mubbasir Kapadia, Yizhak Ben-Shabat  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.26241v1.pdf)  
  Keywords: evaluation, human motion  
- **[iTryOn: Mastering Interactive Video Virtual Try-On with Spatial-Semantic Guidance](https://arxiv.org/abs/2605.21431v2)**  
  Authors: Jun Zheng, Zhengze Xu, Mengting Chen, Jing Wang, Jinsong Lan, Xiaoyong Zhu, Kaifu Zhang, Bo Zheng, Xiaodan Liang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.21431v2.pdf)  
  Keywords: benchmark, dynamics, virtual try-on, controllable, video diffusion, dit, temporal consistency, interactive, diffusion transformer  

### Image-to-Video Generation

- **[Taming I2V models for Image HOI Editing: A Cognitive Benchmark and Agentic Self-Correcting Framework](https://arxiv.org/abs/2606.19073v1)**  
  Authors: Jiayi Gao, Qingchao Chen, Yuxin Peng, Yang Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.19073v1.pdf) | [![GitHub](https://img.shields.io/github/stars/oceanflowlab/HOI-Edit?style=social)](https://github.com/oceanflowlab/HOI-Edit)  
  Keywords: image-to-video, benchmark, i2v, dit  
- **[Physics-IQ Verified](https://arxiv.org/abs/2606.18943v1)**  
  Authors: Tim Rädsch, Yuki M Asano, Hilde Kuehne, Stefan Bauer, Priyank Jaini, Robert Geirhos, Carsten T. Lüth  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.18943v1.pdf) | [![GitHub](https://img.shields.io/github/stars/google-deepmind/physics-iq-benchmark?style=social)](https://github.com/google-deepmind/physics-iq-benchmark)  
  Keywords: world model, benchmark, physics, dit, physical, image-to-video, video generation  
- **[Data-Forcing Distillation: Restoring Diversity and Fidelity in Few-Step Video Generation](https://arxiv.org/abs/2606.18478v1)**  
  Authors: Siyi Chen, Shaowei Liu, Yixuan Jia, Zian Wang, Huan Ling, Qing Qu, Jun Gao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.18478v1.pdf)  
  Keywords: dynamics, text-to-video, video diffusion, efficient, diffusion model, distillation, image-to-video, video generation, autoregressive  
- **[Pulling The REINS: Training-Free Safety Alignment of Video Diffusion Models via Representation Steering](https://arxiv.org/abs/2606.17257v1)**  
  Authors: Rohit Kundu, Arindam Dutta, Sarosij Bose, Athula Balachandran, Amit K. Roy-Chowdhury  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17257v1.pdf)  
  Keywords: concept, evaluation, text-to-video, video diffusion, diffusion model, diffusion transformer, image-to-video, video generation  
- **[R2RDreamer: 3D-aware Data Augmentation for Spatially-generalized 2D Manipulation Policies](https://arxiv.org/abs/2606.17040v1)**  
  Authors: Xiuwei Xu, Haowen Sun, Angyuan Ma, Yiwei Zhang, Zhenyu Wu, Xiaofeng Wang, Bingyao Yu, Zheng Zhu, Jie Zhou, Jiwen Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17040v1.pdf)  
  Keywords: controllable, dit, style, 3d-aware, video completion, image-to-video, simulation  
- **[DreamX-World 1.0: A General-Purpose Interactive World Model](https://arxiv.org/abs/2606.16993v1)**  
  Authors: DreamX Team, Yancheng Bai, Rui Chen, Xiangxiang Chu, Rujing Dang, Hao Dou, Bingjie Gao, Qiwen Gu, Siyu Hong, Jiachen Lei, Geng Li, Jifan Li, Ruimin Lin, Qingfeng Shi, Bingze Song, Lei Sun, Jing Tang, Ruitian Tian, Jun Wang, Jiahong Wu, Pengfei Zhang, Shen Zhang, Jiashu Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16993v1.pdf)  
  Keywords: world model, camera control, evaluation, controllable, dit, style, interactive, distillation, image-to-video, autoregressive  
- **[Closed-Loop Triplet Synergistic Generation for Long-Form Video](https://arxiv.org/abs/2606.16184v1)**  
  Authors: Xinlei Yin, Xiulian Peng, Xiao Li, Zhiwei Xiong, Yan Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16184v1.pdf)  
  Keywords: long video, benchmark, identity, dit, long-form, image-to-video, video generation  
- **[VideoWeave: Unlocking Geometric Consistency in Video Generation via Joint Geometry-Video Modeling](https://arxiv.org/abs/2606.14162v1)**  
  Authors: Xunzhi Xiang, Zixuan Duan, Yabo Chen, Zhengxuan Wei, Guiyu Zhang, Zixiao Gu, Zhe Gao, Haibin Huang, Chi Zhang, Qi Fan, Xuelong Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.14162v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://videoweave.github.io)  
  Keywords: text-to-video, video diffusion, dit, diffusion model, denoising, image-to-video, video generation  
- **[Prompt2Effect: Training-Free Image-to-Video Model Specialization via LoRA Generation](https://arxiv.org/abs/2606.13971v1)**  
  Authors: Xiaomeng Yang, Yanyu Li, Gordon Guocheng Qian, Ivan Skorokhodov, Viacheslav Ivanov, Avalon Vinella, Xuan Zhang, Yanzhi Wang, Sergey Tulyakov, Anil Kag  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13971v1.pdf)  
  Keywords: dit, interactive, diffusion model, i2v, image-to-video, video generation  
- **[RigPAPR: Rig-Based Animation of Static Neural Point Clouds from a Fixed-Viewpoint Video](https://arxiv.org/abs/2606.06685v1)**  
  Authors: Shichong Peng, Yanshu Zhang, Ke Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.06685v1.pdf)  
  Keywords: novel view, image-to-video, i2v  

### Long Video Generation

*Showing the latest 50 out of 137 papers*

- **[UniTemp: Unlocking Video Generation in Any Temporal Order via Bidirectional Distillation](https://arxiv.org/abs/2606.18702v1)**  
  Authors: Lin Zhang, Sicheng Mo, Zefan Cai, Jinhong Lin, Zihao Lin, Jiuxiang Gu, Krishna Kumar Singh, Yuheng Li, Yin Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.18702v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://lzhangbj.github.io/projects/unitemp)  
  Keywords: long video, video diffusion, dit, streaming, diffusion model, distillation, video generation, autoregressive  
- **[SC3-Eval: Evaluating Robot Foundation Models via Self-Consistent Video Generation](https://arxiv.org/abs/2606.18610v1)**  
  Authors: Wei-Cheng Tseng, Gashon Hussein, Yuzhu Dong, Allen Z. Ren, Lucy X. Shi, XuDong Wang, Sergey Levine, Zhaoshuo Li, Jinwei Gu, Florian Shkurti, Ming-Yu Liu, Quan Vuong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.18610v1.pdf)  
  Keywords: world model, action-conditioned, dynamics, dit, physical, video generation, autoregressive  
- **[Data-Forcing Distillation: Restoring Diversity and Fidelity in Few-Step Video Generation](https://arxiv.org/abs/2606.18478v1)**  
  Authors: Siyi Chen, Shaowei Liu, Yixuan Jia, Zian Wang, Huan Ling, Qing Qu, Jun Gao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.18478v1.pdf)  
  Keywords: dynamics, text-to-video, video diffusion, efficient, diffusion model, distillation, image-to-video, video generation, autoregressive  
- **[MaineCoon: Pursuing A Real-Time Audio-Visual Social World Model](https://arxiv.org/abs/2606.17800v1)**  
  Authors: Lichen Bai, Tianhao Zhang, Shitong Shao, Dingwei Tan, Qiyu Zhong, Zhengpeng Xie, Haopeng Li, Qinghao Huang, Dandan Shen, Tengjiao Ji, Wei Wang, Peicheng Wu, Yuxuan Zhao, Xiangyu Zhu, Welly Luo, Shurui Yang, Zeke Xie  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17800v1.pdf)  
  Keywords: world model, benchmark, dynamics, efficient, streaming, interactive, physical, distillation, video generation, autoregressive  
- **[DreamX-World 1.0: A General-Purpose Interactive World Model](https://arxiv.org/abs/2606.16993v1)**  
  Authors: DreamX Team, Yancheng Bai, Rui Chen, Xiangxiang Chu, Rujing Dang, Hao Dou, Bingjie Gao, Qiwen Gu, Siyu Hong, Jiachen Lei, Geng Li, Jifan Li, Ruimin Lin, Qingfeng Shi, Bingze Song, Lei Sun, Jing Tang, Ruitian Tian, Jun Wang, Jiahong Wu, Pengfei Zhang, Shen Zhang, Jiashu Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16993v1.pdf)  
  Keywords: world model, camera control, evaluation, controllable, dit, style, interactive, distillation, image-to-video, autoregressive  
- **[RGFVR: Reference-Guided Face Video Restoration with Flow Matching](https://arxiv.org/abs/2606.16401v1)**  
  Authors: Cem Eteke, Batuhan Tosun, Eckehard Steinbach  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16401v1.pdf) | [![GitHub](https://img.shields.io/github/stars/batuhanntosun/RG-FVR?style=social)](https://github.com/batuhanntosun/RG-FVR)  
  Keywords: text-to-video, identity, dit, temporal consistency, video restoration, flow matching  
- **[RealityBridge: Bridging Editable 3D Gaussian Splatting Driving Simulations and Real-World Videos](https://arxiv.org/abs/2606.16278v1)**  
  Authors: Zhenhua Wu, Yun Pang, Mingkun Chang, Yuwei Ning, Liangzhi Wang, Yi Xiao, Guanbin Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16278v1.pdf)  
  Keywords: autonomous driving, controllable, dit, temporal consistency, simulation, video generation, autoregressive  
- **[Closed-Loop Triplet Synergistic Generation for Long-Form Video](https://arxiv.org/abs/2606.16184v1)**  
  Authors: Xinlei Yin, Xiulian Peng, Xiao Li, Zhiwei Xiong, Yan Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16184v1.pdf)  
  Keywords: long video, benchmark, identity, dit, long-form, image-to-video, video generation  
- **[CausalDrive: Real-time Causal World Models for Autonomous Driving](https://arxiv.org/abs/2606.15341v1)**  
  Authors: Tianyi Yan, Huan Zheng, Dubing Chen, Meizhi Qu, Yingying Shen, Lijun Zhou, Mingfei Tu, Bing Wang, Guang Chen, Hangjun Ye, Haiyang Sun, Cheng-zhong Xu, Jianbing Shen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.15341v1.pdf)  
  Keywords: world model, autonomous driving, action-conditioned, architecture, evaluation, controllable, dit, layout, interactive, distillation, simulation, trajectory, autoregressive  
- **[GeoStream: Toward Precise Camera Controlled Streaming Video Generation](https://arxiv.org/abs/2606.15162v1)**  
  Authors: Yizhou Zhao, Yifan Wang, Xiaoyuan Wang, Yushu Wu, Hao Zhang, Moayed Haji-Ali, Rameen Abdal, Ashkan Mirzaei, Yanyu Li, Willi Menapace, Laszlo Jeni, Sergey Tulyakov, Peter Wonka, Chaoyang Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.15162v1.pdf)  
  Keywords: world model, camera control, dit, streaming, interactive, distillation, video generation, autoregressive  

### Personalization & Customization

*Showing the latest 50 out of 87 papers*

- **[Pulling The REINS: Training-Free Safety Alignment of Video Diffusion Models via Representation Steering](https://arxiv.org/abs/2606.17257v1)**  
  Authors: Rohit Kundu, Arindam Dutta, Sarosij Bose, Athula Balachandran, Amit K. Roy-Chowdhury  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17257v1.pdf)  
  Keywords: concept, evaluation, text-to-video, video diffusion, diffusion model, diffusion transformer, image-to-video, video generation  
- **[R2RDreamer: 3D-aware Data Augmentation for Spatially-generalized 2D Manipulation Policies](https://arxiv.org/abs/2606.17040v1)**  
  Authors: Xiuwei Xu, Haowen Sun, Angyuan Ma, Yiwei Zhang, Zhenyu Wu, Xiaofeng Wang, Bingyao Yu, Zheng Zhu, Jie Zhou, Jiwen Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17040v1.pdf)  
  Keywords: controllable, dit, style, 3d-aware, video completion, image-to-video, simulation  
- **[DreamX-World 1.0: A General-Purpose Interactive World Model](https://arxiv.org/abs/2606.16993v1)**  
  Authors: DreamX Team, Yancheng Bai, Rui Chen, Xiangxiang Chu, Rujing Dang, Hao Dou, Bingjie Gao, Qiwen Gu, Siyu Hong, Jiachen Lei, Geng Li, Jifan Li, Ruimin Lin, Qingfeng Shi, Bingze Song, Lei Sun, Jing Tang, Ruitian Tian, Jun Wang, Jiahong Wu, Pengfei Zhang, Shen Zhang, Jiashu Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16993v1.pdf)  
  Keywords: world model, camera control, evaluation, controllable, dit, style, interactive, distillation, image-to-video, autoregressive  
- **[RGFVR: Reference-Guided Face Video Restoration with Flow Matching](https://arxiv.org/abs/2606.16401v1)**  
  Authors: Cem Eteke, Batuhan Tosun, Eckehard Steinbach  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16401v1.pdf) | [![GitHub](https://img.shields.io/github/stars/batuhanntosun/RG-FVR?style=social)](https://github.com/batuhanntosun/RG-FVR)  
  Keywords: text-to-video, identity, dit, temporal consistency, video restoration, flow matching  
- **[Closed-Loop Triplet Synergistic Generation for Long-Form Video](https://arxiv.org/abs/2606.16184v1)**  
  Authors: Xinlei Yin, Xiulian Peng, Xiao Li, Zhiwei Xiong, Yan Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16184v1.pdf)  
  Keywords: long video, benchmark, identity, dit, long-form, image-to-video, video generation  
- **[NEXUS: Neural Energy Fields for Physically Consistent Contact-Rich 3D Object Dynamics](https://arxiv.org/abs/2606.15015v2)**  
  Authors: Qizhen Ying, Guangming Wang, Yangchen Pan, Victor Adrian Prisacariu, Brian Sheil, Yixiong Jing  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.15015v2.pdf)  
  Keywords: benchmark, dynamics, acceleration, controllable, physics, video generation, dit, style, physical, trajectory  
- **[ReGenHuman: Re-Generating Human Appearances for Realistic Full-Body Video Anonymization](https://arxiv.org/abs/2606.14972v1)**  
  Authors: Adam Sun, Eshaan Barkataki, Arnold Milstein, Gordon Wetzstein, Ehsan Adeli  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.14972v1.pdf)  
  Keywords: video-to-video, identity, video diffusion, dit  
- **[Memento: Reconstruct to Remember for Consistent Long Video Generation](https://arxiv.org/abs/2606.14667v1)**  
  Authors: Xuan Wei, Longbin Ji, Guan Wang, Xiangrui Liu, Zhenyu Zhang, Shuohuan Wang, Yu Sun, Qingqi Hong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.14667v1.pdf)  
  Keywords: long video, identity, dit, long-form, video generation, autoregressive  
- **[Avatar V: Scaling Video-Reference Avatar Video Generation](https://arxiv.org/abs/2606.13872v1)**  
  Authors: Benjamin Liang, Ce Chen, Desmond Lin, Ivan Somov, Jiajun Zhao, Jiewei Yuan, Jingfeng Zhang, Junhao Huang, Nik Nolte, Pedram Haqiqi, Penghan Wang, Rong Yan, Rui Zhang, Sam Prokopchuk, Sivan Wang, Viktor Goriachko, Yi Ren, Yuanming Li, Yutao Chen, Zhenhui Ye, Zhibin Hong, Zilong Nie, Zujin Guo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13872v1.pdf)  
  Keywords: benchmark, dynamics, evaluation, acceleration, identity, dit, style, distillation, super-resolution, video generation, avatar, flow matching  
- **[CineOrchestra: Unified Entity-Centric Conditioning for Cinematic Video Generation](https://arxiv.org/abs/2606.13768v2)**  
  Authors: Sharath Girish, Tsai-Shien Chen, Zhikang Dong, Mukesh Singhal, Hao Chen, Sergey Tulyakov, Aliaksandr Siarohin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13768v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://snap-research.github.io/CineOrchestra)  
  Keywords: camera control, benchmark, text-to-video, video diffusion, dit, diffusion model, video generation, personalization  

### Physical Understanding

*Showing the latest 50 out of 147 papers*

- **[LooseControlVideo: Directorial Video Control using Spatial Blocking](https://arxiv.org/abs/2606.19495v1)**  
  Authors: Shariq Farooq Bhat, Niloy J. Mitra, Kalyan Sunkavalli  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.19495v1.pdf)  
  Keywords: benchmark, dynamics, evaluation, text-to-video, video generation, dit, layout, trajectory  
- **[Cinematic Compositing Using Character-Environment-Harmonized Video Generation Models](https://arxiv.org/abs/2606.20233v1)**  
  Authors: Tianyi Xiang, Mingming He, Li Ma, Jing Liao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.20233v1.pdf)  
  Keywords: architecture, controllable, video diffusion, video generation, efficient, dit, interactive, physical, denoising  
- **[Physics-IQ Verified](https://arxiv.org/abs/2606.18943v1)**  
  Authors: Tim Rädsch, Yuki M Asano, Hilde Kuehne, Stefan Bauer, Priyank Jaini, Robert Geirhos, Carsten T. Lüth  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.18943v1.pdf) | [![GitHub](https://img.shields.io/github/stars/google-deepmind/physics-iq-benchmark?style=social)](https://github.com/google-deepmind/physics-iq-benchmark)  
  Keywords: world model, benchmark, physics, dit, physical, image-to-video, video generation  
- **[SC3-Eval: Evaluating Robot Foundation Models via Self-Consistent Video Generation](https://arxiv.org/abs/2606.18610v1)**  
  Authors: Wei-Cheng Tseng, Gashon Hussein, Yuzhu Dong, Allen Z. Ren, Lucy X. Shi, XuDong Wang, Sergey Levine, Zhaoshuo Li, Jinwei Gu, Florian Shkurti, Ming-Yu Liu, Quan Vuong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.18610v1.pdf)  
  Keywords: world model, action-conditioned, dynamics, dit, physical, video generation, autoregressive  
- **[Data-Forcing Distillation: Restoring Diversity and Fidelity in Few-Step Video Generation](https://arxiv.org/abs/2606.18478v1)**  
  Authors: Siyi Chen, Shaowei Liu, Yixuan Jia, Zian Wang, Huan Ling, Qing Qu, Jun Gao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.18478v1.pdf)  
  Keywords: dynamics, text-to-video, video diffusion, efficient, diffusion model, distillation, image-to-video, video generation, autoregressive  
- **[Future Dynamic 3D Reconstruction: A 3D World Model with Disentangled Ego-Motion](https://arxiv.org/abs/2606.18250v1)**  
  Authors: Nils Morbitzer, Jonathan Evers, Artem Savkin, Thomas Stauner, Nassir Navab, Federico Tombari, Stefano Gasperini  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.18250v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://fr3d-wm.github.io)  
  Keywords: world model, video synthesis, dynamics, physical, distillation, trajectory  
- **[MaineCoon: Pursuing A Real-Time Audio-Visual Social World Model](https://arxiv.org/abs/2606.17800v1)**  
  Authors: Lichen Bai, Tianhao Zhang, Shitong Shao, Dingwei Tan, Qiyu Zhong, Zhengpeng Xie, Haopeng Li, Qinghao Huang, Dandan Shen, Tengjiao Ji, Wei Wang, Peicheng Wu, Yuxuan Zhao, Xiangyu Zhu, Welly Luo, Shurui Yang, Zeke Xie  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17800v1.pdf)  
  Keywords: world model, benchmark, dynamics, efficient, streaming, interactive, physical, distillation, video generation, autoregressive  
- **[AoiZora: Topology-Aware Auto-Parallel Optimization for Inference of Diffusion Transformers](https://arxiv.org/abs/2606.17566v1)**  
  Authors: Kaijian Wang, Yuanyuan Xu, Fanjiang Ye, Ye Cao, Jingwei Zuo, T. S. Eugene Ng, Yarong Mu, Yuke Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17566v1.pdf)  
  Keywords: diffusion transformer, physical, denoising, video diffusion  
- **[Qwen-RobotWorld Technical Report: Unifying Embodied World Modeling through Language-Conditioned Video Generation](https://arxiv.org/abs/2606.17030v3)**  
  Authors: Jie Zhang, Xiaoyue Chen, Anzhe Chen, Dayiheng Liu, Deqing Li, Gengze Zhou, Hale Yin, Haoqi Yuan, Haoyang Li, Jiahao Li, Jiazhao Zhang, Jingren Zhou, Kaiyuan Gao, Kun Yan, Lihan Jiang, Ningyuan Tang, Pei Lin, Qihang Peng, Shengming Yin, Tianhe Wu, Tianyi Yan, Xiao Xu, Yan Shu, Yanran Zhang, Ye Wang, Yi Wang, Yilei Chen, Yixian Xu, Yiyang Huang, Yuxiang Chen, Zekai Zhang, Zhendong Wang, Zixing Lei, Zhixuan Liang, Zihao Liu, Zikai Zhou, Chenxu Lv, Xiong-Hui Chen, Chenfei Wu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17030v3.pdf)  
  Keywords: world model, benchmark, autonomous driving, evaluation, dit, physical, diffusion transformer, video generation  
- **[LaWAM: Latent World Action Models for Efficient Dynamics-Aware Robot Policies](https://arxiv.org/abs/2606.15768v1)**  
  Authors: Jialei Chen, Kai Wang, Kang Chen, Shuaihang Chen, Feng Gao, Wenhao Tang, Zhiyuan Li, Weilin Liu, Zhuyu Yao, Boxun Li, Yuanbo Xu, Chao Yu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.15768v1.pdf)  
  Keywords: world model, action-conditioned, dynamics, efficient, dit, video generation  

### Surveys & Benchmarks

*Showing the latest 50 out of 236 papers*

- **[S-Agent: Spatial Tool-Use Elicits Reasoning for Spatial Intelligence](https://arxiv.org/abs/2606.20515v1)**  
  Authors: Yalun Dai, Hao Li, Shulin Tian, Runmao Yao, Yuhao Dong, Fangzhou Hong, Zhaoxi Chen, Fangfu Liu, Baoliang Tian, Dingwen Zhang, Tao Wang, Kim-Hui Yap, Ziwei Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.20515v1.pdf)  
  Keywords: benchmark, dit  
- **[DataMagic: Transforming Tabular Data into Data Insight Video](https://arxiv.org/abs/2606.20388v1)**  
  Authors: Yupeng Xie, Chen Ma, Zhenyang Wang, Liangwei Wang, Jiayi Zhu, Chuxuan Zeng, Zhouan Shen, Boyan Li, Yuyu Luo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.20388v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://datamagic-home.github.io/) | [![Dataset](https://img.shields.io/badge/-Dataset-orange)](https://datamagic-home.github.io)  
  Keywords: architecture, evaluation, video generation, interactive  
- **[Through the PRISM: Preference Representation in Intermediate States of Video Diffusion Models](https://arxiv.org/abs/2606.20310v1)**  
  Authors: Haoxuan Wu, Lai Man Po, Mengyang Liu, Kun Li, Hongzheng Yang, Wei Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.20310v1.pdf)  
  Keywords: evaluation, video diffusion, video generation, diffusion model, denoising  
- **[The Hidden Evolution of Disguised Visual Context inside the VLM](https://arxiv.org/abs/2606.20077v1)**  
  Authors: Wish Suharitdamrong, Tony Alex, Muhammad Awais, Sara Atito  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.20077v1.pdf)  
  Keywords: architecture, benchmark, dit  
- **[TeleMorpher: Toward Robust Simultaneous Motion-Location Editing](https://arxiv.org/abs/2606.19676v1)**  
  Authors: Haengbok Chung  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.19676v1.pdf)  
  Keywords: evaluation, controllable, dit, diffusion model, video generation  
- **[LooseControlVideo: Directorial Video Control using Spatial Blocking](https://arxiv.org/abs/2606.19495v1)**  
  Authors: Shariq Farooq Bhat, Niloy J. Mitra, Kalyan Sunkavalli  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.19495v1.pdf)  
  Keywords: benchmark, dynamics, evaluation, text-to-video, video generation, dit, layout, trajectory  
- **[Taming I2V models for Image HOI Editing: A Cognitive Benchmark and Agentic Self-Correcting Framework](https://arxiv.org/abs/2606.19073v1)**  
  Authors: Jiayi Gao, Qingchao Chen, Yuxin Peng, Yang Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.19073v1.pdf) | [![GitHub](https://img.shields.io/github/stars/oceanflowlab/HOI-Edit?style=social)](https://github.com/oceanflowlab/HOI-Edit)  
  Keywords: image-to-video, benchmark, i2v, dit  
- **[Physics-IQ Verified](https://arxiv.org/abs/2606.18943v1)**  
  Authors: Tim Rädsch, Yuki M Asano, Hilde Kuehne, Stefan Bauer, Priyank Jaini, Robert Geirhos, Carsten T. Lüth  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.18943v1.pdf) | [![GitHub](https://img.shields.io/github/stars/google-deepmind/physics-iq-benchmark?style=social)](https://github.com/google-deepmind/physics-iq-benchmark)  
  Keywords: world model, benchmark, physics, dit, physical, image-to-video, video generation  
- **[Bridging Creative Intent and Visual Quality: Creator-Driven Recurrent Video Generation with Agentic Feedback Loops](https://arxiv.org/abs/2606.18591v1)**  
  Authors: Denis Savytski, Aiden Lei, Heding Liu, Warren Yang, Sihan Liang, Alexander Liu, Zhe Zhao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.18591v1.pdf)  
  Keywords: creative, film, evaluation, dit, video generation  
- **[MaineCoon: Pursuing A Real-Time Audio-Visual Social World Model](https://arxiv.org/abs/2606.17800v1)**  
  Authors: Lichen Bai, Tianhao Zhang, Shitong Shao, Dingwei Tan, Qiyu Zhong, Zhengpeng Xie, Haopeng Li, Qinghao Huang, Dandan Shen, Tengjiao Ji, Wei Wang, Peicheng Wu, Yuxuan Zhao, Xiangyu Zhu, Welly Luo, Shurui Yang, Zeke Xie  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17800v1.pdf)  
  Keywords: world model, benchmark, dynamics, efficient, streaming, interactive, physical, distillation, video generation, autoregressive  

### Text-to-Video Generation

*Showing the latest 50 out of 59 papers*

- **[LooseControlVideo: Directorial Video Control using Spatial Blocking](https://arxiv.org/abs/2606.19495v1)**  
  Authors: Shariq Farooq Bhat, Niloy J. Mitra, Kalyan Sunkavalli  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.19495v1.pdf)  
  Keywords: benchmark, dynamics, evaluation, text-to-video, video generation, dit, layout, trajectory  
- **[Data-Forcing Distillation: Restoring Diversity and Fidelity in Few-Step Video Generation](https://arxiv.org/abs/2606.18478v1)**  
  Authors: Siyi Chen, Shaowei Liu, Yixuan Jia, Zian Wang, Huan Ling, Qing Qu, Jun Gao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.18478v1.pdf)  
  Keywords: dynamics, text-to-video, video diffusion, efficient, diffusion model, distillation, image-to-video, video generation, autoregressive  
- **[Reasoning Text-to-Video Retrieval for Operating Room Clips via Action-Driven Digital Twins](https://arxiv.org/abs/2606.17298v1)**  
  Authors: Yiqing Shen, Hao Ding, Mathias Unberath  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17298v1.pdf)  
  Keywords: text-to-video, benchmark  
- **[Pulling The REINS: Training-Free Safety Alignment of Video Diffusion Models via Representation Steering](https://arxiv.org/abs/2606.17257v1)**  
  Authors: Rohit Kundu, Arindam Dutta, Sarosij Bose, Athula Balachandran, Amit K. Roy-Chowdhury  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17257v1.pdf)  
  Keywords: concept, evaluation, text-to-video, video diffusion, diffusion model, diffusion transformer, image-to-video, video generation  
- **[Revealing Artifacts via Noise Amplification: A Novel Perspective for AI-Generated Video Detection](https://arxiv.org/abs/2606.16742v1)**  
  Authors: Renxi Cheng, Jie Gui, Hongsong Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16742v1.pdf)  
  Keywords: video generation, benchmark, text-to-video  
- **[RGFVR: Reference-Guided Face Video Restoration with Flow Matching](https://arxiv.org/abs/2606.16401v1)**  
  Authors: Cem Eteke, Batuhan Tosun, Eckehard Steinbach  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16401v1.pdf) | [![GitHub](https://img.shields.io/github/stars/batuhanntosun/RG-FVR?style=social)](https://github.com/batuhanntosun/RG-FVR)  
  Keywords: text-to-video, identity, dit, temporal consistency, video restoration, flow matching  
- **[VideoWeave: Unlocking Geometric Consistency in Video Generation via Joint Geometry-Video Modeling](https://arxiv.org/abs/2606.14162v1)**  
  Authors: Xunzhi Xiang, Zixuan Duan, Yabo Chen, Zhengxuan Wei, Guiyu Zhang, Zixiao Gu, Zhe Gao, Haibin Huang, Chi Zhang, Qi Fan, Xuelong Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.14162v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://videoweave.github.io)  
  Keywords: text-to-video, video diffusion, dit, diffusion model, denoising, image-to-video, video generation  
- **[CineOrchestra: Unified Entity-Centric Conditioning for Cinematic Video Generation](https://arxiv.org/abs/2606.13768v2)**  
  Authors: Sharath Girish, Tsai-Shien Chen, Zhikang Dong, Mukesh Singhal, Hao Chen, Sergey Tulyakov, Aliaksandr Siarohin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13768v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://snap-research.github.io/CineOrchestra)  
  Keywords: camera control, benchmark, text-to-video, video diffusion, dit, diffusion model, video generation, personalization  
- **[Flex4DHuman: Flexible Multi-view Video Diffusion for 4D Human Reconstruction](https://arxiv.org/abs/2606.13655v2)**  
  Authors: Jen-Hao Cheng, Yipeng Wang, Hao Zhang, Gengshan Yang, Jenq-Neng Hwang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13655v2.pdf)  
  Keywords: architecture, text-to-video, video diffusion, dit, diffusion model, simulation, multi-view video  
- **[SpecLoR: Spectral Lookahead Rectification for Motion-Coherent Text-to-Video Generation](https://arxiv.org/abs/2606.11969v1)**  
  Authors: Xu Zhang, Yu Lu, Ruijie Quan, Zhaozheng Chen, Bohan Wang, Yi Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.11969v1.pdf)  
  Keywords: benchmark, text-to-video, dit, physical, video generation, flow matching  

### Video Editing

- **[ReGenHuman: Re-Generating Human Appearances for Realistic Full-Body Video Anonymization](https://arxiv.org/abs/2606.14972v1)**  
  Authors: Adam Sun, Eshaan Barkataki, Arnold Milstein, Gordon Wetzstein, Ehsan Adeli  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.14972v1.pdf)  
  Keywords: video-to-video, identity, video diffusion, dit  
- **[Lip Forcing: Few-Step Autoregressive Diffusion for Real-time Lip Synchronization](https://arxiv.org/abs/2606.11180v1)**  
  Authors: Paul Hyunbin Cho, Jinhyuk Jang, SeokYoung Lee, Joungbin Lee, Siyoon Jin, Heeseong Shin, Jung Yi, Yunjin Park, Chulmin Park, Seungryong Kim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.11180v1.pdf)  
  Keywords: video-to-video, video diffusion, dit, streaming, diffusion model, denoising, trajectory, autoregressive  
- **[CoVEBench: Can Video Editing Models Handle Complex Instructions?](https://arxiv.org/abs/2606.08415v2)**  
  Authors: Jiangtao Wu, Jiaming Wang, Yiwen He, Yuanxing Zhang, Shihao Li, Dunyuan Liu, Xuedong Zhao, Jialu Chen, Zekun Moore Wang, Jiaheng Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.08415v2.pdf)  
  Keywords: video editing, benchmark, style, dit  
- **[TIDE: Task-Isolated Diffusion for Unified Video Editing and Generation](https://arxiv.org/abs/2606.08260v1)**  
  Authors: Qi Liu, Gang Yue, Mingyu Yin, Lisai Zhang, Yidi Wu, Yaole Wang, Yaohui Wang, Chang Yao, Jingyuan Chen, Lin Ma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.08260v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://LittleWork123.github.io/tide)  
  Keywords: video editing, benchmark, dit, diffusion transformer, video generation  
- **[LoomVideo: Unifying Multimodal Inputs into Video Generation and Editing](https://arxiv.org/abs/2606.06042v2)**  
  Authors: Jianzong Wu, Hao Lian, Jiongfan Yang, Dachao Hao, Ye Tian, Yunhai Tong, Jingyuan Zhu, Biaolong Chen, Qiaosong Qi, Aixi Zhang, Wanggui He, Mushui Liu, Jinlong Liu, Pipei Huang, Hao Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.06042v2.pdf)  
  Keywords: video editing, benchmark, architecture, acceleration, efficient, dit, diffusion transformer, video generation  
- **[V2V-Bench: A Comprehensive Benchmark for Video-to-Video Generation Evaluation](https://arxiv.org/abs/2606.05665v1)**  
  Authors: Tao Liu, Leela Krishna, Gouti Pavan Kumar, Sreeja K, Vishav Garg  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.05665v1.pdf)  
  Keywords: benchmark, evaluation, video generation, dit, i2v, t2v, video-to-video  
- **[Bootstrap Your Generator: Unpaired Visual Editing with Flow Matching](https://arxiv.org/abs/2606.03911v1)**  
  Authors: Yoad Tewel, Yuval Atzmon, Gal Chechik, Lior Wolf  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.03911v1.pdf)  
  Keywords: evaluation, video editing, flow matching, dit  
- **[AlbedoEdit: Unified Instance-Level Video Editing with Albedo Guidance](https://arxiv.org/abs/2606.01362v1)**  
  Authors: Xilong Zhou, Bao-Huy Nguyen, Zheng Zeng, Jacob Munkberg, Jon Hasselgren, Thomas Leimkühler, Nima Kalantari, Miloš Hašan, Christian Theobalt  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.01362v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://vcai.mpi-inf.mpg.de/projects/AlbedoEdit)  
  Keywords: creative, video editing, dit  
- **[DeltaCam: Differential Intrinsic Camera Modeling for Video Generation](https://arxiv.org/abs/2605.25266v1)**  
  Authors: Debabrata Mandal, Zhihan Peng, Yujie Wang, Praneeth Chakravarthula  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25266v1.pdf)  
  Keywords: dynamics, controllable, video diffusion, video style transfer, dit, style, video generation, video-to-video  
- **[Geo-Align: Video Generation Alignment via Metric Geometry Reward](https://arxiv.org/abs/2605.23903v1)**  
  Authors: Zizun Li, Haoyu Guo, Runzhe Teng, Chunhua Shen, Tong He  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.23903v1.pdf)  
  Keywords: camera control, dit, physical, video generation, video-to-video  

### Video Inpainting & Completion

- **[ImageWAM: Do World Action Models Really Need Video Generation, or Just Image Editing?](https://arxiv.org/abs/2606.19531v1)**  
  Authors: Yuyang Zhang, Wenyao Zhang, Zekun Qi, He Zhang, Haitao Lin, Jingbo Zhang, Yao Mu, Xiaokang Yang, Wenjun Zeng, Xin Jin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.19531v1.pdf)  
  Keywords: world model, dit, video prediction, denoising, video generation  
- **[R2RDreamer: 3D-aware Data Augmentation for Spatially-generalized 2D Manipulation Policies](https://arxiv.org/abs/2606.17040v1)**  
  Authors: Xiuwei Xu, Haowen Sun, Angyuan Ma, Yiwei Zhang, Zhenyu Wu, Xiaofeng Wang, Bingyao Yu, Zheng Zhu, Jie Zhou, Jiwen Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17040v1.pdf)  
  Keywords: controllable, dit, style, 3d-aware, video completion, image-to-video, simulation  
- **[PointAction: 3D Points as Universal Action Representations for Robot Control](https://arxiv.org/abs/2606.03943v1)**  
  Authors: Mutian Tong, Han Jiang, Qiao Feng, Lingjie Liu, Jiatao Gu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.03943v1.pdf)  
  Keywords: dynamics, video diffusion, video generation, video prediction, 4d generation, diffusion model, simulation  
- **[World Models: A Comprehensive Survey of Architectures, Methodologies, Reasoning Paradigms, and Applications](https://arxiv.org/abs/2606.00133v1)**  
  Authors: Arif Hassan Zidan, Yi Pan, Hanqi Jiang, Ruiyu Yan, Wei Ruan, Zihao Wu, Lifeng Chen, Weihang You, Xinliang Li, Bowen Chen, Huawen Hu, Peilong Wang, Sizhuang Liu, Jing Zhang, Siyuan Li, Zhengliang Liu, Yu Bao, Lin Zhao, Lichao Sun, Dajiang Zhu, Xiang Li, Jinglei Lv, Quanzheng Li, Wei Liu, Tianming Liu, Wei Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.00133v1.pdf)  
  Keywords: world model, robotics, benchmark, autonomous driving, dynamics, architecture, education, evaluation, physics, video prediction, interactive, survey, video generation, medical  
- **[Full-4D: Generating Full-Scope 4D Scenes from a Single-View Video](https://arxiv.org/abs/2605.25500v1)**  
  Authors: Tingxi Chen, Ke Hao, Yabo Chen, Zhengxue Cheng, Rong Xie, Li Song, Haibin Huang, Chi Zhang, Xuelong Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25500v1.pdf)  
  Keywords: multi-view video, video synthesis, video interpolation, video diffusion, dit, interactive, diffusion model, 4d generation, physical, distillation, flow matching  
- **[CRONOS: Benchmarking Counterfactual Physical Consistency in Video Models](https://arxiv.org/abs/2605.23699v1)**  
  Authors: León Begiristain, Olaf Dünkel, Adam Kortylewski  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.23699v1.pdf)  
  Keywords: world model, benchmark, dynamics, evaluation, dit, video prediction, physical  
- **[GEM-4D: Geometry-Enhanced Video World Models for Robot Manipulation](https://arxiv.org/abs/2605.22882v3)**  
  Authors: Kaichen Zhou, Yuzhen Chen, Fangneng Zhan, Hang Hua, Grace Chen, Xinhai Chang, Ao Qu, Yilun Du, Zhuang Liu, Paul Pu Liang, Mengyu Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.22882v3.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://gem-4d.github.io)  
  Keywords: world model, dynamics, architecture, dit, video prediction, physical, simulation  
- **[Goodbye Drift: Anchored Tree Sampling for Long-Horizon Video-to-Video Generation](https://arxiv.org/abs/2605.20476v1)**  
  Authors: Matthew Bendel, Stephen W. Bailey, Mithilesh Vaidya, Sumukh Badam, Xingzhe He  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20476v1.pdf)  
  Keywords: video-to-video, outpainting, video generation, dit, style, distillation, t2v, autoregressive  
- **[Nano World Models: A Minimalist Implementation of Future Video Prediction](https://arxiv.org/abs/2605.23993v2)**  
  Authors: Siqiao Huang, Partha Kaushik, Michael Chen, Hengkai Pan, Kaiwen Geng, Omar Chehab, Fernando Moreno-Pino, Max Simchowitz  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.23993v2.pdf)  
  Keywords: world model, architecture, evaluation, dit, video prediction, interactive, simulation, video generation, autoregressive  
- **[Relit-LiVE: Relight Video by Jointly Learning Environment Video](https://arxiv.org/abs/2605.06658v1)**  
  Authors: Weiqing Xiao, Hong Li, Xiuyu Yang, Houyuan Chen, Wenyi Li, Tianqi Liu, Shaocong Xu, Chongjie Ye, Hao Zhao, Beibei Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.06658v1.pdf) | [![GitHub](https://img.shields.io/github/stars/zhuxing0/Relit-LiVE?style=social)](https://github.com/zhuxing0/Relit-LiVE)  
  Keywords: benchmark, video diffusion, dit, streaming, video prediction, diffusion model, physical  

### Video Super-Resolution & Enhancement

*Showing the latest 50 out of 75 papers*

- **[Through the PRISM: Preference Representation in Intermediate States of Video Diffusion Models](https://arxiv.org/abs/2606.20310v1)**  
  Authors: Haoxuan Wu, Lai Man Po, Mengyang Liu, Kun Li, Hongzheng Yang, Wei Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.20310v1.pdf)  
  Keywords: evaluation, video diffusion, video generation, diffusion model, denoising  
- **[ImageWAM: Do World Action Models Really Need Video Generation, or Just Image Editing?](https://arxiv.org/abs/2606.19531v1)**  
  Authors: Yuyang Zhang, Wenyao Zhang, Zekun Qi, He Zhang, Haitao Lin, Jingbo Zhang, Yao Mu, Xiaokang Yang, Wenjun Zeng, Xin Jin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.19531v1.pdf)  
  Keywords: world model, dit, video prediction, denoising, video generation  
- **[Cinematic Compositing Using Character-Environment-Harmonized Video Generation Models](https://arxiv.org/abs/2606.20233v1)**  
  Authors: Tianyi Xiang, Mingming He, Li Ma, Jing Liao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.20233v1.pdf)  
  Keywords: architecture, controllable, video diffusion, video generation, efficient, dit, interactive, physical, denoising  
- **[AoiZora: Topology-Aware Auto-Parallel Optimization for Inference of Diffusion Transformers](https://arxiv.org/abs/2606.17566v1)**  
  Authors: Kaijian Wang, Yuanyuan Xu, Fanjiang Ye, Ye Cao, Jingwei Zuo, T. S. Eugene Ng, Yarong Mu, Yuke Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17566v1.pdf)  
  Keywords: diffusion transformer, physical, denoising, video diffusion  
- **[RGFVR: Reference-Guided Face Video Restoration with Flow Matching](https://arxiv.org/abs/2606.16401v1)**  
  Authors: Cem Eteke, Batuhan Tosun, Eckehard Steinbach  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16401v1.pdf) | [![GitHub](https://img.shields.io/github/stars/batuhanntosun/RG-FVR?style=social)](https://github.com/batuhanntosun/RG-FVR)  
  Keywords: text-to-video, identity, dit, temporal consistency, video restoration, flow matching  
- **[VideoWeave: Unlocking Geometric Consistency in Video Generation via Joint Geometry-Video Modeling](https://arxiv.org/abs/2606.14162v1)**  
  Authors: Xunzhi Xiang, Zixuan Duan, Yabo Chen, Zhengxuan Wei, Guiyu Zhang, Zixiao Gu, Zhe Gao, Haibin Huang, Chi Zhang, Qi Fan, Xuelong Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.14162v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://videoweave.github.io)  
  Keywords: text-to-video, video diffusion, dit, diffusion model, denoising, image-to-video, video generation  
- **[Avatar V: Scaling Video-Reference Avatar Video Generation](https://arxiv.org/abs/2606.13872v1)**  
  Authors: Benjamin Liang, Ce Chen, Desmond Lin, Ivan Somov, Jiajun Zhao, Jiewei Yuan, Jingfeng Zhang, Junhao Huang, Nik Nolte, Pedram Haqiqi, Penghan Wang, Rong Yan, Rui Zhang, Sam Prokopchuk, Sivan Wang, Viktor Goriachko, Yi Ren, Yuanming Li, Yutao Chen, Zhenhui Ye, Zhibin Hong, Zilong Nie, Zujin Guo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13872v1.pdf)  
  Keywords: benchmark, dynamics, evaluation, acceleration, identity, dit, style, distillation, super-resolution, video generation, avatar, flow matching  
- **[Temporal Backtracking Search for Test-time Generative Video Reasoning](https://arxiv.org/abs/2606.13861v1)**  
  Authors: Sejoon Jun, Zheng Ding, Huangyuan Su, Weirui Ye, Yilun Du  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13861v1.pdf)  
  Keywords: robotics, efficient, video generation, dit, denoising  
- **[World Tracing: Generative Pixel-Aligned Geometry Beyond the Visible](https://arxiv.org/abs/2606.13652v1)**  
  Authors: Hao Zhang, Mohamed El Banani, Jen-Hao Cheng, Paul Zhang, Yi Hua, Ben Mildenhall, Christoph Lassner, Narendra Ahuja, Gengshan Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13652v1.pdf)  
  Keywords: video synthesis, benchmark, dit, diffusion transformer, denoising, flow matching  
- **[Next Forcing: Causal World Modeling with Multi-Chunk Prediction](https://arxiv.org/abs/2606.11187v1)**  
  Authors: Gangwei Xu, Qihang Zhang, Jiaming Zhou, Xing Zhu, Yujun Shen, Xin Yang, Yinghao Xu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.11187v1.pdf)  
  Keywords: world model, benchmark, dynamics, acceleration, physical, denoising, video generation, autoregressive  

### World Models & Simulation

*Showing the latest 50 out of 131 papers*

- **[DataMagic: Transforming Tabular Data into Data Insight Video](https://arxiv.org/abs/2606.20388v1)**  
  Authors: Yupeng Xie, Chen Ma, Zhenyang Wang, Liangwei Wang, Jiayi Zhu, Chuxuan Zeng, Zhouan Shen, Boyan Li, Yuyu Luo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.20388v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://datamagic-home.github.io/) | [![Dataset](https://img.shields.io/badge/-Dataset-orange)](https://datamagic-home.github.io)  
  Keywords: architecture, evaluation, video generation, interactive  
- **[ImageWAM: Do World Action Models Really Need Video Generation, or Just Image Editing?](https://arxiv.org/abs/2606.19531v1)**  
  Authors: Yuyang Zhang, Wenyao Zhang, Zekun Qi, He Zhang, Haitao Lin, Jingbo Zhang, Yao Mu, Xiaokang Yang, Wenjun Zeng, Xin Jin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.19531v1.pdf)  
  Keywords: world model, dit, video prediction, denoising, video generation  
- **[Cinematic Compositing Using Character-Environment-Harmonized Video Generation Models](https://arxiv.org/abs/2606.20233v1)**  
  Authors: Tianyi Xiang, Mingming He, Li Ma, Jing Liao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.20233v1.pdf)  
  Keywords: architecture, controllable, video diffusion, video generation, efficient, dit, interactive, physical, denoising  
- **[Physics-IQ Verified](https://arxiv.org/abs/2606.18943v1)**  
  Authors: Tim Rädsch, Yuki M Asano, Hilde Kuehne, Stefan Bauer, Priyank Jaini, Robert Geirhos, Carsten T. Lüth  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.18943v1.pdf) | [![GitHub](https://img.shields.io/github/stars/google-deepmind/physics-iq-benchmark?style=social)](https://github.com/google-deepmind/physics-iq-benchmark)  
  Keywords: world model, benchmark, physics, dit, physical, image-to-video, video generation  
- **[SC3-Eval: Evaluating Robot Foundation Models via Self-Consistent Video Generation](https://arxiv.org/abs/2606.18610v1)**  
  Authors: Wei-Cheng Tseng, Gashon Hussein, Yuzhu Dong, Allen Z. Ren, Lucy X. Shi, XuDong Wang, Sergey Levine, Zhaoshuo Li, Jinwei Gu, Florian Shkurti, Ming-Yu Liu, Quan Vuong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.18610v1.pdf)  
  Keywords: world model, action-conditioned, dynamics, dit, physical, video generation, autoregressive  
- **[Future Dynamic 3D Reconstruction: A 3D World Model with Disentangled Ego-Motion](https://arxiv.org/abs/2606.18250v1)**  
  Authors: Nils Morbitzer, Jonathan Evers, Artem Savkin, Thomas Stauner, Nassir Navab, Federico Tombari, Stefano Gasperini  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.18250v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://fr3d-wm.github.io)  
  Keywords: world model, video synthesis, dynamics, physical, distillation, trajectory  
- **[EgoCS-400K: An Egocentric Gameplay Dataset for World Models](https://arxiv.org/abs/2606.18180v1)**  
  Authors: Rongjin Guo, Dong Liang, Yuhao Liu, Fang Liu, Tianyu Huang, Gerhard P. Hancke, Rynson W. H. Lau  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.18180v1.pdf)  
  Keywords: world model, action-conditioned, controllable, video generation, dit, interactive, simulation  
- **[MaineCoon: Pursuing A Real-Time Audio-Visual Social World Model](https://arxiv.org/abs/2606.17800v1)**  
  Authors: Lichen Bai, Tianhao Zhang, Shitong Shao, Dingwei Tan, Qiyu Zhong, Zhengpeng Xie, Haopeng Li, Qinghao Huang, Dandan Shen, Tengjiao Ji, Wei Wang, Peicheng Wu, Yuxuan Zhao, Xiangyu Zhu, Welly Luo, Shurui Yang, Zeke Xie  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17800v1.pdf)  
  Keywords: world model, benchmark, dynamics, efficient, streaming, interactive, physical, distillation, video generation, autoregressive  
- **[OmniDrive: An LLM-Choreographed Multi-Agent World Model with Unified Latent Co-Compression for Multi-View Driving Video Generation](https://arxiv.org/abs/2606.17536v1)**  
  Authors: Zijie Meng, Yufei Liu, Chengqian Ma, Zhiyu Li, Jiyuan Liu, Wenhua Nie, Bingcai Wei, Shuqin Chen, Weichen Xu, Jiquan Yuan, Miao Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17536v1.pdf)  
  Keywords: world model, autonomous driving, controllable, dit, layout, video generation, multi-view video  
- **[R2RDreamer: 3D-aware Data Augmentation for Spatially-generalized 2D Manipulation Policies](https://arxiv.org/abs/2606.17040v1)**  
  Authors: Xiuwei Xu, Haowen Sun, Angyuan Ma, Yiwei Zhang, Zhenyu Wu, Xiaofeng Wang, Bingyao Yu, Zheng Zhu, Jie Zhou, Jiwen Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17040v1.pdf)  
  Keywords: controllable, dit, style, 3d-aware, video completion, image-to-video, simulation  



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
