# Awesome Video Diffusions [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of latest research papers, projects and resources related to Video Diffusion Models and Video Generation. Content is automatically updated daily.

> Last Update: 2026-06-16 04:09:36

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
- [Applications](#applications) (58 papers) - Domain-specific applications of video diffusion models
- [Architecture & Efficiency](#architecture-&-efficiency) (363 papers) - Architectural innovations (DiT, UNet), flow matching, and training/inference efficiency
- [Audio & Multi-modal](#audio-&-multi-modal) (32 papers) - Audio-driven and multi-modal conditioned video generation
- [Controllable Generation](#controllable-generation) (129 papers) - Controllable video generation with motion, camera, pose, or layout guidance
- [Human & Character Animation](#human-&-character-animation) (23 papers) - Human-centric video generation including talking heads, dance, and character animation
- [Image-to-Video Generation](#image-to-video-generation) (43 papers) - Methods for animating still images into videos
- [Long Video Generation](#long-video-generation) (136 papers) - Generating temporally consistent long-form videos beyond short clips
- [Personalization & Customization](#personalization-&-customization) (90 papers) - Personalized video generation with custom subjects, identities, or styles
- [Physical Understanding](#physical-understanding) (142 papers) - Physics-aware video generation and dynamics modeling
- [Surveys & Benchmarks](#surveys-&-benchmarks) (237 papers) - Survey papers, benchmarks, and evaluation metrics for video generation
- [Text-to-Video Generation](#text-to-video-generation) (56 papers) - Foundation models and methods for generating videos from text prompts
- [Video Editing](#video-editing) (29 papers) - Diffusion-based video editing, style transfer, and manipulation
- [Video Inpainting & Completion](#video-inpainting-&-completion) (10 papers) - Video inpainting, completion, outpainting, and temporal prediction
- [Video Super-Resolution & Enhancement](#video-super-resolution-&-enhancement) (75 papers) - Video quality improvement, upscaling, restoration, and frame interpolation
- [World Models & Simulation](#world-models-&-simulation) (123 papers) - Video generation as world simulators and interactive environment generation



## Table of Contents

- [Categorized Papers](#categorized-papers)
- [Classic Papers](#classic-papers)
- [Open Source Projects](#open-source-projects)
- [Applications](#applications)
- [Tutorials & Blogs](#tutorials--blogs)





## Categorized Papers

### 3D-aware Video Generation

- **[R2RDreamer: 3D-aware Data Augmentation for Spatially-generalized 2D Manipulation Policies](https://arxiv.org/abs/2606.17040v1)**  
  Authors: Xiuwei Xu, Haowen Sun, Angyuan Ma, Yiwei Zhang, Zhenyu Wu, Xiaofeng Wang, Bingyao Yu, Zheng Zhu, Jie Zhou, Jiwen Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17040v1.pdf)  
  Keywords: image-to-video, simulation, style, controllable, 3d-aware, video completion, dit  
- **[Flex4DHuman: Flexible Multi-view Video Diffusion for 4D Human Reconstruction](https://arxiv.org/abs/2606.13655v2)**  
  Authors: Jen-Hao Cheng, Yipeng Wang, Hao Zhang, Gengshan Yang, Jenq-Neng Hwang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13655v2.pdf)  
  Keywords: simulation, video diffusion, architecture, diffusion model, multi-view video, text-to-video, dit  
- **[Latent Spatial Memory for Video World Models](https://arxiv.org/abs/2606.09828v1)**  
  Authors: Weijie Wang, Haoyu Zhao, Yifan Yang, Feng Chen, Zeyu Zhang, Yefei He, Zicheng Duan, Donny Y. Chen, Yuqing Yang, Bohan Zhuang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.09828v1.pdf)  
  Keywords: novel view, world model, video generation, depth-guided, diffusion model  
- **[CP4D: Compositional Physics-aware 4D Scene Generation](https://arxiv.org/abs/2606.09187v1)**  
  Authors: Hanxin Zhu, Cong Wang, Tianyu He, Long Chen, Xin Jin, Chen Gao, Zhibo Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.09187v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://anonymous.4open.science/w/CP4D)  
  Keywords: 4d generation, video diffusion, physics, interactive, physical, diffusion model, dynamics, physics-aware  
- **[RigPAPR: Rig-Based Animation of Static Neural Point Clouds from a Fixed-Viewpoint Video](https://arxiv.org/abs/2606.06685v1)**  
  Authors: Shichong Peng, Yanshu Zhang, Ke Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.06685v1.pdf)  
  Keywords: novel view, i2v, image-to-video  
- **[PointAction: 3D Points as Universal Action Representations for Robot Control](https://arxiv.org/abs/2606.03943v1)**  
  Authors: Mutian Tong, Han Jiang, Qiao Feng, Lingjie Liu, Jiatao Gu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.03943v1.pdf)  
  Keywords: simulation, video prediction, video diffusion, 4d generation, video generation, diffusion model, dynamics  
- **[RoboDream: Compositional World Models for Scalable Robot Data Synthesis](https://arxiv.org/abs/2606.02577v1)**  
  Authors: Junjie Ye, Rong Xue, Basile Van Hoorick, Runhao Li, Harshitha Rajaprakash, Pavel Tokmakov, Muhammad Zubair Irshad, Vitor Guizilini, Yue Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.02577v1.pdf)  
  Keywords: novel view, video diffusion, trajectory, world model, physical, diffusion model, dit  
- **[Towards 3D-Aware Video Diffusion Models: Render-Free Human Motion Control with Mesh Tokenization](https://arxiv.org/abs/2606.02000v1)**  
  Authors: Jingyun Liang, Min Wei, Shikai Li, Yizeng Han, Hangjie Yuan, Lei Sun, Weihua Chen, Fan Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.02000v1.pdf)  
  Keywords: benchmark, motion control, video diffusion, trajectory, video generation, architecture, 3d-aware, human motion, diffusion model, dit  
- **[Effective Multi-sensor Conditioning for Street-view Novel-view Synthesis](https://arxiv.org/abs/2606.01590v1)**  
  Authors: Zhengfei Kuang, Adam Sun, Liyuan Zhu, Tong Wu, Shengqu Cai, Jonathan Tremblay, Iro Armeni, Ehsan Adeli, Lior Yariv, Gordon Wetzstein  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.01590v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://streetnvs.github.io)  
  Keywords: novel view, video diffusion, trajectory, diffusion model, dit  
- **[Real2SAM2Real: Generative 3D Caches as Complementary Context for Video Diffusion](https://arxiv.org/abs/2606.00299v1)**  
  Authors: Jiayi Wu, Haoming Cai, Cornelia Fermuller, Christopher Metzler, Yiannis Aloimonos  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.00299v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://jiayi-wu-leo.github.io/real2sam2real)  
  Keywords: video diffusion, temporal consistency, 3d-aware, diffusion model, dynamics, dit  

### Applications

*Showing the latest 50 out of 58 papers*

- **[Qwen-RobotWorld Technical Report: Unifying Embodied World Modeling through Language-Conditioned Video Generation](https://arxiv.org/abs/2606.17030v1)**  
  Authors: Jie Zhang, Xiaoyue Chen, Anzhe Chen, Chenxu Lv, Deqing Li, Gengze Zhou, Hang Yin, Haoqi Yuan, Haoyang Li, Jiahao Li, Jiazhao Zhang, Jingren Zhou, Kaiyuan Gao, Kun Yan, Lihan Jiang, Ningyuan Tang, Pei Lin, Qihang Peng, Shengming Yin, Tianhe Wu, Tianyi Yan, Xiao Xu, Yan Shu, Yanran Zhang, Ye Wang, Yi Wang, Yilei Chen, Yixian Xu, Yiyang Huang, Yuxiang Chen, Zekai Zhang, Zhendong Wang, Zhixing Lei, Zhixuan Liang, Zihao Liu, Zikai Zhou, Xiong-Hui Chen, Chenfei Wu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17030v1.pdf)  
  Keywords: benchmark, diffusion transformer, autonomous driving, world model, evaluation, video generation, physical, dit  
- **[RealityBridge: Bridging Editable 3D Gaussian Splatting Driving Simulations and Real-World Videos](https://arxiv.org/abs/2606.16278v1)**  
  Authors: Zhenhua Wu, Yun Pang, Mingkun Chang, Yuwei Ning, Liangzhi Wang, Yi Xiao, Guanbin Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16278v1.pdf)  
  Keywords: simulation, autonomous driving, controllable, video generation, temporal consistency, autoregressive, dit  
- **[Metis: A Generalizable and Efficient World-Action Model for Autonomous Driving and Urban Navigation](https://arxiv.org/abs/2606.15869v1)**  
  Authors: Jingyu Li, Zhe Liu, Dongnan Hu, Junjie Wu, Zipei Ma, Wenxiao Wu, Chao Han, Zhihui Hao, Zhikang Liu, Kun Zhan, Jiankang Deng, Xiatian Zhu, Li Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.15869v1.pdf)  
  Keywords: benchmark, video generation, architecture, efficient, autonomous driving  
- **[CausalDrive: Real-time Causal World Models for Autonomous Driving](https://arxiv.org/abs/2606.15341v1)**  
  Authors: Tianyi Yan, Huan Zheng, Dubing Chen, Meizhi Qu, Yingying Shen, Lijun Zhou, Mingfei Tu, Bing Wang, Guang Chen, Hangjun Ye, Haiyang Sun, Cheng-zhong Xu, Jianbing Shen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.15341v1.pdf)  
  Keywords: simulation, distillation, autonomous driving, trajectory, action-conditioned, controllable, layout, evaluation, world model, interactive, architecture, autoregressive, dit  
- **[Temporal Backtracking Search for Test-time Generative Video Reasoning](https://arxiv.org/abs/2606.13861v1)**  
  Authors: Sejoon Jun, Zheng Ding, Huangyuan Su, Weirui Ye, Yilun Du  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13861v1.pdf)  
  Keywords: video generation, robotics, denoising, efficient, dit  
- **[World Model Self-Distillation: Training World Models to Solve General Tasks](https://arxiv.org/abs/2606.12072v1)**  
  Authors: Sebastian Stapf, Pablo Acuaviva Huertos, Aram Davtyan, Paolo Favaro  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.12072v1.pdf)  
  Keywords: benchmark, distillation, video diffusion, world model, evaluation, robotics, diffusion model, dit  
- **[CineDance: Towards Next-Generation Multi-Shot Long-Form Cinematic Audio-Video Generation](https://arxiv.org/abs/2606.09639v2)**  
  Authors: Yuheng Chen, Teng Hu, Yuji Wang, Qingdong He, Zhucun Xue, Qianyu Zhou, Jason Li, Lizhuang Ma, Jiangning Zhang, Dacheng Tao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.09639v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://aliothchen.github.io/projects/CineDance)  
  Keywords: film, long-form, evaluation, video generation  
- **[CapRL++: Unified Reinforcement Learning with Verifiable Rewards for Dense Image and Video Captioning](https://arxiv.org/abs/2606.09393v1)**  
  Authors: Penghui Yang, Long Xing, Xiaoyi Dong, Yuhang Zang, Yuhang Cao, Yibin Wang, Yujie Zhou, Jiazi Bu, Jianze Liang, Qidong Huang, Jiaqi Wang, Feng Wu, Dahua Lin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.09393v1.pdf)  
  Keywords: benchmark, creative, dit, evaluation  
- **[Temporally Consistent and Controllable Video Generation of 2D Cine CMR via Latent Space Motion Modeling](https://arxiv.org/abs/2606.14759v1)**  
  Authors: Yiheng Cao, Gustavo Andrade-Miranda, Jiatian Zhang, Guillaume Sallé, Xin Gao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.14759v1.pdf)  
  Keywords: medical, controllable, video generation, diffusion model, text-to-video, dit  
- **[LongSpace: Exploring Long-Horizon Spatial Memory from Perception to Recall in Video](https://arxiv.org/abs/2606.05677v1)**  
  Authors: Shiqiang Lang, Jing Liu, Haoyang He, Peiwen Sun, Yuanteng Chen, Tao Liu, Lan Yang, Longteng Guo, Honggang Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.05677v1.pdf)  
  Keywords: benchmark, layout, long video, autonomous driving  

### Architecture & Efficiency

*Showing the latest 50 out of 363 papers*

- **[R2RDreamer: 3D-aware Data Augmentation for Spatially-generalized 2D Manipulation Policies](https://arxiv.org/abs/2606.17040v1)**  
  Authors: Xiuwei Xu, Haowen Sun, Angyuan Ma, Yiwei Zhang, Zhenyu Wu, Xiaofeng Wang, Bingyao Yu, Zheng Zhu, Jie Zhou, Jiwen Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17040v1.pdf)  
  Keywords: image-to-video, simulation, style, controllable, 3d-aware, video completion, dit  
- **[Qwen-RobotWorld Technical Report: Unifying Embodied World Modeling through Language-Conditioned Video Generation](https://arxiv.org/abs/2606.17030v1)**  
  Authors: Jie Zhang, Xiaoyue Chen, Anzhe Chen, Chenxu Lv, Deqing Li, Gengze Zhou, Hang Yin, Haoqi Yuan, Haoyang Li, Jiahao Li, Jiazhao Zhang, Jingren Zhou, Kaiyuan Gao, Kun Yan, Lihan Jiang, Ningyuan Tang, Pei Lin, Qihang Peng, Shengming Yin, Tianhe Wu, Tianyi Yan, Xiao Xu, Yan Shu, Yanran Zhang, Ye Wang, Yi Wang, Yilei Chen, Yixian Xu, Yiyang Huang, Yuxiang Chen, Zekai Zhang, Zhendong Wang, Zhixing Lei, Zhixuan Liang, Zihao Liu, Zikai Zhou, Xiong-Hui Chen, Chenfei Wu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17030v1.pdf)  
  Keywords: benchmark, diffusion transformer, autonomous driving, world model, evaluation, video generation, physical, dit  
- **[DreamX-World 1.0: A General-Purpose Interactive World Model](https://arxiv.org/abs/2606.16993v1)**  
  Authors: DreamX Team, Yancheng Bai, Rui Chen, Xiangxiang Chu, Rujing Dang, Hao Dou, Bingjie Gao, Qiwen Gu, Siyu Hong, Jiachen Lei, Geng Li, Jifan Li, Ruimin Lin, Qingfeng Shi, Bingze Song, Lei Sun, Jing Tang, Ruitian Tian, Jun Wang, Jiahong Wu, Pengfei Zhang, Shen Zhang, Jiashu Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16993v1.pdf)  
  Keywords: image-to-video, distillation, style, controllable, evaluation, camera control, world model, interactive, autoregressive, dit  
- **[PermaVid: Consistent Video Generation Across Edits via Disentangled Context Memory](https://arxiv.org/abs/2606.16449v1)**  
  Authors: Shuai Yang, Bingjie Gao, Ziwei Liu, Jiaqi Wang, Dahua Lin, Tong Wu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16449v1.pdf)  
  Keywords: layout, dit, multi-modal, video generation  
- **[RGFVR: Reference-Guided Face Video Restoration with Flow Matching](https://arxiv.org/abs/2606.16401v1)**  
  Authors: Cem Eteke, Batuhan Tosun, Eckehard Steinbach  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16401v1.pdf) | [![GitHub](https://img.shields.io/github/stars/batuhanntosun/RG-FVR?style=social)](https://github.com/batuhanntosun/RG-FVR)  
  Keywords: flow matching, temporal consistency, identity, video restoration, text-to-video, dit  
- **[Training-free sparse attention based on cumulative energy filtering](https://arxiv.org/abs/2606.16317v1)**  
  Authors: Chunlu Li, Yixuan Pan, Bai Du, Zhenyuan Chen, Yanzhao Li, Hui Dong, Hui Wang, Zhiqiang Zou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16317v1.pdf)  
  Keywords: diffusion transformer, dit, video generation  
- **[RealityBridge: Bridging Editable 3D Gaussian Splatting Driving Simulations and Real-World Videos](https://arxiv.org/abs/2606.16278v1)**  
  Authors: Zhenhua Wu, Yun Pang, Mingkun Chang, Yuwei Ning, Liangzhi Wang, Yi Xiao, Guanbin Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16278v1.pdf)  
  Keywords: simulation, autonomous driving, controllable, video generation, temporal consistency, autoregressive, dit  
- **[Learned Image Compression for Vision-Language-Action Models](https://arxiv.org/abs/2606.16253v1)**  
  Authors: Hyeonjun Kim, Jegwang Ryu, Sangbeom Ha, Junhyeok Lee, Jun-Hyuk Kim, Hyemin Ahn, Jaeho Lee  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16253v1.pdf)  
  Keywords: benchmark, dit  
- **[Closed-Loop Triplet Synergistic Generation for Long-Form Video](https://arxiv.org/abs/2606.16184v1)**  
  Authors: Xinlei Yin, Xiulian Peng, Xiao Li, Zhiwei Xiong, Yan Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16184v1.pdf)  
  Keywords: benchmark, long-form, image-to-video, video generation, long video, identity, dit  
- **[Training-Free Open-Vocabulary Visual Grounding for Remote Sensing Images and Videos](https://arxiv.org/abs/2606.16124v1)**  
  Authors: Ke Li, Di Wang, Yongshan Zhu, Ting Wang, Weiping Ni, Tao Lei, Quan Wang, Xinbo Gao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16124v1.pdf)  
  Keywords: diffusion model, benchmark, efficient  

### Audio & Multi-modal

- **[PermaVid: Consistent Video Generation Across Edits via Disentangled Context Memory](https://arxiv.org/abs/2606.16449v1)**  
  Authors: Shuai Yang, Bingjie Gao, Ziwei Liu, Jiaqi Wang, Dahua Lin, Tong Wu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16449v1.pdf)  
  Keywords: layout, dit, multi-modal, video generation  
- **[ReFree: Towards Realistic Co-Speech Video Generation via Reward-Free RL and Multilevel Speech Guidance](https://arxiv.org/abs/2606.13304v1)**  
  Authors: Salaheldin Mohamed, M. Hamza Mughal, Rishabh Dabral, Christian Theobalt  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13304v1.pdf)  
  Keywords: speech-driven, evaluation, video generation  
- **[MSUE: Multi-Modal Soccer Understanding Expert](https://arxiv.org/abs/2606.12106v1)**  
  Authors: Litao Li, Yibo Yu, Yufeng Hu, Zhuo Yang, Jiali Wen, Yixin Chen, Yixi Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.12106v1.pdf)  
  Keywords: benchmark, multi-modal, long-form, architecture  
- **[Conan-embedding-v3: Fusing Modality-Specific Models for Omni-Modal Embedding](https://arxiv.org/abs/2606.09331v1)**  
  Authors: Shiyu Li, Zhiyuan Hu, Yifan Wang, Peiming Li, Zheng Wei, Yang Tang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.09331v1.pdf)  
  Keywords: architecture, dynamics, multi-modal  
- **[EgoPressDiff: Multimodal Video Diffusion for Egocentric UV-Domain Hand-Pressure Estimation](https://arxiv.org/abs/2606.06872v1)**  
  Authors: Yuan Zeng, Zilue Gao, Yujia Shi, Zongqing Lu, Wenming Yang, QingMin Liao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.06872v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://egopressdiff.github.io)  
  Keywords: video diffusion, multi-modal, physical, efficient, dit  
- **[Mamba-Enhanced Implicit Motion Learning for Audio-Driven Portrait Animation](https://arxiv.org/abs/2606.03402v2)**  
  Authors: Xuan Wei, Jiahui Chen, Kaiheng Li, Mingyu Shao, Qingqi Hong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.03402v2.pdf)  
  Keywords: benchmark, audio-driven, video generation, human animation, architecture, human motion, gesture, diffusion model, dynamics  
- **[Inference-Time Scaling for Joint Audio-Video Generation](https://arxiv.org/abs/2606.03183v1)**  
  Authors: Jaemin Jung, Kyeongha Rho, Inkyu Shin, Joon Son Chung  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.03183v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://jung-jaemin.github.io/ITS-AVGen-Proj)  
  Keywords: benchmark, sound, video generation  
- **[Cohort-Scale Neural Atlases of Ultrasound Video](https://arxiv.org/abs/2606.00890v1)**  
  Authors: Zhuorui Zhang, Roger Pallarès-López, Xuan Wu, Praneeth Namburi, Brian W. Anthony  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.00890v1.pdf)  
  Keywords: sound  
- **[LongCat-Video-Avatar 1.5 Technical Report](https://arxiv.org/abs/2605.26486v1)**  
  Authors: Meituan LongCat Team, Xunliang Cai, Meng Cheng, Feng Gao, Zhe Kong, Jiamu Li, Le Li, Weiheng Li, Hongyu Liu, Shuai Tan, Xiaoming Wei, Tianyu Yang, Yong Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.26486v1.pdf)  
  Keywords: benchmark, distillation, audio-driven, avatar, evaluation, video generation, identity, dit  
- **[StreamChar: Long-Horizon Streaming Character Audio-Video Generation with Decoupled Orchestration](https://arxiv.org/abs/2605.25659v1)**  
  Authors: Linrui Tian, Qi Wang, Bang Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25659v1.pdf)  
  Keywords: distillation, audio-driven, video generation, streaming, identity, denoising, autoregressive, efficient, dit  

### Controllable Generation

*Showing the latest 50 out of 129 papers*

- **[R2RDreamer: 3D-aware Data Augmentation for Spatially-generalized 2D Manipulation Policies](https://arxiv.org/abs/2606.17040v1)**  
  Authors: Xiuwei Xu, Haowen Sun, Angyuan Ma, Yiwei Zhang, Zhenyu Wu, Xiaofeng Wang, Bingyao Yu, Zheng Zhu, Jie Zhou, Jiwen Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17040v1.pdf)  
  Keywords: image-to-video, simulation, style, controllable, 3d-aware, video completion, dit  
- **[DreamX-World 1.0: A General-Purpose Interactive World Model](https://arxiv.org/abs/2606.16993v1)**  
  Authors: DreamX Team, Yancheng Bai, Rui Chen, Xiangxiang Chu, Rujing Dang, Hao Dou, Bingjie Gao, Qiwen Gu, Siyu Hong, Jiachen Lei, Geng Li, Jifan Li, Ruimin Lin, Qingfeng Shi, Bingze Song, Lei Sun, Jing Tang, Ruitian Tian, Jun Wang, Jiahong Wu, Pengfei Zhang, Shen Zhang, Jiashu Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16993v1.pdf)  
  Keywords: image-to-video, distillation, style, controllable, evaluation, camera control, world model, interactive, autoregressive, dit  
- **[PermaVid: Consistent Video Generation Across Edits via Disentangled Context Memory](https://arxiv.org/abs/2606.16449v1)**  
  Authors: Shuai Yang, Bingjie Gao, Ziwei Liu, Jiaqi Wang, Dahua Lin, Tong Wu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16449v1.pdf)  
  Keywords: layout, dit, multi-modal, video generation  
- **[RealityBridge: Bridging Editable 3D Gaussian Splatting Driving Simulations and Real-World Videos](https://arxiv.org/abs/2606.16278v1)**  
  Authors: Zhenhua Wu, Yun Pang, Mingkun Chang, Yuwei Ning, Liangzhi Wang, Yi Xiao, Guanbin Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16278v1.pdf)  
  Keywords: simulation, autonomous driving, controllable, video generation, temporal consistency, autoregressive, dit  
- **[Track2View: 4D-Consistent Camera-Controlled Video Generation via Paired 3D Point Tracks](https://arxiv.org/abs/2606.15534v1)**  
  Authors: Feng Qiao, Zhaochong An, Zhexiao Xiong, Serge Belongie, Nathan Jacobs  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.15534v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://qjizhi.github.io/track2view)  
  Keywords: benchmark, diffusion transformer, video diffusion, trajectory, video generation, dynamics, dit  
- **[CausalDrive: Real-time Causal World Models for Autonomous Driving](https://arxiv.org/abs/2606.15341v1)**  
  Authors: Tianyi Yan, Huan Zheng, Dubing Chen, Meizhi Qu, Yingying Shen, Lijun Zhou, Mingfei Tu, Bing Wang, Guang Chen, Hangjun Ye, Haiyang Sun, Cheng-zhong Xu, Jianbing Shen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.15341v1.pdf)  
  Keywords: simulation, distillation, autonomous driving, trajectory, action-conditioned, controllable, layout, evaluation, world model, interactive, architecture, autoregressive, dit  
- **[GeoStream: Toward Precise Camera Controlled Streaming Video Generation](https://arxiv.org/abs/2606.15162v1)**  
  Authors: Yizhou Zhao, Yifan Wang, Xiaoyuan Wang, Yushu Wu, Hao Zhang, Moayed Haji-Ali, Rameen Abdal, Ashkan Mirzaei, Yanyu Li, Willi Menapace, Laszlo Jeni, Sergey Tulyakov, Peter Wonka, Chaoyang Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.15162v1.pdf)  
  Keywords: distillation, world model, streaming, camera control, video generation, interactive, autoregressive, dit  
- **[NEXUS: Neural Energy Fields for Physically Consistent Contact-Rich 3D Object Dynamics](https://arxiv.org/abs/2606.15015v1)**  
  Authors: Qizhen Ying, Guangming Wang, Yangchen Pan, Victor Adrian Prisacariu, Yixiong Jing  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.15015v1.pdf)  
  Keywords: benchmark, trajectory, style, physics, controllable, acceleration, video generation, physical, dynamics, dit  
- **[CausalMotion: Structured Physical Reasoning as Keyframe and Trajectory Guidance for Training-Free Video Generation](https://arxiv.org/abs/2606.14317v1)**  
  Authors: Sihan Zhuang, Xinyuan Chen, Tianfan Xue, Yaohui Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.14317v1.pdf)  
  Keywords: video diffusion, trajectory, video generation, physical, diffusion model, dynamics, dit  
- **[CineOrchestra: Unified Entity-Centric Conditioning for Cinematic Video Generation](https://arxiv.org/abs/2606.13768v1)**  
  Authors: Sharath Girish, Tsai-Shien Chen, Zhikang Dong, Mukesh Singhal, Hao Chen, Sergey Tulyakov, Aliaksandr Siarohin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13768v1.pdf)  
  Keywords: benchmark, personalization, video diffusion, video generation, camera control, diffusion model, text-to-video, dit  

### Human & Character Animation

- **[Avatar V: Scaling Video-Reference Avatar Video Generation](https://arxiv.org/abs/2606.13872v1)**  
  Authors: Benjamin Liang, Ce Chen, Desmond Lin, Ivan Somov, Jiajun Zhao, Jiewei Yuan, Jingfeng Zhang, Junhao Huang, Nik Nolte, Pedram Haqiqi, Penghan Wang, Rong Yan, Rui Zhang, Sam Prokopchuk, Sivan Wang, Viktor Goriachko, Yi Ren, Yuanming Li, Yutao Chen, Zhenhui Ye, Zhibin Hong, Zilong Nie, Zujin Guo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13872v1.pdf)  
  Keywords: benchmark, flow matching, distillation, super-resolution, style, avatar, evaluation, video generation, acceleration, identity, dynamics, dit  
- **[CULTURESCORE: Evaluating Cultural Faithfulness in Video Generation Models](https://arxiv.org/abs/2606.07311v1)**  
  Authors: Anku Rani, Wei Dai, Shravan Nayak, Pattie Maes, Mahdi M. Kalayeh, Paul Pu Liang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.07311v1.pdf)  
  Keywords: gesture, identity, evaluation, video generation  
- **[Resonant Minds: Closed-Loop Social Avatars with Theory of Mind](https://arxiv.org/abs/2606.05896v1)**  
  Authors: Jianxu Shangguan, Jing Xu, Hang Ye, Xiaoxuan Ma, Yizhou Wang, Wentao Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.05896v1.pdf)  
  Keywords: controllable, avatar, evaluation, video generation, dynamics, talking head  
- **[Mamba-Enhanced Implicit Motion Learning for Audio-Driven Portrait Animation](https://arxiv.org/abs/2606.03402v2)**  
  Authors: Xuan Wei, Jiahui Chen, Kaiheng Li, Mingyu Shao, Qingqi Hong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.03402v2.pdf)  
  Keywords: benchmark, audio-driven, video generation, human animation, architecture, human motion, gesture, diffusion model, dynamics  
- **[Towards 3D-Aware Video Diffusion Models: Render-Free Human Motion Control with Mesh Tokenization](https://arxiv.org/abs/2606.02000v1)**  
  Authors: Jingyun Liang, Min Wei, Shikai Li, Yizeng Han, Hangjie Yuan, Lei Sun, Weihua Chen, Fan Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.02000v1.pdf)  
  Keywords: benchmark, motion control, video diffusion, trajectory, video generation, architecture, 3d-aware, human motion, diffusion model, dit  
- **[Auteur: Language-Driven Cinematographic Framing for Human-Centric Video Generation](https://arxiv.org/abs/2606.01900v2)**  
  Authors: Muhammed Burak Kizil, Enes Sanli, Niloy J. Mitra, Xuelin Chen, Erkut Erdem, Aykut Erdem, Duygu Ceylan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.01900v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://cyberiada.github.io/Auteur)  
  Keywords: film, camera control, human motion, video generation  
- **[Archon: A Unified Multimodal Model for Holistic Digital Human Generation](https://arxiv.org/abs/2605.30311v1)**  
  Authors: Chong Bao, Shichen Liu, Lijun Yu, David Futschik, Stylianos Moschoglou, Shefali Srivastava, Ziqian Bai, Feitong Tan, Guofeng Zhang, Zhaopeng Cui, Sean Fanello, Yinda Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.30311v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://zju3dv.github.io/archon)  
  Keywords: video diffusion, avatar, dynamics, autoregressive, efficient  
- **[LongCat-Video-Avatar 1.5 Technical Report](https://arxiv.org/abs/2605.26486v1)**  
  Authors: Meituan LongCat Team, Xunliang Cai, Meng Cheng, Feng Gao, Zhe Kong, Jiamu Li, Le Li, Weiheng Li, Hongyu Liu, Shuai Tan, Xiaoming Wei, Tianyu Yang, Yong Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.26486v1.pdf)  
  Keywords: benchmark, distillation, audio-driven, avatar, evaluation, video generation, identity, dit  
- **[RoMo: A Large-Scale, Richly Organized Dataset and Semantic Taxonomy for Human Motion Generation](https://arxiv.org/abs/2605.26241v1)**  
  Authors: Jiahao Zhang, Joseph Liu, Young-Yoon Lee, Seonghyeon Moon, Victor Zordan, Guy Tevet, Karen Liu, Stephen Gould, Oren Jacob, Haomiao Jiang, Mubbasir Kapadia, Yizhak Ben-Shabat  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.26241v1.pdf)  
  Keywords: human motion, evaluation  
- **[iTryOn: Mastering Interactive Video Virtual Try-On with Spatial-Semantic Guidance](https://arxiv.org/abs/2605.21431v1)**  
  Authors: Jun Zheng, Zhengze Xu, Mengting Chen, Jing Wang, Jinsong Lan, Xiaoyong Zhu, Kaifu Zhang, Bo Zheng, Xiaodan Liang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.21431v1.pdf)  
  Keywords: benchmark, diffusion transformer, video diffusion, virtual try-on, controllable, temporal consistency, interactive, dynamics, dit  

### Image-to-Video Generation

- **[R2RDreamer: 3D-aware Data Augmentation for Spatially-generalized 2D Manipulation Policies](https://arxiv.org/abs/2606.17040v1)**  
  Authors: Xiuwei Xu, Haowen Sun, Angyuan Ma, Yiwei Zhang, Zhenyu Wu, Xiaofeng Wang, Bingyao Yu, Zheng Zhu, Jie Zhou, Jiwen Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17040v1.pdf)  
  Keywords: image-to-video, simulation, style, controllable, 3d-aware, video completion, dit  
- **[DreamX-World 1.0: A General-Purpose Interactive World Model](https://arxiv.org/abs/2606.16993v1)**  
  Authors: DreamX Team, Yancheng Bai, Rui Chen, Xiangxiang Chu, Rujing Dang, Hao Dou, Bingjie Gao, Qiwen Gu, Siyu Hong, Jiachen Lei, Geng Li, Jifan Li, Ruimin Lin, Qingfeng Shi, Bingze Song, Lei Sun, Jing Tang, Ruitian Tian, Jun Wang, Jiahong Wu, Pengfei Zhang, Shen Zhang, Jiashu Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16993v1.pdf)  
  Keywords: image-to-video, distillation, style, controllable, evaluation, camera control, world model, interactive, autoregressive, dit  
- **[Closed-Loop Triplet Synergistic Generation for Long-Form Video](https://arxiv.org/abs/2606.16184v1)**  
  Authors: Xinlei Yin, Xiulian Peng, Xiao Li, Zhiwei Xiong, Yan Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16184v1.pdf)  
  Keywords: benchmark, long-form, image-to-video, video generation, long video, identity, dit  
- **[VideoWeave: Unlocking Geometric Consistency in Video Generation via Joint Geometry-Video Modeling](https://arxiv.org/abs/2606.14162v1)**  
  Authors: Xunzhi Xiang, Zixuan Duan, Yabo Chen, Zhengxuan Wei, Guiyu Zhang, Zixiao Gu, Zhe Gao, Haibin Huang, Chi Zhang, Qi Fan, Xuelong Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.14162v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://videoweave.github.io)  
  Keywords: image-to-video, video diffusion, video generation, denoising, diffusion model, text-to-video, dit  
- **[Prompt2Effect: Training-Free Image-to-Video Model Specialization via LoRA Generation](https://arxiv.org/abs/2606.13971v1)**  
  Authors: Xiaomeng Yang, Yanyu Li, Gordon Guocheng Qian, Ivan Skorokhodov, Viacheslav Ivanov, Avalon Vinella, Xuan Zhang, Yanzhi Wang, Sergey Tulyakov, Anil Kag  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13971v1.pdf)  
  Keywords: image-to-video, video generation, i2v, interactive, diffusion model, dit  
- **[RigPAPR: Rig-Based Animation of Static Neural Point Clouds from a Fixed-Viewpoint Video](https://arxiv.org/abs/2606.06685v1)**  
  Authors: Shichong Peng, Yanshu Zhang, Ke Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.06685v1.pdf)  
  Keywords: novel view, i2v, image-to-video  
- **[Physics in 2-Steps: Locking Motion Priors Before Visual Refinement Erases Them](https://arxiv.org/abs/2606.06361v1)**  
  Authors: Woojung Han, Seil Kang, Youngjun Jun, Min-Hung Chen, Fu-En Yang, Seong Jae Hwang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.06361v1.pdf)  
  Keywords: image-to-video, video diffusion, trajectory, physics, physical, denoising, diffusion model  
- **[V2V-Bench: A Comprehensive Benchmark for Video-to-Video Generation Evaluation](https://arxiv.org/abs/2606.05665v1)**  
  Authors: Tao Liu, Leela Krishna, Gouti Pavan Kumar, Sreeja K, Vishav Garg  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.05665v1.pdf)  
  Keywords: benchmark, t2v, video-to-video, evaluation, video generation, i2v, dit  
- **[AAD-1: Asymmetric Adversarial Distillation for One-Step Autoregressive Video Generation](https://arxiv.org/abs/2606.03972v2)**  
  Authors: Haobo Li, Yanhong Zeng, Yunhong Lu, Jiapeng Zhu, Hao Ouyang, Qiuyu Wang, Ka Leong Cheng, Yujun Shen, Zhipeng Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.03972v2.pdf)  
  Keywords: image-to-video, distillation, video generation, architecture, autoregressive  
- **[Cosmos 3: Omnimodal World Models for Physical AI](https://arxiv.org/abs/2606.02800v2)**  
  Authors: NVIDIA, :, Aditi, Niket Agarwal, Arslan Ali, Jon Allen, Martin Antolini, Adeline Aubame, Alisson Azzolini, Junjie Bai, Maciej Bala, Yogesh Balaji, Josh Bapst, Aarti Basant, Mukesh Beladiya, Mohammad Qazim Bhat, Zaid Pervaiz Bhat, Dan Blick, Vanni Brighella, Han Cai, Tiffany Cai, Eric Cameracci, Jiaxin Cao, Yulong Cao, Mark Carlson, Carlos Casanova, Ting-Yun Chang, Yan Chang, Yu-Wei Chao, Prithvijit Chattopadhyay, Roshan Chaudhari, Chieh-Yun Chen, Junyu Chen, Ke Chen, Qizhi Chen, Wenkai Chen, Xiaotong Chen, Yu Chen, An-Chieh Cheng, Click Cheng, Xiu Chia, Jeana Choi, Chaeyeon Chung, Wenyan Cong, Yin Cui, Magdalena Dadela, Nalin Dadhich, Wenliang Dai, Joyjit Daw, Alperen Degirmenci, Rodrigo Vieira Del Monte, Robert Denomme, Sameer Dharur, Marco Di Lucca, Ke Ding, Wenhao Ding, Yifan Ding, Yuzhu Dong, Nicole Drumheller, Yilun Du, Aigul Dzhumamuratova, Aleksandr Efitorov, Hamid Eghbalzadeh, Naomi Eigbe, Imad El Hanafi, Hassan Eslami, Benedikt Falk, Jiaojiao Fan, Jim Fan, Amol Fasale, Sergiy Fefilatyev, Liang Feng, Francesco Ferroni, Sanja Fidler, Xiao Fu, Vikram Fugro, Prashant Gaikwad, TJ Galda, Katelyn Gao, Yihuai Gao, Wenhang Ge, Sreyan Ghosh, Arushi Goel, Vivek Goel, Akash Gokul, Rama Govindaraju, Jinwei Gu, Miguel Guerrero, Elfie Guo, Aryaman Gupta, Siddharth Gururani, Hugo Hadfield, Song Han, Ankur Handa, Zekun Hao, Mohammad Harrim, Ali Hassani, Nathan Hayes-Roth, Yufan He, Chris Helvig, Cyrus Hogg, Madison Huang, Michael Huang, Sophia Huang, Yufan Huang, Jacob Huffman, DeLesley Hutchins, Suneel Indupuru, Boris Ivanovic, Arihant Jain, Joel Jang, Ryan Ji, Yanan Jian, Dongfu Jiang, Jingyi Jin, Atharva Joshi, Nikhilesh Joshi, Pranjali Joshi, Andy Ju, Jaehun Jung, Weiwei Kang, Scott Kassekert, Jan Kautz, Ashna Khetan, Julia Kiczka, Slawek Kierat, Gwanghyun Kim, Kuno Kim, Sunny Kim, Kezhi Kong, Xin Kong, Zhifeng Kong, Tomasz Kornuta, Egor Krivov, Hui Kuang, Saurav Kumar, Chia-Wen Kuo, George Kurian, Wojciech Kutak, JF Lafleche, Himangshu Lahkar, Omar Laymoun, Jayjun Lee, Sanggil Lee, Gabriele Leone, Boyi Li, Freya Li, Jiajun Li, Jinfeng Li, Ling Li, Pengcheng Li, Shangru Li, Tingle Li, Xiaolong Li, Xuan Li, Zhaoshuo Li, Zhiqi Li, Hao Liang, Maosheng Liao, Chen-Hsuan Lin, Tsung-Yi Lin, Ming-Yu Liu, Sifei Liu, Zihan Liu, Hai Loc Lu, Xiangyu Lu, Alice Luo, Ruipu Luo, Wenjie Luo, Jiangran Lyu, Martin Ding Ma, Nic Ma, Qianli Ma, Dawid Majchrowski, Louis Marcoux, Miguel Martin, Qing Miao, Ashkan Mirzaei, Shreyas Misra, Kaichun Mo, Durra Mohsin, Hyejin Moon, Pawel Morkisz, Saeid Motiian, Kirill Motkov, Seungjun Nah, Yashraj Narang, Deepak Narayanan, Thabang Ngazimbi, Julian Ouyang, Shubham Pachori, David Page, Yatian Pang, Sehwi Park, Mahesh Patekar, Mostofa Patwary, Marco Pavone, Trung Pham, Wei Ping, Soha Pouya, Shrimai Prabhumoye, Varun Praveen, Delin Qu, Hesam Rabeti, Morteza Ramezanali, Marilyn Reeb, Xuanchi Ren, Kristen Rumley, Wojciech Rymer, Jun Saito, Yeongho Seol, John Shao, Piyush Shekdar, Tianwei Shen, Humphrey Shi, Min Shi, Stella Shi, Kevin Shih, Mohammad Shoeybi, Mateusz Sieniawski, Shuran Song, Alexander Sotelo, Amir Sotoodeh, Sunil Srinivasa, Vignesh Srinivasakumar, Bartosz Stefaniak, Rahul Heinrich Steiger, Shangkun Sun, Jiaxiang Tang, Shitao Tang, Yangyang Tang, Yue Tang, Tolou Tavakkoli, Kayley Ting, Krzysztof Tomala, Wei-Cheng Tseng, Jibin Varghese, Sergei Vasilev, Thomas Volk, Raju Wagwani, Roger Waleffe, Andrew Z. Wang, Boxiang Wang, Haoxiang Wang, Qiao Wang, Shihao Wang, Shijie Wang, Ting-Chun Wang, Yan Wang, Yu Wang, Rohit Watve, David Wehr, Fangyin Wei, Xinshuo Weng, Jay Zhangjie Wu, Kedi Wu, Hongchi Xia, Summer Xiao, Tianjun Xiao, Kevin Xie, Daguang Xu, Jiashu Xu, Mengyao Xu, Ruqing Xu, Xingqian Xu, Yao Xu, Dinghao Yang, Dong Yang, Hans Yang, Xiaodong Yang, Xuning Yang, Yichu Yang, Yurong You, Zhiding Yu, Hao Yuan, Simon Yuen, Xiaohui Zeng, Pengcuo Zeren, Cindy Zha, Haotian Zhang, Jenny Zhang, Jing Zhang, Liangkai Zhang, Paris Zhang, Shun Zhang, Xuanmeng Zhang, Zhizheng Zhang, Ann Zhao, Yilin Zhao, Yuliya Zhautouskaya, Charles Zhou, Fengzhe Zhou, Shilin Zhu, Yuke Zhu, Dima Zhylko, Artur Zolkowski  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.02800v2.pdf) | [![GitHub](https://img.shields.io/github/stars/nvidia/cosmos?style=social)](https://github.com/nvidia/cosmos) | [![Project](https://img.shields.io/badge/-Project-blue)](https://research.nvidia.com/labs/cosmos-lab/cosmos3) | [![HuggingFace](https://img.shields.io/badge/-HuggingFace-yellow)](https://huggingface.co/collections/nvidia/cosmos3)  
  Keywords: benchmark, world simulator, image-to-video, world model, evaluation, architecture, physical  

### Long Video Generation

*Showing the latest 50 out of 136 papers*

- **[DreamX-World 1.0: A General-Purpose Interactive World Model](https://arxiv.org/abs/2606.16993v1)**  
  Authors: DreamX Team, Yancheng Bai, Rui Chen, Xiangxiang Chu, Rujing Dang, Hao Dou, Bingjie Gao, Qiwen Gu, Siyu Hong, Jiachen Lei, Geng Li, Jifan Li, Ruimin Lin, Qingfeng Shi, Bingze Song, Lei Sun, Jing Tang, Ruitian Tian, Jun Wang, Jiahong Wu, Pengfei Zhang, Shen Zhang, Jiashu Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16993v1.pdf)  
  Keywords: image-to-video, distillation, style, controllable, evaluation, camera control, world model, interactive, autoregressive, dit  
- **[RGFVR: Reference-Guided Face Video Restoration with Flow Matching](https://arxiv.org/abs/2606.16401v1)**  
  Authors: Cem Eteke, Batuhan Tosun, Eckehard Steinbach  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16401v1.pdf) | [![GitHub](https://img.shields.io/github/stars/batuhanntosun/RG-FVR?style=social)](https://github.com/batuhanntosun/RG-FVR)  
  Keywords: flow matching, temporal consistency, identity, video restoration, text-to-video, dit  
- **[RealityBridge: Bridging Editable 3D Gaussian Splatting Driving Simulations and Real-World Videos](https://arxiv.org/abs/2606.16278v1)**  
  Authors: Zhenhua Wu, Yun Pang, Mingkun Chang, Yuwei Ning, Liangzhi Wang, Yi Xiao, Guanbin Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16278v1.pdf)  
  Keywords: simulation, autonomous driving, controllable, video generation, temporal consistency, autoregressive, dit  
- **[Closed-Loop Triplet Synergistic Generation for Long-Form Video](https://arxiv.org/abs/2606.16184v1)**  
  Authors: Xinlei Yin, Xiulian Peng, Xiao Li, Zhiwei Xiong, Yan Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16184v1.pdf)  
  Keywords: benchmark, long-form, image-to-video, video generation, long video, identity, dit  
- **[CausalDrive: Real-time Causal World Models for Autonomous Driving](https://arxiv.org/abs/2606.15341v1)**  
  Authors: Tianyi Yan, Huan Zheng, Dubing Chen, Meizhi Qu, Yingying Shen, Lijun Zhou, Mingfei Tu, Bing Wang, Guang Chen, Hangjun Ye, Haiyang Sun, Cheng-zhong Xu, Jianbing Shen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.15341v1.pdf)  
  Keywords: simulation, distillation, autonomous driving, trajectory, action-conditioned, controllable, layout, evaluation, world model, interactive, architecture, autoregressive, dit  
- **[GeoStream: Toward Precise Camera Controlled Streaming Video Generation](https://arxiv.org/abs/2606.15162v1)**  
  Authors: Yizhou Zhao, Yifan Wang, Xiaoyuan Wang, Yushu Wu, Hao Zhang, Moayed Haji-Ali, Rameen Abdal, Ashkan Mirzaei, Yanyu Li, Willi Menapace, Laszlo Jeni, Sergey Tulyakov, Peter Wonka, Chaoyang Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.15162v1.pdf)  
  Keywords: distillation, world model, streaming, camera control, video generation, interactive, autoregressive, dit  
- **[Memento: Reconstruct to Remember for Consistent Long Video Generation](https://arxiv.org/abs/2606.14667v1)**  
  Authors: Xuan Wei, Longbin Ji, Guan Wang, Xiangrui Liu, Zhenyu Zhang, Shuohuan Wang, Yu Sun, Qingqi Hong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.14667v1.pdf)  
  Keywords: long-form, video generation, long video, identity, autoregressive, dit  
- **[TetherCache: Stabilizing Autoregressive Long-Form Video Generation with Gated Recall and Trusted Alignment](https://arxiv.org/abs/2606.13035v1)**  
  Authors: Yu Meng, Xiangyang Luo, Letian Li, Wenyuan Jiang, Chen Gao, Xinlei Chen, Yong Li, Xiao-Ping Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13035v1.pdf)  
  Keywords: long-form, video diffusion, video generation, long video, streaming, diffusion model, autoregressive, dit  
- **[MSUE: Multi-Modal Soccer Understanding Expert](https://arxiv.org/abs/2606.12106v1)**  
  Authors: Litao Li, Yibo Yu, Yufeng Hu, Zhuo Yang, Jiali Wen, Yixin Chen, Yixi Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.12106v1.pdf)  
  Keywords: benchmark, multi-modal, long-form, architecture  
- **[Next Forcing: Causal World Modeling with Multi-Chunk Prediction](https://arxiv.org/abs/2606.11187v1)**  
  Authors: Gangwei Xu, Qihang Zhang, Jiaming Zhou, Xing Zhu, Yujun Shen, Xin Yang, Yinghao Xu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.11187v1.pdf)  
  Keywords: benchmark, world model, video generation, acceleration, physical, denoising, dynamics, autoregressive  

### Personalization & Customization

*Showing the latest 50 out of 90 papers*

- **[R2RDreamer: 3D-aware Data Augmentation for Spatially-generalized 2D Manipulation Policies](https://arxiv.org/abs/2606.17040v1)**  
  Authors: Xiuwei Xu, Haowen Sun, Angyuan Ma, Yiwei Zhang, Zhenyu Wu, Xiaofeng Wang, Bingyao Yu, Zheng Zhu, Jie Zhou, Jiwen Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17040v1.pdf)  
  Keywords: image-to-video, simulation, style, controllable, 3d-aware, video completion, dit  
- **[DreamX-World 1.0: A General-Purpose Interactive World Model](https://arxiv.org/abs/2606.16993v1)**  
  Authors: DreamX Team, Yancheng Bai, Rui Chen, Xiangxiang Chu, Rujing Dang, Hao Dou, Bingjie Gao, Qiwen Gu, Siyu Hong, Jiachen Lei, Geng Li, Jifan Li, Ruimin Lin, Qingfeng Shi, Bingze Song, Lei Sun, Jing Tang, Ruitian Tian, Jun Wang, Jiahong Wu, Pengfei Zhang, Shen Zhang, Jiashu Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16993v1.pdf)  
  Keywords: image-to-video, distillation, style, controllable, evaluation, camera control, world model, interactive, autoregressive, dit  
- **[RGFVR: Reference-Guided Face Video Restoration with Flow Matching](https://arxiv.org/abs/2606.16401v1)**  
  Authors: Cem Eteke, Batuhan Tosun, Eckehard Steinbach  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16401v1.pdf) | [![GitHub](https://img.shields.io/github/stars/batuhanntosun/RG-FVR?style=social)](https://github.com/batuhanntosun/RG-FVR)  
  Keywords: flow matching, temporal consistency, identity, video restoration, text-to-video, dit  
- **[Closed-Loop Triplet Synergistic Generation for Long-Form Video](https://arxiv.org/abs/2606.16184v1)**  
  Authors: Xinlei Yin, Xiulian Peng, Xiao Li, Zhiwei Xiong, Yan Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16184v1.pdf)  
  Keywords: benchmark, long-form, image-to-video, video generation, long video, identity, dit  
- **[NEXUS: Neural Energy Fields for Physically Consistent Contact-Rich 3D Object Dynamics](https://arxiv.org/abs/2606.15015v1)**  
  Authors: Qizhen Ying, Guangming Wang, Yangchen Pan, Victor Adrian Prisacariu, Yixiong Jing  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.15015v1.pdf)  
  Keywords: benchmark, trajectory, style, physics, controllable, acceleration, video generation, physical, dynamics, dit  
- **[ReGenHuman: Re-Generating Human Appearances for Realistic Full-Body Video Anonymization](https://arxiv.org/abs/2606.14972v1)**  
  Authors: Adam Sun, Eshaan Barkataki, Arnold Milstein, Gordon Wetzstein, Ehsan Adeli  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.14972v1.pdf)  
  Keywords: video-to-video, video diffusion, identity, dit  
- **[Memento: Reconstruct to Remember for Consistent Long Video Generation](https://arxiv.org/abs/2606.14667v1)**  
  Authors: Xuan Wei, Longbin Ji, Guan Wang, Xiangrui Liu, Zhenyu Zhang, Shuohuan Wang, Yu Sun, Qingqi Hong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.14667v1.pdf)  
  Keywords: long-form, video generation, long video, identity, autoregressive, dit  
- **[Avatar V: Scaling Video-Reference Avatar Video Generation](https://arxiv.org/abs/2606.13872v1)**  
  Authors: Benjamin Liang, Ce Chen, Desmond Lin, Ivan Somov, Jiajun Zhao, Jiewei Yuan, Jingfeng Zhang, Junhao Huang, Nik Nolte, Pedram Haqiqi, Penghan Wang, Rong Yan, Rui Zhang, Sam Prokopchuk, Sivan Wang, Viktor Goriachko, Yi Ren, Yuanming Li, Yutao Chen, Zhenhui Ye, Zhibin Hong, Zilong Nie, Zujin Guo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13872v1.pdf)  
  Keywords: benchmark, flow matching, distillation, super-resolution, style, avatar, evaluation, video generation, acceleration, identity, dynamics, dit  
- **[CineOrchestra: Unified Entity-Centric Conditioning for Cinematic Video Generation](https://arxiv.org/abs/2606.13768v1)**  
  Authors: Sharath Girish, Tsai-Shien Chen, Zhikang Dong, Mukesh Singhal, Hao Chen, Sergey Tulyakov, Aliaksandr Siarohin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13768v1.pdf)  
  Keywords: benchmark, personalization, video diffusion, video generation, camera control, diffusion model, text-to-video, dit  
- **[A Comprehensive Ecosystem for Open-Domain Customized Video Generation](https://arxiv.org/abs/2606.11783v1)**  
  Authors: Jingxu Zhang, Yuqian Hong, Daneul Kim, Kai Qiu, Qi Dai, Jianmin Bao, Yifan Yang, Xiaoyan Sun, Chong Luo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.11783v1.pdf)  
  Keywords: benchmark, diffusion transformer, video generation, identity, efficient, dit  

### Physical Understanding

*Showing the latest 50 out of 142 papers*

- **[Qwen-RobotWorld Technical Report: Unifying Embodied World Modeling through Language-Conditioned Video Generation](https://arxiv.org/abs/2606.17030v1)**  
  Authors: Jie Zhang, Xiaoyue Chen, Anzhe Chen, Chenxu Lv, Deqing Li, Gengze Zhou, Hang Yin, Haoqi Yuan, Haoyang Li, Jiahao Li, Jiazhao Zhang, Jingren Zhou, Kaiyuan Gao, Kun Yan, Lihan Jiang, Ningyuan Tang, Pei Lin, Qihang Peng, Shengming Yin, Tianhe Wu, Tianyi Yan, Xiao Xu, Yan Shu, Yanran Zhang, Ye Wang, Yi Wang, Yilei Chen, Yixian Xu, Yiyang Huang, Yuxiang Chen, Zekai Zhang, Zhendong Wang, Zhixing Lei, Zhixuan Liang, Zihao Liu, Zikai Zhou, Xiong-Hui Chen, Chenfei Wu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17030v1.pdf)  
  Keywords: benchmark, diffusion transformer, autonomous driving, world model, evaluation, video generation, physical, dit  
- **[LaWAM: Latent World Action Models for Efficient Dynamics-Aware Robot Policies](https://arxiv.org/abs/2606.15768v1)**  
  Authors: Jialei Chen, Kai Wang, Kang Chen, Shuaihang Chen, Feng Gao, Wenhao Tang, Zhiyuan Li, Weilin Liu, Zhuyu Yao, Boxun Li, Yuanbo Xu, Chao Yu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.15768v1.pdf)  
  Keywords: action-conditioned, world model, video generation, dynamics, efficient, dit  
- **[Track2View: 4D-Consistent Camera-Controlled Video Generation via Paired 3D Point Tracks](https://arxiv.org/abs/2606.15534v1)**  
  Authors: Feng Qiao, Zhaochong An, Zhexiao Xiong, Serge Belongie, Nathan Jacobs  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.15534v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://qjizhi.github.io/track2view)  
  Keywords: benchmark, diffusion transformer, video diffusion, trajectory, video generation, dynamics, dit  
- **[NEXUS: Neural Energy Fields for Physically Consistent Contact-Rich 3D Object Dynamics](https://arxiv.org/abs/2606.15015v1)**  
  Authors: Qizhen Ying, Guangming Wang, Yangchen Pan, Victor Adrian Prisacariu, Yixiong Jing  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.15015v1.pdf)  
  Keywords: benchmark, trajectory, style, physics, controllable, acceleration, video generation, physical, dynamics, dit  
- **[CausalMotion: Structured Physical Reasoning as Keyframe and Trajectory Guidance for Training-Free Video Generation](https://arxiv.org/abs/2606.14317v1)**  
  Authors: Sihan Zhuang, Xinyuan Chen, Tianfan Xue, Yaohui Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.14317v1.pdf)  
  Keywords: video diffusion, trajectory, video generation, physical, diffusion model, dynamics, dit  
- **[Avatar V: Scaling Video-Reference Avatar Video Generation](https://arxiv.org/abs/2606.13872v1)**  
  Authors: Benjamin Liang, Ce Chen, Desmond Lin, Ivan Somov, Jiajun Zhao, Jiewei Yuan, Jingfeng Zhang, Junhao Huang, Nik Nolte, Pedram Haqiqi, Penghan Wang, Rong Yan, Rui Zhang, Sam Prokopchuk, Sivan Wang, Viktor Goriachko, Yi Ren, Yuanming Li, Yutao Chen, Zhenhui Ye, Zhibin Hong, Zilong Nie, Zujin Guo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13872v1.pdf)  
  Keywords: benchmark, flow matching, distillation, super-resolution, style, avatar, evaluation, video generation, acceleration, identity, dynamics, dit  
- **[RepWAM: World Action Modeling with Representation Visual-Action Tokenizers](https://arxiv.org/abs/2606.13674v2)**  
  Authors: Junke Wang, Qihang Zhang, Shuai Yang, Yiming Luo, Yujun Shen, Zuxuan Wu, Yu-Gang Jiang, Yinghao Xu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13674v2.pdf) | [![GitHub](https://img.shields.io/github/stars/wdrink/RepWAM?style=social)](https://github.com/wdrink/RepWAM)  
  Keywords: benchmark, dynamics, simulation, video generation  
- **[SpecLoR: Spectral Lookahead Rectification for Motion-Coherent Text-to-Video Generation](https://arxiv.org/abs/2606.11969v1)**  
  Authors: Xu Zhang, Yu Lu, Ruijie Quan, Zhaozheng Chen, Bohan Wang, Yi Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.11969v1.pdf)  
  Keywords: benchmark, flow matching, video generation, physical, text-to-video, dit  
- **[Next Forcing: Causal World Modeling with Multi-Chunk Prediction](https://arxiv.org/abs/2606.11187v1)**  
  Authors: Gangwei Xu, Qihang Zhang, Jiaming Zhou, Xing Zhu, Yujun Shen, Xin Yang, Yinghao Xu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.11187v1.pdf)  
  Keywords: benchmark, world model, video generation, acceleration, physical, denoising, dynamics, autoregressive  
- **[FadeMem: Distance-Aware Memory Consolidation for Autoregressive Video Diffusion](https://arxiv.org/abs/2606.10671v1)**  
  Authors: Yu Lu, Junjie Yang, Piotr Koniusz, YuXin Song, Yi Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.10671v1.pdf)  
  Keywords: video diffusion, long video, identity, dynamics, autoregressive  

### Surveys & Benchmarks

*Showing the latest 50 out of 237 papers*

- **[Qwen-RobotWorld Technical Report: Unifying Embodied World Modeling through Language-Conditioned Video Generation](https://arxiv.org/abs/2606.17030v1)**  
  Authors: Jie Zhang, Xiaoyue Chen, Anzhe Chen, Chenxu Lv, Deqing Li, Gengze Zhou, Hang Yin, Haoqi Yuan, Haoyang Li, Jiahao Li, Jiazhao Zhang, Jingren Zhou, Kaiyuan Gao, Kun Yan, Lihan Jiang, Ningyuan Tang, Pei Lin, Qihang Peng, Shengming Yin, Tianhe Wu, Tianyi Yan, Xiao Xu, Yan Shu, Yanran Zhang, Ye Wang, Yi Wang, Yilei Chen, Yixian Xu, Yiyang Huang, Yuxiang Chen, Zekai Zhang, Zhendong Wang, Zhixing Lei, Zhixuan Liang, Zihao Liu, Zikai Zhou, Xiong-Hui Chen, Chenfei Wu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17030v1.pdf)  
  Keywords: benchmark, diffusion transformer, autonomous driving, world model, evaluation, video generation, physical, dit  
- **[DreamX-World 1.0: A General-Purpose Interactive World Model](https://arxiv.org/abs/2606.16993v1)**  
  Authors: DreamX Team, Yancheng Bai, Rui Chen, Xiangxiang Chu, Rujing Dang, Hao Dou, Bingjie Gao, Qiwen Gu, Siyu Hong, Jiachen Lei, Geng Li, Jifan Li, Ruimin Lin, Qingfeng Shi, Bingze Song, Lei Sun, Jing Tang, Ruitian Tian, Jun Wang, Jiahong Wu, Pengfei Zhang, Shen Zhang, Jiashu Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16993v1.pdf)  
  Keywords: image-to-video, distillation, style, controllable, evaluation, camera control, world model, interactive, autoregressive, dit  
- **[Revealing Artifacts via Noise Amplification: A Novel Perspective for AI-Generated Video Detection](https://arxiv.org/abs/2606.16742v1)**  
  Authors: Renxi Cheng, Jie Gui, Hongsong Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16742v1.pdf)  
  Keywords: benchmark, text-to-video, video generation  
- **[Learned Image Compression for Vision-Language-Action Models](https://arxiv.org/abs/2606.16253v1)**  
  Authors: Hyeonjun Kim, Jegwang Ryu, Sangbeom Ha, Junhyeok Lee, Jun-Hyuk Kim, Hyemin Ahn, Jaeho Lee  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16253v1.pdf)  
  Keywords: benchmark, dit  
- **[Closed-Loop Triplet Synergistic Generation for Long-Form Video](https://arxiv.org/abs/2606.16184v1)**  
  Authors: Xinlei Yin, Xiulian Peng, Xiao Li, Zhiwei Xiong, Yan Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16184v1.pdf)  
  Keywords: benchmark, long-form, image-to-video, video generation, long video, identity, dit  
- **[Training-Free Open-Vocabulary Visual Grounding for Remote Sensing Images and Videos](https://arxiv.org/abs/2606.16124v1)**  
  Authors: Ke Li, Di Wang, Yongshan Zhu, Ting Wang, Weiping Ni, Tao Lei, Quan Wang, Xinbo Gao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16124v1.pdf)  
  Keywords: diffusion model, benchmark, efficient  
- **[Metis: A Generalizable and Efficient World-Action Model for Autonomous Driving and Urban Navigation](https://arxiv.org/abs/2606.15869v1)**  
  Authors: Jingyu Li, Zhe Liu, Dongnan Hu, Junjie Wu, Zipei Ma, Wenxiao Wu, Chao Han, Zhihui Hao, Zhikang Liu, Kun Zhan, Jiankang Deng, Xiatian Zhu, Li Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.15869v1.pdf)  
  Keywords: benchmark, video generation, architecture, efficient, autonomous driving  
- **[Track2View: 4D-Consistent Camera-Controlled Video Generation via Paired 3D Point Tracks](https://arxiv.org/abs/2606.15534v1)**  
  Authors: Feng Qiao, Zhaochong An, Zhexiao Xiong, Serge Belongie, Nathan Jacobs  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.15534v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://qjizhi.github.io/track2view)  
  Keywords: benchmark, diffusion transformer, video diffusion, trajectory, video generation, dynamics, dit  
- **[CausalDrive: Real-time Causal World Models for Autonomous Driving](https://arxiv.org/abs/2606.15341v1)**  
  Authors: Tianyi Yan, Huan Zheng, Dubing Chen, Meizhi Qu, Yingying Shen, Lijun Zhou, Mingfei Tu, Bing Wang, Guang Chen, Hangjun Ye, Haiyang Sun, Cheng-zhong Xu, Jianbing Shen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.15341v1.pdf)  
  Keywords: simulation, distillation, autonomous driving, trajectory, action-conditioned, controllable, layout, evaluation, world model, interactive, architecture, autoregressive, dit  
- **[NEXUS: Neural Energy Fields for Physically Consistent Contact-Rich 3D Object Dynamics](https://arxiv.org/abs/2606.15015v1)**  
  Authors: Qizhen Ying, Guangming Wang, Yangchen Pan, Victor Adrian Prisacariu, Yixiong Jing  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.15015v1.pdf)  
  Keywords: benchmark, trajectory, style, physics, controllable, acceleration, video generation, physical, dynamics, dit  

### Text-to-Video Generation

*Showing the latest 50 out of 56 papers*

- **[Revealing Artifacts via Noise Amplification: A Novel Perspective for AI-Generated Video Detection](https://arxiv.org/abs/2606.16742v1)**  
  Authors: Renxi Cheng, Jie Gui, Hongsong Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16742v1.pdf)  
  Keywords: benchmark, text-to-video, video generation  
- **[RGFVR: Reference-Guided Face Video Restoration with Flow Matching](https://arxiv.org/abs/2606.16401v1)**  
  Authors: Cem Eteke, Batuhan Tosun, Eckehard Steinbach  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16401v1.pdf) | [![GitHub](https://img.shields.io/github/stars/batuhanntosun/RG-FVR?style=social)](https://github.com/batuhanntosun/RG-FVR)  
  Keywords: flow matching, temporal consistency, identity, video restoration, text-to-video, dit  
- **[VideoWeave: Unlocking Geometric Consistency in Video Generation via Joint Geometry-Video Modeling](https://arxiv.org/abs/2606.14162v1)**  
  Authors: Xunzhi Xiang, Zixuan Duan, Yabo Chen, Zhengxuan Wei, Guiyu Zhang, Zixiao Gu, Zhe Gao, Haibin Huang, Chi Zhang, Qi Fan, Xuelong Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.14162v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://videoweave.github.io)  
  Keywords: image-to-video, video diffusion, video generation, denoising, diffusion model, text-to-video, dit  
- **[CineOrchestra: Unified Entity-Centric Conditioning for Cinematic Video Generation](https://arxiv.org/abs/2606.13768v1)**  
  Authors: Sharath Girish, Tsai-Shien Chen, Zhikang Dong, Mukesh Singhal, Hao Chen, Sergey Tulyakov, Aliaksandr Siarohin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13768v1.pdf)  
  Keywords: benchmark, personalization, video diffusion, video generation, camera control, diffusion model, text-to-video, dit  
- **[Flex4DHuman: Flexible Multi-view Video Diffusion for 4D Human Reconstruction](https://arxiv.org/abs/2606.13655v2)**  
  Authors: Jen-Hao Cheng, Yipeng Wang, Hao Zhang, Gengshan Yang, Jenq-Neng Hwang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13655v2.pdf)  
  Keywords: simulation, video diffusion, architecture, diffusion model, multi-view video, text-to-video, dit  
- **[SpecLoR: Spectral Lookahead Rectification for Motion-Coherent Text-to-Video Generation](https://arxiv.org/abs/2606.11969v1)**  
  Authors: Xu Zhang, Yu Lu, Ruijie Quan, Zhaozheng Chen, Bohan Wang, Yi Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.11969v1.pdf)  
  Keywords: benchmark, flow matching, video generation, physical, text-to-video, dit  
- **[Plan-and-Verify Video Reward Reasoning with Spatio-Temporal Scene Graph Grounding](https://arxiv.org/abs/2606.11838v1)**  
  Authors: Hyomin Kim, Junghye Kim, Joanie Hayoun Chung, Yoonjin Oh, Kyungjae Lee, Sungbin Lim, Sungwoong Kim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.11838v1.pdf)  
  Keywords: text-to-video, t2v, dit  
- **[HarmoView: Harmonizing Multi-View Constraints for Identity-Consistent Video Generation](https://arxiv.org/abs/2606.10839v1)**  
  Authors: Cong Wang, Zhentao Yu, Hongmei Wang, Weicong Liang, Zixiang Zhou, Zilin Yang, Jiarong Ou, Rui Chen, Yuan Zhou, Qinglin Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.10839v1.pdf)  
  Keywords: benchmark, t2v, evaluation, layout, video generation, identity, dit  
- **[Temporally Consistent and Controllable Video Generation of 2D Cine CMR via Latent Space Motion Modeling](https://arxiv.org/abs/2606.14759v1)**  
  Authors: Yiheng Cao, Gustavo Andrade-Miranda, Jiatian Zhang, Guillaume Sallé, Xin Gao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.14759v1.pdf)  
  Keywords: medical, controllable, video generation, diffusion model, text-to-video, dit  
- **[OmniGen-AR: AutoRegressive Any-to-Image Generation](https://arxiv.org/abs/2606.09156v1)**  
  Authors: Junke Wang, Xun Wang, Qiushan Guo, Peize Sun, Weilin Huang, Zuxuan Wu, Yu-Gang Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.09156v1.pdf)  
  Keywords: benchmark, video generation, architecture, text-to-video, autoregressive, dit  

### Video Editing

- **[ReGenHuman: Re-Generating Human Appearances for Realistic Full-Body Video Anonymization](https://arxiv.org/abs/2606.14972v1)**  
  Authors: Adam Sun, Eshaan Barkataki, Arnold Milstein, Gordon Wetzstein, Ehsan Adeli  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.14972v1.pdf)  
  Keywords: video-to-video, video diffusion, identity, dit  
- **[Lip Forcing: Few-Step Autoregressive Diffusion for Real-time Lip Synchronization](https://arxiv.org/abs/2606.11180v1)**  
  Authors: Paul Hyunbin Cho, Jinhyuk Jang, SeokYoung Lee, Joungbin Lee, Siyoon Jin, Heeseong Shin, Jung Yi, Yunjin Park, Chulmin Park, Seungryong Kim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.11180v1.pdf)  
  Keywords: video-to-video, video diffusion, trajectory, streaming, denoising, diffusion model, autoregressive, dit  
- **[CoVEBench: Can Video Editing Models Handle Complex Instructions?](https://arxiv.org/abs/2606.08415v2)**  
  Authors: Jiangtao Wu, Jiaming Wang, Yiwen He, Yuanxing Zhang, Shihao Li, Dunyuan Liu, Xuedong Zhao, Jialu Chen, Zekun Moore Wang, Jiaheng Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.08415v2.pdf)  
  Keywords: benchmark, style, video editing, dit  
- **[TIDE: Task-Isolated Diffusion for Unified Video Editing and Generation](https://arxiv.org/abs/2606.08260v1)**  
  Authors: Qi Liu, Gang Yue, Mingyu Yin, Lisai Zhang, Yidi Wu, Yaole Wang, Yaohui Wang, Chang Yao, Jingyuan Chen, Lin Ma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.08260v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://LittleWork123.github.io/tide)  
  Keywords: benchmark, diffusion transformer, video generation, video editing, dit  
- **[LoomVideo: Unifying Multimodal Inputs into Video Generation and Editing](https://arxiv.org/abs/2606.06042v2)**  
  Authors: Jianzong Wu, Hao Lian, Jiongfan Yang, Dachao Hao, Ye Tian, Yunhai Tong, Jingyuan Zhu, Biaolong Chen, Qiaosong Qi, Aixi Zhang, Wanggui He, Mushui Liu, Jinlong Liu, Pipei Huang, Hao Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.06042v2.pdf)  
  Keywords: benchmark, diffusion transformer, video generation, acceleration, architecture, video editing, efficient, dit  
- **[V2V-Bench: A Comprehensive Benchmark for Video-to-Video Generation Evaluation](https://arxiv.org/abs/2606.05665v1)**  
  Authors: Tao Liu, Leela Krishna, Gouti Pavan Kumar, Sreeja K, Vishav Garg  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.05665v1.pdf)  
  Keywords: benchmark, t2v, video-to-video, evaluation, video generation, i2v, dit  
- **[Bootstrap Your Generator: Unpaired Visual Editing with Flow Matching](https://arxiv.org/abs/2606.03911v1)**  
  Authors: Yoad Tewel, Yuval Atzmon, Gal Chechik, Lior Wolf  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.03911v1.pdf)  
  Keywords: flow matching, video editing, dit, evaluation  
- **[AlbedoEdit: Unified Instance-Level Video Editing with Albedo Guidance](https://arxiv.org/abs/2606.01362v1)**  
  Authors: Xilong Zhou, Bao-Huy Nguyen, Zheng Zeng, Jacob Munkberg, Jon Hasselgren, Thomas Leimkühler, Nima Kalantari, Miloš Hašan, Christian Theobalt  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.01362v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://vcai.mpi-inf.mpg.de/projects/AlbedoEdit)  
  Keywords: video editing, creative, dit  
- **[DeltaCam: Differential Intrinsic Camera Modeling for Video Generation](https://arxiv.org/abs/2605.25266v1)**  
  Authors: Debabrata Mandal, Zhihan Peng, Yujie Wang, Praneeth Chakravarthula  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25266v1.pdf)  
  Keywords: video-to-video, video diffusion, style, controllable, video generation, video style transfer, dynamics, dit  
- **[Geo-Align: Video Generation Alignment via Metric Geometry Reward](https://arxiv.org/abs/2605.23903v1)**  
  Authors: Zizun Li, Haoyu Guo, Runzhe Teng, Chunhua Shen, Tong He  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.23903v1.pdf)  
  Keywords: video-to-video, video generation, camera control, physical, dit  

### Video Inpainting & Completion

- **[R2RDreamer: 3D-aware Data Augmentation for Spatially-generalized 2D Manipulation Policies](https://arxiv.org/abs/2606.17040v1)**  
  Authors: Xiuwei Xu, Haowen Sun, Angyuan Ma, Yiwei Zhang, Zhenyu Wu, Xiaofeng Wang, Bingyao Yu, Zheng Zhu, Jie Zhou, Jiwen Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17040v1.pdf)  
  Keywords: image-to-video, simulation, style, controllable, 3d-aware, video completion, dit  
- **[PointAction: 3D Points as Universal Action Representations for Robot Control](https://arxiv.org/abs/2606.03943v1)**  
  Authors: Mutian Tong, Han Jiang, Qiao Feng, Lingjie Liu, Jiatao Gu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.03943v1.pdf)  
  Keywords: simulation, video prediction, video diffusion, 4d generation, video generation, diffusion model, dynamics  
- **[World Models: A Comprehensive Survey of Architectures, Methodologies, Reasoning Paradigms, and Applications](https://arxiv.org/abs/2606.00133v1)**  
  Authors: Arif Hassan Zidan, Yi Pan, Hanqi Jiang, Ruiyu Yan, Wei Ruan, Zihao Wu, Lifeng Chen, Weihang You, Xinliang Li, Bowen Chen, Huawen Hu, Peilong Wang, Sizhuang Liu, Jing Zhang, Siyuan Li, Zhengliang Liu, Yu Bao, Lin Zhao, Lichao Sun, Dajiang Zhu, Xiang Li, Jinglei Lv, Quanzheng Li, Wei Liu, Tianming Liu, Wei Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.00133v1.pdf)  
  Keywords: survey, benchmark, medical, video prediction, physics, evaluation, video generation, world model, interactive, architecture, robotics, education, dynamics, autonomous driving  
- **[Full-4D: Generating Full-Scope 4D Scenes from a Single-View Video](https://arxiv.org/abs/2605.25500v1)**  
  Authors: Tingxi Chen, Ke Hao, Yabo Chen, Zhengxue Cheng, Rong Xie, Li Song, Haibin Huang, Chi Zhang, Xuelong Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25500v1.pdf)  
  Keywords: flow matching, video interpolation, video synthesis, distillation, video diffusion, 4d generation, interactive, physical, diffusion model, multi-view video, dit  
- **[CRONOS: Benchmarking Counterfactual Physical Consistency in Video Models](https://arxiv.org/abs/2605.23699v1)**  
  Authors: León Begiristain, Olaf Dünkel, Adam Kortylewski  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.23699v1.pdf)  
  Keywords: benchmark, video prediction, world model, evaluation, physical, dynamics, dit  
- **[GEM-4D: Geometry-Enhanced Video World Models for Robot Manipulation](https://arxiv.org/abs/2605.22882v3)**  
  Authors: Kaichen Zhou, Yuzhen Chen, Fangneng Zhan, Hang Hua, Grace Chen, Xinhai Chang, Ao Qu, Yilun Du, Zhuang Liu, Paul Pu Liang, Mengyu Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.22882v3.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://gem-4d.github.io)  
  Keywords: simulation, video prediction, world model, architecture, physical, dynamics, dit  
- **[Goodbye Drift: Anchored Tree Sampling for Long-Horizon Video-to-Video Generation](https://arxiv.org/abs/2605.20476v1)**  
  Authors: Matthew Bendel, Stephen W. Bailey, Mithilesh Vaidya, Sumukh Badam, Xingzhe He  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20476v1.pdf)  
  Keywords: outpainting, t2v, distillation, video-to-video, style, video generation, autoregressive, dit  
- **[Nano World Models: A Minimalist Implementation of Future Video Prediction](https://arxiv.org/abs/2605.23993v2)**  
  Authors: Siqiao Huang, Partha Kaushik, Michael Chen, Hengkai Pan, Kaiwen Geng, Omar Chehab, Fernando Moreno-Pino, Max Simchowitz  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.23993v2.pdf)  
  Keywords: simulation, video prediction, world model, evaluation, video generation, interactive, architecture, autoregressive, dit  
- **[Relit-LiVE: Relight Video by Jointly Learning Environment Video](https://arxiv.org/abs/2605.06658v1)**  
  Authors: Weiqing Xiao, Hong Li, Xiuyu Yang, Houyuan Chen, Wenyi Li, Tianqi Liu, Shaocong Xu, Chongjie Ye, Hao Zhao, Beibei Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.06658v1.pdf) | [![GitHub](https://img.shields.io/github/stars/zhuxing0/Relit-LiVE?style=social)](https://github.com/zhuxing0/Relit-LiVE)  
  Keywords: benchmark, video prediction, video diffusion, streaming, physical, diffusion model, dit  
- **[Quaternion Nonlinear Transform-Induced Nuclear Norm for Low-Rank Tensor Completion](https://arxiv.org/abs/2605.01467v1)**  
  Authors: Biswarup Karmakar, Ratikanta Behera  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.01467v1.pdf)  
  Keywords: benchmark, video inpainting, efficient  

### Video Super-Resolution & Enhancement

*Showing the latest 50 out of 75 papers*

- **[RGFVR: Reference-Guided Face Video Restoration with Flow Matching](https://arxiv.org/abs/2606.16401v1)**  
  Authors: Cem Eteke, Batuhan Tosun, Eckehard Steinbach  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16401v1.pdf) | [![GitHub](https://img.shields.io/github/stars/batuhanntosun/RG-FVR?style=social)](https://github.com/batuhanntosun/RG-FVR)  
  Keywords: flow matching, temporal consistency, identity, video restoration, text-to-video, dit  
- **[VideoWeave: Unlocking Geometric Consistency in Video Generation via Joint Geometry-Video Modeling](https://arxiv.org/abs/2606.14162v1)**  
  Authors: Xunzhi Xiang, Zixuan Duan, Yabo Chen, Zhengxuan Wei, Guiyu Zhang, Zixiao Gu, Zhe Gao, Haibin Huang, Chi Zhang, Qi Fan, Xuelong Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.14162v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://videoweave.github.io)  
  Keywords: image-to-video, video diffusion, video generation, denoising, diffusion model, text-to-video, dit  
- **[Avatar V: Scaling Video-Reference Avatar Video Generation](https://arxiv.org/abs/2606.13872v1)**  
  Authors: Benjamin Liang, Ce Chen, Desmond Lin, Ivan Somov, Jiajun Zhao, Jiewei Yuan, Jingfeng Zhang, Junhao Huang, Nik Nolte, Pedram Haqiqi, Penghan Wang, Rong Yan, Rui Zhang, Sam Prokopchuk, Sivan Wang, Viktor Goriachko, Yi Ren, Yuanming Li, Yutao Chen, Zhenhui Ye, Zhibin Hong, Zilong Nie, Zujin Guo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13872v1.pdf)  
  Keywords: benchmark, flow matching, distillation, super-resolution, style, avatar, evaluation, video generation, acceleration, identity, dynamics, dit  
- **[Temporal Backtracking Search for Test-time Generative Video Reasoning](https://arxiv.org/abs/2606.13861v1)**  
  Authors: Sejoon Jun, Zheng Ding, Huangyuan Su, Weirui Ye, Yilun Du  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13861v1.pdf)  
  Keywords: video generation, robotics, denoising, efficient, dit  
- **[World Tracing: Generative Pixel-Aligned Geometry Beyond the Visible](https://arxiv.org/abs/2606.13652v1)**  
  Authors: Hao Zhang, Mohamed El Banani, Jen-Hao Cheng, Paul Zhang, Yi Hua, Ben Mildenhall, Christoph Lassner, Narendra Ahuja, Gengshan Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13652v1.pdf)  
  Keywords: benchmark, flow matching, diffusion transformer, video synthesis, denoising, dit  
- **[Next Forcing: Causal World Modeling with Multi-Chunk Prediction](https://arxiv.org/abs/2606.11187v1)**  
  Authors: Gangwei Xu, Qihang Zhang, Jiaming Zhou, Xing Zhu, Yujun Shen, Xin Yang, Yinghao Xu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.11187v1.pdf)  
  Keywords: benchmark, world model, video generation, acceleration, physical, denoising, dynamics, autoregressive  
- **[Lip Forcing: Few-Step Autoregressive Diffusion for Real-time Lip Synchronization](https://arxiv.org/abs/2606.11180v1)**  
  Authors: Paul Hyunbin Cho, Jinhyuk Jang, SeokYoung Lee, Joungbin Lee, Siyoon Jin, Heeseong Shin, Jung Yi, Yunjin Park, Chulmin Park, Seungryong Kim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.11180v1.pdf)  
  Keywords: video-to-video, video diffusion, trajectory, streaming, denoising, diffusion model, autoregressive, dit  
- **[Flow-DPPO: Divergence Proximal Policy Optimization for Flow Matching Models](https://arxiv.org/abs/2606.11025v1)**  
  Authors: Bowen Ping, Xiangxin Zhou, Penghui Qi, Minnan Luo, Liefeng Bo, Tianyu Pang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.11025v1.pdf) | [![GitHub](https://img.shields.io/github/stars/Tencent-Hunyuan/UniRL?style=social)](https://github.com/Tencent-Hunyuan/UniRL)  
  Keywords: flow matching, trajectory, style, video generation, denoising  
- **[LiteVSR: Lightweight Adaptation of Frozen Diffusion Transformers for Video Super-Resolution](https://arxiv.org/abs/2606.09250v1)**  
  Authors: Yu Cao, Ziquan Liu, Zhensong Zhang, Jiankang Deng, Shaogang Gong, Jifei Song  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.09250v1.pdf)  
  Keywords: flow matching, diffusion transformer, super-resolution, style, architecture, denoising  
- **[Ultra Flash: Scaling Real-Time Streaming Video Generation to High Resolutions](https://arxiv.org/abs/2606.09150v2)**  
  Authors: Luxury, Jie Huang, Zihao Fan, Xiaoxiao Ma, Jun-hao Zhuang, Yuming Li, Zeyue Xue, Siming Fu, Haoran Li, Mingchen Zhong, Guohui Zhang, Shichen Ma, Yijun Liu, Jiaqi Shi, Yanwen Ma, Yaofeng Su, Haoyu Wang, Yaowei Li, Songchun Zhang, Weiyang Jin, Yuxuan Bian, Shiyi Zhang, Haojun Xu, Shuai Lu, Xin Han, Wei Tang, Haoyang Huang, Nan Duan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.09150v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://xin1u.github.io/UltraFlash)  
  Keywords: t2v, distillation, super-resolution, video diffusion, video generation, streaming, architecture, diffusion model, autoregressive, efficient  

### World Models & Simulation

*Showing the latest 50 out of 123 papers*

- **[R2RDreamer: 3D-aware Data Augmentation for Spatially-generalized 2D Manipulation Policies](https://arxiv.org/abs/2606.17040v1)**  
  Authors: Xiuwei Xu, Haowen Sun, Angyuan Ma, Yiwei Zhang, Zhenyu Wu, Xiaofeng Wang, Bingyao Yu, Zheng Zhu, Jie Zhou, Jiwen Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17040v1.pdf)  
  Keywords: image-to-video, simulation, style, controllable, 3d-aware, video completion, dit  
- **[Qwen-RobotWorld Technical Report: Unifying Embodied World Modeling through Language-Conditioned Video Generation](https://arxiv.org/abs/2606.17030v1)**  
  Authors: Jie Zhang, Xiaoyue Chen, Anzhe Chen, Chenxu Lv, Deqing Li, Gengze Zhou, Hang Yin, Haoqi Yuan, Haoyang Li, Jiahao Li, Jiazhao Zhang, Jingren Zhou, Kaiyuan Gao, Kun Yan, Lihan Jiang, Ningyuan Tang, Pei Lin, Qihang Peng, Shengming Yin, Tianhe Wu, Tianyi Yan, Xiao Xu, Yan Shu, Yanran Zhang, Ye Wang, Yi Wang, Yilei Chen, Yixian Xu, Yiyang Huang, Yuxiang Chen, Zekai Zhang, Zhendong Wang, Zhixing Lei, Zhixuan Liang, Zihao Liu, Zikai Zhou, Xiong-Hui Chen, Chenfei Wu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17030v1.pdf)  
  Keywords: benchmark, diffusion transformer, autonomous driving, world model, evaluation, video generation, physical, dit  
- **[DreamX-World 1.0: A General-Purpose Interactive World Model](https://arxiv.org/abs/2606.16993v1)**  
  Authors: DreamX Team, Yancheng Bai, Rui Chen, Xiangxiang Chu, Rujing Dang, Hao Dou, Bingjie Gao, Qiwen Gu, Siyu Hong, Jiachen Lei, Geng Li, Jifan Li, Ruimin Lin, Qingfeng Shi, Bingze Song, Lei Sun, Jing Tang, Ruitian Tian, Jun Wang, Jiahong Wu, Pengfei Zhang, Shen Zhang, Jiashu Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16993v1.pdf)  
  Keywords: image-to-video, distillation, style, controllable, evaluation, camera control, world model, interactive, autoregressive, dit  
- **[RealityBridge: Bridging Editable 3D Gaussian Splatting Driving Simulations and Real-World Videos](https://arxiv.org/abs/2606.16278v1)**  
  Authors: Zhenhua Wu, Yun Pang, Mingkun Chang, Yuwei Ning, Liangzhi Wang, Yi Xiao, Guanbin Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16278v1.pdf)  
  Keywords: simulation, autonomous driving, controllable, video generation, temporal consistency, autoregressive, dit  
- **[LaWAM: Latent World Action Models for Efficient Dynamics-Aware Robot Policies](https://arxiv.org/abs/2606.15768v1)**  
  Authors: Jialei Chen, Kai Wang, Kang Chen, Shuaihang Chen, Feng Gao, Wenhao Tang, Zhiyuan Li, Weilin Liu, Zhuyu Yao, Boxun Li, Yuanbo Xu, Chao Yu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.15768v1.pdf)  
  Keywords: action-conditioned, world model, video generation, dynamics, efficient, dit  
- **[CausalDrive: Real-time Causal World Models for Autonomous Driving](https://arxiv.org/abs/2606.15341v1)**  
  Authors: Tianyi Yan, Huan Zheng, Dubing Chen, Meizhi Qu, Yingying Shen, Lijun Zhou, Mingfei Tu, Bing Wang, Guang Chen, Hangjun Ye, Haiyang Sun, Cheng-zhong Xu, Jianbing Shen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.15341v1.pdf)  
  Keywords: simulation, distillation, autonomous driving, trajectory, action-conditioned, controllable, layout, evaluation, world model, interactive, architecture, autoregressive, dit  
- **[GeoStream: Toward Precise Camera Controlled Streaming Video Generation](https://arxiv.org/abs/2606.15162v1)**  
  Authors: Yizhou Zhao, Yifan Wang, Xiaoyuan Wang, Yushu Wu, Hao Zhang, Moayed Haji-Ali, Rameen Abdal, Ashkan Mirzaei, Yanyu Li, Willi Menapace, Laszlo Jeni, Sergey Tulyakov, Peter Wonka, Chaoyang Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.15162v1.pdf)  
  Keywords: distillation, world model, streaming, camera control, video generation, interactive, autoregressive, dit  
- **[Prompt2Effect: Training-Free Image-to-Video Model Specialization via LoRA Generation](https://arxiv.org/abs/2606.13971v1)**  
  Authors: Xiaomeng Yang, Yanyu Li, Gordon Guocheng Qian, Ivan Skorokhodov, Viacheslav Ivanov, Avalon Vinella, Xuan Zhang, Yanzhi Wang, Sergey Tulyakov, Anil Kag  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13971v1.pdf)  
  Keywords: image-to-video, video generation, i2v, interactive, diffusion model, dit  
- **[RepWAM: World Action Modeling with Representation Visual-Action Tokenizers](https://arxiv.org/abs/2606.13674v2)**  
  Authors: Junke Wang, Qihang Zhang, Shuai Yang, Yiming Luo, Yujun Shen, Zuxuan Wu, Yu-Gang Jiang, Yinghao Xu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13674v2.pdf) | [![GitHub](https://img.shields.io/github/stars/wdrink/RepWAM?style=social)](https://github.com/wdrink/RepWAM)  
  Keywords: benchmark, dynamics, simulation, video generation  
- **[Flex4DHuman: Flexible Multi-view Video Diffusion for 4D Human Reconstruction](https://arxiv.org/abs/2606.13655v2)**  
  Authors: Jen-Hao Cheng, Yipeng Wang, Hao Zhang, Gengshan Yang, Jenq-Neng Hwang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13655v2.pdf)  
  Keywords: simulation, video diffusion, architecture, diffusion model, multi-view video, text-to-video, dit  



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
