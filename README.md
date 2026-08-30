# Awesome Video Diffusions [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of latest research papers, projects and resources related to Video Diffusion Models and Video Generation. Content is automatically updated daily.

> Last Update: 2026-08-30 03:42:32

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

- [3D-aware Video Generation](#3d-aware-video-generation) (11 papers) - Video generation with 3D awareness, multi-view consistency, and 4D content creation
- [Applications](#applications) (44 papers) - Domain-specific applications of video diffusion models
- [Architecture & Efficiency](#architecture-&-efficiency) (355 papers) - Architectural innovations (DiT, UNet), flow matching, and training/inference efficiency
- [Audio & Multi-modal](#audio-&-multi-modal) (22 papers) - Audio-driven and multi-modal conditioned video generation
- [Controllable Generation](#controllable-generation) (124 papers) - Controllable video generation with motion, camera, pose, or layout guidance
- [Human & Character Animation](#human-&-character-animation) (30 papers) - Human-centric video generation including talking heads, dance, and character animation
- [Image-to-Video Generation](#image-to-video-generation) (51 papers) - Methods for animating still images into videos
- [Long Video Generation](#long-video-generation) (120 papers) - Generating temporally consistent long-form videos beyond short clips
- [Personalization & Customization](#personalization-&-customization) (89 papers) - Personalized video generation with custom subjects, identities, or styles
- [Physical Understanding](#physical-understanding) (143 papers) - Physics-aware video generation and dynamics modeling
- [Surveys & Benchmarks](#surveys-&-benchmarks) (229 papers) - Survey papers, benchmarks, and evaluation metrics for video generation
- [Text-to-Video Generation](#text-to-video-generation) (74 papers) - Foundation models and methods for generating videos from text prompts
- [Video Editing](#video-editing) (20 papers) - Diffusion-based video editing, style transfer, and manipulation
- [Video Inpainting & Completion](#video-inpainting-&-completion) (9 papers) - Video inpainting, completion, outpainting, and temporal prediction
- [Video Super-Resolution & Enhancement](#video-super-resolution-&-enhancement) (79 papers) - Video quality improvement, upscaling, restoration, and frame interpolation
- [World Models & Simulation](#world-models-&-simulation) (120 papers) - Video generation as world simulators and interactive environment generation



## Table of Contents

- [Categorized Papers](#categorized-papers)
- [Classic Papers](#classic-papers)
- [Open Source Projects](#open-source-projects)
- [Applications](#applications)
- [Tutorials & Blogs](#tutorials--blogs)





## Categorized Papers

### 3D-aware Video Generation

- **[GaussVid: Sparse-View Gaussian Splatting with 3D-Aware Video Diffusion Priors](https://arxiv.org/abs/2608.21849v1)**  
  Authors: Xinhui Liu, Can Wang, Wei Jiang, Wei Wang, Dong Xu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.21849v1.pdf)  
  Keywords: video restoration, 3d-aware, dit, diffusion model, video diffusion, video generation, novel view  
- **[Grounded-Exo2Ego: Structured Semantic Grounding for Robust Exocentric-to-Egocentric Video Generation](https://arxiv.org/abs/2608.20534v1)**  
  Authors: Shengze Wang, Michael Stengel, Tianye Li, Seonwook Park, Amrita Mazumdar, Koki Nagano, Alex Trevithick, Shalini De Mello  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.20534v1.pdf)  
  Keywords: evaluation, dit, physical, diffusion model, video diffusion, video generation, novel view  
- **[Beyond Pixels: From Video Priors to 4D Worlds](https://arxiv.org/abs/2608.10744v1)**  
  Authors: Zihao Liu, Xiaolong Shen, Zhenglin Zhou, Ruijie Quan, Yi Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.10744v1.pdf)  
  Keywords: 4d generation, video diffusion, dit, diffusion transformer  
- **[UniWorld-View: Large-Baseline View Synthesis via Video Diffusion Models](https://arxiv.org/abs/2608.04701v1)**  
  Authors: Haiyang Zhou, Wangbo Yu, Chaoran Feng, Xunyu Zhou, Yonghong Tian, Li Yuan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.04701v1.pdf)  
  Keywords: camera control, multi-view video, diffusion model, benchmark, video diffusion, novel view, controllable  
- **[AniGS: Bridging Rendering and Diffusion Prior for 3D Scene Animation](https://arxiv.org/abs/2607.18539v1)**  
  Authors: Yen-Chi Cheng, Chen Gao, Chuhan Chen, Tuotuo Li, Rajvi Shah, Ayush Saraf, Changil Kim, Liangyan Gui, Alexander Schwing, Johannes Kopf, Hung-Yu Tseng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.18539v1.pdf)  
  Keywords: dit, diffusion model, video diffusion, novel view, video-to-video, dynamics  
- **[Delving into the Temporal Challenges of Unified Video Protection Against Image-to-Video and Fine-Tuning-based Customization](https://arxiv.org/abs/2607.13336v1)**  
  Authors: Yuxin Huang, Ziming Hong, Mingming Gong, Wanyu Wang, Jing Zhang, Tongliang Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.13336v1.pdf)  
  Keywords: dit, diffusion model, 3d video, identity, image-to-video, video diffusion, video generation, customization  
- **[4D Human-Scene Reconstruction from Low-Overlap Captures](https://arxiv.org/abs/2607.09125v1)**  
  Authors: Minhyuk Hwang, Sangmin Kim, Seunguk Do, Daneul Kim, Jaesik Park  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.09125v1.pdf)  
  Keywords: diffusion model, identity, video diffusion, novel view, trajectory  
- **[SoccerNet 2026 Challenges Results](https://arxiv.org/abs/2607.07320v1)**  
  Authors: Anthony Cioppa, Silvio Giancola, Håkan Ardö, Mohamad Dalal, Jan Held, Jérémie Ochin, Jiayuan Rao, Karen Sanchez, Renaud Vandeghen, Artur Xarles, Olivier Barnich, Albert Clapés, Mathieu Delvaux, Sergio Escalera, Bernard Ghanem, Cédric Hons, Antoine Houet, Sotiris Manitsaris, Tom Michel, Pierre Miralles, Thomas B. Moeslund, Mikael Nilsson, Bogdan Stanciulescu, Marc Van Droogenbroeck, Yanfeng Wang, Weidi Xie, Faisal Altawijri, Mohamed Atef, Semen Budennyy, Vasiliy Chelpanov, Puhua Chen, Yixin Chen, Lechao Cheng, Jianling Chu, Ju-Seong Do, Oleg Durygin, Omar Fetouh, Mirco Fuchs, Youssef Ghallab, Falguni Ghosh, Wonjun Heo, Yufeng Hu, Weixuan Huang, Phuong-Linh Huynh-Ha, Matvey Isupov, Yangguang Ji, Siyuan Jiang, Zhenxiang Jiang, Wonyong Jo, Ho-Young Jung, SeongHeon Kang, MinJae Kim, Youngseon Kim, Jakub Komosa, Artem Konshin, Trung-Hoang Le, Jongmin Lee, Lingling Li, Litao Li, Vadim Linkov, Fang Liu, Haoxuan Ma, Shun Makino, Ismail Mathkour, Konstantin Mitin, Mikhail Moiseev, Takumi Nagaya, Yuki Nakamura, Thanh-Khoi Nguyen, Hoang-Phuc Nguyen, Trong-Thuan Nguyen, Christian Orduz, Kwanyong Park, Fabian Perez, Parthsarthi Rawat, SuHyun Rim, Hoover Rueda-Chacón, Atom Scott, Minori Sugimura, Yuyang Sun, Shengeng Tang, Minh-Triet Tran, Ikuma Uchida, Juan Vanegas, Thanh-Nhan Vo, Jiangtao Wang, Yaxiong Wang, Xiaogang Wang, Ruifeng Wang, Rio Watanabe, Jiali Wen, Yongliang Wu, Di Yang, Xu Yang, Zhuo Yang, Xinyu Ye, Yibo Yu, Zihan Zhai, Yu Zhang, Zhenyu Zhao, Zhun Zhong, Yixi Zhou, Xingyu Zhu, Wenbo Zhu, Julian Ziegler  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.07320v1.pdf)  
  Keywords: evaluation, dit, benchmark, novel view  
- **[MV-Forcing: Long Multi-View Video Generation via 4D-Grounded Spatio-Temporal Self-Forcing](https://arxiv.org/abs/2607.05376v1)**  
  Authors: Gal Fiebelman, Hadar Averbuch-Elor, Sagie Benaim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.05376v1.pdf)  
  Keywords: autoregressive, multi-view video, diffusion model, denoising, video diffusion, video generation, distillation  
- **[NeoMap: Training-free Novel-View Synthesis from Single Images and Videos](https://arxiv.org/abs/2607.01962v1)**  
  Authors: Jinxi Li, Tianyi Zhang, Yafei Yang, Zihui Zhang, Peng Huang, Koon Wing Macgyver Lin, Bo Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.01962v1.pdf)  
  Keywords: dit, benchmark, denoising, novel view, video synthesis  

### Applications

- **[SpatialCrafter: Single Image World Modeling with Generative 3D Proxies](https://arxiv.org/abs/2608.27073v1)**  
  Authors: Chuan Fang, Lingteng Qiu, Yixun Liang, Rui Chen, Kunming Luo, Zhaohua Zheng, Tongyuan Bai, Feipeng Tian, Zilong Dong, Zihan Zhou, Ping Tan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.27073v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://fangchuan.github.io/SpatialCrafter)  
  Keywords: dit, diffusion model, video diffusion, robotics, world model  
- **[GeoWAM: Visual Geometry World Action Models for Autonomous Driving](https://arxiv.org/abs/2608.23486v2)**  
  Authors: Yiren Lu, Xin Ye, Jiaming Liu, Philip Jacobson, Jin Yao, Yi-chung Chen, Liam Merino, Dhruva Dixith Kurra, Min Cai, Tom Lampo, Yu Yin, Danhua Guo, Burhan Yaman  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.23486v2.pdf)  
  Keywords: evaluation, dit, autonomous driving, world model, trajectory, dynamics  
- **[SPVC: Structured and Panoptic Video Fixing for Cross-Dataset Driving Scene Rendering](https://arxiv.org/abs/2608.17420v1)**  
  Authors: Gen Li, Shu Han, Yun Xi Qiao, Hua Chen, Xuyang Dai, Bohan Li, Hao Zhao, Chaojian Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.17420v1.pdf)  
  Keywords: dit, layout, diffusion model, autonomous driving, video diffusion, controllable, simulation  
- **[EditStream: A Unified Autoregressive Framework for Interactive Video Generation and Editing](https://arxiv.org/abs/2608.21424v1)**  
  Authors: Yuqian Zhou, Zhenghong Zhou, Zongze Wu, Cameron Smith, Richard Zhang, Jiebo Luo, Eli Shechtman, Zhe Lin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.21424v1.pdf)  
  Keywords: autoregressive, dit, efficient, interactive, image-to-video, video generation, video-to-video, creative, text-to-video, video editing, streaming, distillation  
- **[CrossView: Can Vision-Language Models Reason Across Cameras?](https://arxiv.org/abs/2608.15539v1)**  
  Authors: Sahil Shah, S P Sharan, Harsh Goel, Manvik Pasula, Adithya Hebbalae, Minkyu Choi, Sandeep P. Chinchali  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.15539v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://utaustin-swarmlab.github.io/CrossView)  
  Keywords: evaluation, multi-modal, benchmark, autonomous driving, robotics  
- **[A survey of AI-generated voices and their detection](https://arxiv.org/abs/2608.15411v1)**  
  Authors: Chengzhe Sun, Tianle Yang, Siwei Lyu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.15411v1.pdf)  
  Keywords: creative, dit, survey, benchmark  
- **[StateFlow: Building, Evolving, and Accessing 3D World States for Previsualization](https://arxiv.org/abs/2608.12314v1)**  
  Authors: Yuyang Yin, Zixiang Li, Longxuan Deng, Hongkai Li, Shifang Zhao, Junnan Liu, Weirong Huang, Mengyu Wang, Tianxiao Fu, Yikai Wang, Peng-Shuai Wang, Xiaojie Jin, Yao Zhao, Yunchao Wei  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.12314v1.pdf)  
  Keywords: dit, film, video synthesis, dynamics, architecture  
- **[Multi-View Relational Distillation for Spatial Reasoning with Vision-Language Models](https://arxiv.org/abs/2608.10864v1)**  
  Authors: Kiet T. Nguyen, Hanbo Shim, Jinwoo Kim, Seunghoon Hong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.10864v1.pdf)  
  Keywords: autonomous driving, robotics, distillation  
- **[GeoRoute: Geometry-Aware Hybrid Inference for Traffic Future-Frame Prediction](https://arxiv.org/abs/2608.09493v1)**  
  Authors: Khang Minh Le, Hieu Dinh Trung Pham, Luu Thanh Danh, Nam-Tien Le, Hieu Anh Ngo, Phuong Huu Vu Tran, Son Nguyen Minh Le, Nguyen Trong Nghia, Tu Tran Thi Cam, Huy Minh Nhat Nguyen, Cuong Tuan Nguyen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.09493v1.pdf)  
  Keywords: dit, diffusion model, benchmark, latent video, video prediction, autonomous driving, video diffusion, architecture  
- **[Findings of the First Teaching Monster Challenge: A Benchmark of Pedagogical Content Knowledge in AI Agents](https://arxiv.org/abs/2608.08852v1)**  
  Authors: Yi-Cheng Lin, Yu-Kai Guo, Szu-Chi Chen, Bo-Han Feng, Yun-Man Hsu, Hsiang Hsieh, Yu-Jung Lin, Yue-Ling Wu, Jia-Kai Dong, An-Yu Cheng, Yu-Han Huang, Lok-Lam Ieong, Kuan-Yu Chen, Ming-Douo Tchouang, Shao-Hua Sun, Che Lin, Jian-Jiun Ding, Hung-yi Lee  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.08852v1.pdf)  
  Keywords: evaluation, dit, long-form, benchmark, video generation, education  

### Architecture & Efficiency

*Showing the latest 50 out of 355 papers*

- **[CLAP: Cross-Embodiment Video World Models are Zero-Shot Physical Simulators](https://arxiv.org/abs/2608.27406v1)**  
  Authors: Kechen Liu, Ola Shorinwa  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.27406v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://omni-clap.github.io)  
  Keywords: dit, physical, video generation, physics, world model, action-conditioned, dynamics  
- **[SpatialCrafter: Single Image World Modeling with Generative 3D Proxies](https://arxiv.org/abs/2608.27073v1)**  
  Authors: Chuan Fang, Lingteng Qiu, Yixun Liang, Rui Chen, Kunming Luo, Zhaohua Zheng, Tongyuan Bai, Feipeng Tian, Zilong Dong, Zihan Zhou, Ping Tan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.27073v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://fangchuan.github.io/SpatialCrafter)  
  Keywords: dit, diffusion model, video diffusion, robotics, world model  
- **[TempJail: Temporal Jailbreak Attacks against Image-to-Video Generation Models](https://arxiv.org/abs/2608.26971v1)**  
  Authors: Qi Lu, Zehui Guo, David Yuanda Gan, Zijing Li, Hengda Zhang, Weijun Xu, Qiankun Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.26971v1.pdf) | [![GitHub](https://img.shields.io/github/stars/luqi-glory/TempJail?style=social)](https://github.com/luqi-glory/TempJail)  
  Keywords: evaluation, dit, image-to-video, video generation, video synthesis, i2v  
- **[Tether the Subject, Release the Scene: Query-Aware Memory Routing for Long-Horizon Autoregressive Video Generation](https://arxiv.org/abs/2608.26902v1)**  
  Authors: Chen Li, Peng Zhang, Hanyu Zhou, Jialong Zuo, Fei Wang, Daiguo Zhou, Nong Sang, Changxin Gao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.26902v1.pdf)  
  Keywords: autoregressive, dit, long video, identity, video generation, streaming  
- **[RECAP-Forcing: Retaining Content Appearances for Long Video Generation](https://arxiv.org/abs/2608.26671v1)**  
  Authors: Haiyang Xu, Zheng Ding, Zhuowen Tu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.26671v1.pdf)  
  Keywords: autoregressive, long video, dit, video generation  
- **[Activation Outliers Matter: Robust Recovery for Quantized Multimodal LLMs](https://arxiv.org/abs/2608.26581v1)**  
  Authors: Tanzila Rahman, Mehran Taghian Jazi, Yunke Peng, Zhuang Ma, Anandharaju Durai Raju, Yao Wang, Xing Huang, Hei Yi Mak, Shadan Golestan, Hoang Le, Yonghan Dong, Wei Guo, Yaoyuan Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.26581v1.pdf)  
  Keywords: efficient, benchmark, video generation  
- **[Multi2AV-Safety: Benchmarking Safety in Multimodal-to-Audio-Video Generation](https://arxiv.org/abs/2608.26535v1)**  
  Authors: Kaichao Jiang, Changtao Miao, Baiqi Wu, Zhiyuan Lu, Kang Yang, Peiwei Zhao, Junchi Chen, Yunfeng Diao, He Liu, Qi Chu, Tao Gong, Nenghai Yu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.26535v1.pdf)  
  Keywords: evaluation, dit, benchmark, video generation  
- **[VBVR-Pro: A Scalable and Verifiable Suite for Native Visual Reasoning](https://arxiv.org/abs/2608.26105v1)**  
  Authors: Junxiang Xu, Ruisi Wang, Fanyi Pu, Maijunxian Wang, Ran Ji, Tongxi Zhou, Chenyang Gu, Jing Zuo, Hongcan Xiao, Yimeng Geng, Wanqi Yin, Wei Chen, Oscar Qian, Zhengan Yan, Ziqi Huang, Haiwen Diao, Liang Pan, Bo Li, Xiangyu Fan, Dezhi Luo, Fengyuan Yu, Zehong Zhao, Qingying Gao, Tinghui Zhu, Yilan Zhang, Jingqi Tong, Pinyuan Feng, Zhengze Jiang, Letian Wang, Ziyu Guo, Renrui Zhang, Jieneng Chen, Sonia Joseph, Constantin Venhoff, Saman Motamed, Mengyue Yang, Chandra Sripada, Alan Yuille, Philip Torr, Lvmin Zhang, Vikash Kumar, Daniel Khashabi, Nikolaus Kriegeskorte, Raphaël Millière, Vincent C. Müller, Anyi Rao, Quan Wang, Ziwei Liu, Dahua Lin, Lei Yang, Hokin Deng, Zhongang Cai  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.26105v1.pdf)  
  Keywords: evaluation, efficient, benchmark, video generation, controllable  
- **[Surgical Video Generation From Diffusion to World Models: A Survey](https://arxiv.org/abs/2608.26214v1)**  
  Authors: Fuxiang Huang, Chenxu Zhang, Liang Han, Lei Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.26214v1.pdf)  
  Keywords: multi-modal, dit, physical, survey, simulation, video generation, concept, world model, dynamics  
- **[4DStreamCtrl: Interactive Video Generation with Online 4D Control](https://arxiv.org/abs/2608.25479v2)**  
  Authors: Shiqian Li, Chenguo Lin, Zhiguang Liu, Yu Tang, Jiarong Ou, Rui Chen, Yixin Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.25479v2.pdf)  
  Keywords: dit, efficient, interactive, diffusion model, long video, denoising, video diffusion, video generation, controllable, world model, trajectory, streaming  

### Audio & Multi-modal

- **[Surgical Video Generation From Diffusion to World Models: A Survey](https://arxiv.org/abs/2608.26214v1)**  
  Authors: Fuxiang Huang, Chenxu Zhang, Liang Han, Lei Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.26214v1.pdf)  
  Keywords: multi-modal, dit, physical, survey, simulation, video generation, concept, world model, dynamics  
- **[WeMM-Embedding: WeChat Multi-Modal Embedding Technical Report](https://arxiv.org/abs/2608.24053v1)**  
  Authors: Junjie Zhou, Ke Mei, Lei Li, Tianyi Wang, Fengyun Rao, Jing Lyu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.24053v1.pdf) | [![GitHub](https://img.shields.io/github/stars/Tencent/WeMM-Embedding?style=social)](https://github.com/Tencent/WeMM-Embedding)  
  Keywords: evaluation, multi-modal, benchmark  
- **[SingDance: Compositional Zero-Shot Singing-and-Dancing Video Generation with Role-Aware Audio Conditioning](https://arxiv.org/abs/2608.16220v1)**  
  Authors: Tao Feng, Xu Li, Xiangyang Luo, Ming Wen, Huadai Liu, Chen Zhang, Wei Xue  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.16220v1.pdf)  
  Keywords: speech-driven, dit, video diffusion, body motion, video generation, controllable  
- **[AnyTalk: Speech Animation for Arbitrary Characters Leveraging a Video Generation Model](https://arxiv.org/abs/2608.16143v1)**  
  Authors: Kwan Yun, Serin Yoon, Sunjin Jung, Jung Eun Yoo, Inyup Lee, Junyong Noh  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.16143v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://serin-yoon.github.io/projects/anytalk)  
  Keywords: diffusion model, video diffusion, audio-driven, video generation  
- **[Adding Voice Cloning to Text-to-Audio-Video Models with a Single Zero-Initialised Layer](https://arxiv.org/abs/2608.15690v1)**  
  Authors: Ivan Mikheev, Viacheslav Vasilev, Anna Dmitrienko, Alexey Letunovskiy, Ivan Kirillov, Kirill Chernyshev, Denis Dimitrov  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.15690v1.pdf)  
  Keywords: dit, sound, benchmark, video diffusion, architecture  
- **[CrossView: Can Vision-Language Models Reason Across Cameras?](https://arxiv.org/abs/2608.15539v1)**  
  Authors: Sahil Shah, S P Sharan, Harsh Goel, Manvik Pasula, Adithya Hebbalae, Minkyu Choi, Sandeep P. Chinchali  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.15539v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://utaustin-swarmlab.github.io/CrossView)  
  Keywords: evaluation, multi-modal, benchmark, autonomous driving, robotics  
- **[Efficient Audio-Visual Generation via Synchrony-Aware Cross-Modal Sparse Attention](https://arxiv.org/abs/2608.15522v1)**  
  Authors: Shengchuan Gao, Teng Hu, Bohao Feng, Luchen Li, Wenqiang Wang, Hongqian Deng, Ran Yi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.15522v1.pdf)  
  Keywords: efficient, sound, long video, denoising, video generation, acceleration  
- **[Avatar-Forever: Decoupled Parallel Training for High-Quality Real-Time Infinite Avatars](https://arxiv.org/abs/2608.12107v1)**  
  Authors: Ruibin Li, Tao Yang, Zhiyuan Ma, Fangzhou Ai, Shilei Wen, Lei Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.12107v1.pdf)  
  Keywords: autoregressive, dit, efficient, interactive, identity, avatar, video generation, audio-driven, streaming, distillation  
- **[Vorch-Omni: Multi-Task Orchestration of Sight and Sound](https://arxiv.org/abs/2608.05803v1)**  
  Authors: Vorch Team, Xiaoyu Chen, Yang Ding, Cong Han, Menglin Han, Yuxin Hong, Jiebo Hou, Zequn Jie, Xiang Li, Jing Liu, Qi Liu, Yulei Lu, Siyuan Luo, Lin Ma, Xin Ma, Yinlong Qian, Peng Shi, Fang Wan, Siqi Wang, Yaohui Wang, Yaole Wang, Yidi Wu, Siqian Yang, Mingyu Yin, Haoran Yu, Gang Yue, Lisai Zhang, Yuting Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.05803v1.pdf)  
  Keywords: dit, sound, diffusion transformer, text-to-video, audio-driven  
- **[EchoCache: Energy-Guided Cross-Modal Caching for Efficient Audio-Driven Video Generation](https://arxiv.org/abs/2608.02474v3)**  
  Authors: Jiayu Chen, Xiaoyu Wu, Rongshan Gao, Maoliang Li, Zihao Zheng, Xinhao Sun, Hailong Zou, Guojie Luo, Xiang Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.02474v3.pdf) | [![GitHub](https://img.shields.io/github/stars/IF-LAB-PKU/EchoCache?style=social)](https://github.com/IF-LAB-PKU/EchoCache)  
  Keywords: efficient, diffusion model, benchmark, denoising, video generation, audio-driven  

### Controllable Generation

*Showing the latest 50 out of 124 papers*

- **[PAWBench: How Far Are We from Probabilistically Aligned World Modeling?](https://arxiv.org/abs/2608.27345v1)**  
  Authors: Yuandong Pu, Le Zhuo, Sayak Paul, Gabriel Jorge Menezes, Avram Đorđević, Shiyang Li, Yifan Zhou, Bin Fu, Wenlong Zhang, Junjun He, Yu Qiao, Yihao Liu, Jingbo Xing, Xi Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.27345v1.pdf)  
  Keywords: evaluation, physical, benchmark, video generation, world model, trajectory, dynamics  
- **[VBVR-Pro: A Scalable and Verifiable Suite for Native Visual Reasoning](https://arxiv.org/abs/2608.26105v1)**  
  Authors: Junxiang Xu, Ruisi Wang, Fanyi Pu, Maijunxian Wang, Ran Ji, Tongxi Zhou, Chenyang Gu, Jing Zuo, Hongcan Xiao, Yimeng Geng, Wanqi Yin, Wei Chen, Oscar Qian, Zhengan Yan, Ziqi Huang, Haiwen Diao, Liang Pan, Bo Li, Xiangyu Fan, Dezhi Luo, Fengyuan Yu, Zehong Zhao, Qingying Gao, Tinghui Zhu, Yilan Zhang, Jingqi Tong, Pinyuan Feng, Zhengze Jiang, Letian Wang, Ziyu Guo, Renrui Zhang, Jieneng Chen, Sonia Joseph, Constantin Venhoff, Saman Motamed, Mengyue Yang, Chandra Sripada, Alan Yuille, Philip Torr, Lvmin Zhang, Vikash Kumar, Daniel Khashabi, Nikolaus Kriegeskorte, Raphaël Millière, Vincent C. Müller, Anyi Rao, Quan Wang, Ziwei Liu, Dahua Lin, Lei Yang, Hokin Deng, Zhongang Cai  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.26105v1.pdf)  
  Keywords: evaluation, efficient, benchmark, video generation, controllable  
- **[4DStreamCtrl: Interactive Video Generation with Online 4D Control](https://arxiv.org/abs/2608.25479v2)**  
  Authors: Shiqian Li, Chenguo Lin, Zhiguang Liu, Yu Tang, Jiarong Ou, Rui Chen, Yixin Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.25479v2.pdf)  
  Keywords: dit, efficient, interactive, diffusion model, long video, denoising, video diffusion, video generation, controllable, world model, trajectory, streaming  
- **[TurboT2VA: Fast Large-Scale Text-to-Video-Audio Generation via Score-Regularized Consistency Distillation](https://arxiv.org/abs/2608.24674v1)**  
  Authors: Xiaoda Yang, Yuxiang Liu, Kaiwen Zheng, Yuan Liu, Yibo Lai, Shengpeng Ji, Kai Jiang, Jianfei Chen, Xiaobin Hu, Shuicheng Yan, Jintao Zhang, Jun Zhu, Zhou Zhao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.24674v1.pdf) | [![GitHub](https://img.shields.io/github/stars/thu-ml/TurboDiffusion?style=social)](https://github.com/thu-ml/TurboDiffusion)  
  Keywords: evaluation, distillation, dit, t2v, text-to-video, trajectory, architecture  
- **[Scaling Reinforcement Learning for Diffusion Models via Velocity Matching](https://arxiv.org/abs/2608.23664v1)**  
  Authors: Jaemoo Choi, Wei Guo, Yuchen Zhu, Arash Vahdat, Molei Tao, Julius Berner, Yongxin Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.23664v1.pdf)  
  Keywords: autoregressive, dit, diffusion model, denoising, video generation, trajectory  
- **[GeoWAM: Visual Geometry World Action Models for Autonomous Driving](https://arxiv.org/abs/2608.23486v2)**  
  Authors: Yiren Lu, Xin Ye, Jiaming Liu, Philip Jacobson, Jin Yao, Yi-chung Chen, Liam Merino, Dhruva Dixith Kurra, Min Cai, Tom Lampo, Yu Yin, Danhua Guo, Burhan Yaman  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.23486v2.pdf)  
  Keywords: evaluation, dit, autonomous driving, world model, trajectory, dynamics  
- **[Direct, Parallel, or Sequential? A Comparative Study of Training-Free Multi-Subject Image-to-Video Generation](https://arxiv.org/abs/2608.22819v1)**  
  Authors: Yanliang Qi, Kexi Chen, Muchao Ye, Haomiao Ni  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.22819v1.pdf)  
  Keywords: dit, image-to-video, temporal consistency, video generation, controllable, i2v  
- **[MotionPhys: Detecting AI-Generated Videos via Physical Consistency of Optical-Flow Trajectories](https://arxiv.org/abs/2608.20770v1)**  
  Authors: Haojin He, Hao Tan, Zichang Tan, Ajian Liu, Jun Wan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.20770v1.pdf)  
  Keywords: physical, efficient, trajectory, video generation  
- **[AvatarDynamizer: From Static to Dynamic Human Avatars via Generative Dynamic Textures](https://arxiv.org/abs/2608.19900v1)**  
  Authors: Guoxing Sun, Heming Zhu, Linjie Lyu, Pascal Fua, Christian Theobalt, Marc Habermann  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.19900v1.pdf)  
  Keywords: dit, diffusion model, avatar, video diffusion, controllable, dynamics  
- **[Magnitude-Direction Decoupling for Fast Video Generation with Flow Matching Models](https://arxiv.org/abs/2608.17695v1)**  
  Authors: Haonan Xu, Feiyang Chen, Songkui Chen, Hongpeng Pan, Zhefeng Wang, Xinyu Duan, Baoxing Huai, Yang Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.17695v1.pdf)  
  Keywords: flow matching, denoising, video generation, acceleration, trajectory  

### Human & Character Animation

- **[AvatarDynamizer: From Static to Dynamic Human Avatars via Generative Dynamic Textures](https://arxiv.org/abs/2608.19900v1)**  
  Authors: Guoxing Sun, Heming Zhu, Linjie Lyu, Pascal Fua, Christian Theobalt, Marc Habermann  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.19900v1.pdf)  
  Keywords: dit, diffusion model, avatar, video diffusion, controllable, dynamics  
- **[CL4D: Contrastive Language-4D Pretraining for Vision-Language Reasoning in Dynamic Scenes](https://arxiv.org/abs/2608.18734v1)**  
  Authors: Kumal Hewagamage, Isuranga Senavirathne, Sasika Amarasinghe, Hasitha Gallella, Dulanga Weerakoon, Vigneshwaran Subbaraju, Ranga Rodrigo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.18734v1.pdf)  
  Keywords: dit, physical, benchmark, human motion, dynamics  
- **[SingDance: Compositional Zero-Shot Singing-and-Dancing Video Generation with Role-Aware Audio Conditioning](https://arxiv.org/abs/2608.16220v1)**  
  Authors: Tao Feng, Xu Li, Xiangyang Luo, Ming Wen, Huadai Liu, Chen Zhang, Wei Xue  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.16220v1.pdf)  
  Keywords: speech-driven, dit, video diffusion, body motion, video generation, controllable  
- **[FlowDance: Music-Driven Dance Video Generation with Parallel Pose and RGB Streams](https://arxiv.org/abs/2608.15818v1)**  
  Authors: Genying Li, Boda Lin, Jiachen Li, Zijian Jia, Haojie Zheng, Yiming Wang, Shuchen Weng, Si Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.15818v1.pdf)  
  Keywords: long video, identity, denoising, body motion, video generation, human animation, video synthesis  
- **[Avatar-Forever: Decoupled Parallel Training for High-Quality Real-Time Infinite Avatars](https://arxiv.org/abs/2608.12107v1)**  
  Authors: Ruibin Li, Tao Yang, Zhiyuan Ma, Fangzhou Ai, Shilei Wen, Lei Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.12107v1.pdf)  
  Keywords: autoregressive, dit, efficient, interactive, identity, avatar, video generation, audio-driven, streaming, distillation  
- **[LiveAnimate: Stable Long-Form Streaming Human Animation in Real-Time](https://arxiv.org/abs/2608.11745v2)**  
  Authors: Yuxuan Zhang, Haozhong Xiong, Yubo Huang, Jiayi Song, Jinpeng Yu, Haofan Wang, Jiaming Liu, Ruihua Huang, Liwei Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.11745v2.pdf)  
  Keywords: autoregressive, dit, interactive, long-form, diffusion transformer, benchmark, identity, avatar, video diffusion, human animation, streaming, distillation  
- **[Ex-Omni-2D: Expressive Omni-Modal Dialogue Models with Native Visual Presence](https://arxiv.org/abs/2608.10720v1)**  
  Authors: Haoyu Zhang, Zhipeng Li, Xiaoying Tang, Tianshu Yu, Yiwen Guo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.10720v1.pdf)  
  Keywords: dit, efficient, streaming, avatar  
- **[Omni-LiveAvatar: Minute-Level Real-Time Streaming Joint Audio-Video Avatar Generation](https://arxiv.org/abs/2608.13602v2)**  
  Authors: Lunjie Zhu, Xingtong Ge, Fangyu Lin, Yi Zhang, Zhening Liu, Mengfei Li, Yumeng Zhang, Guanglu Song, Yu Liu, Jun Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.13602v2.pdf) | [![GitHub](https://img.shields.io/github/stars/Aoko955/Omni-LiveAvatar?style=social)](https://github.com/Aoko955/Omni-LiveAvatar)  
  Keywords: autoregressive, interactive, diffusion model, avatar, denoising, video diffusion, streaming, distillation  
- **[UniVVT: A Unified End-to-End Framework for High-Fidelity Video Virtual Try-on](https://arxiv.org/abs/2608.05745v2)**  
  Authors: Yushe Cao, Shikun Feng, Fei Shen, Haikuo Peng, Jianqiang Xia, Yiheng Zhu, Dianxi Shi, Chun Yu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.05745v2.pdf)  
  Keywords: dit, virtual try-on, benchmark, identity, video inpainting, video generation, dynamics  
- **[Vorch-Streamer: Extending Human Audio-Visual Generation to Real-Time Long-Form Streaming](https://arxiv.org/abs/2608.05663v2)**  
  Authors: Menglin Han, Yang Ding, Yulei Lu, Haoran Yu, Xin Ma, Junyi Chen, Zhangkai Ni, Lin Ma, Yaohui Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.05663v2.pdf)  
  Keywords: autoregressive, dit, long-form, identity, avatar, denoising, video generation, streaming, distillation  

### Image-to-Video Generation

*Showing the latest 50 out of 51 papers*

- **[TempJail: Temporal Jailbreak Attacks against Image-to-Video Generation Models](https://arxiv.org/abs/2608.26971v1)**  
  Authors: Qi Lu, Zehui Guo, David Yuanda Gan, Zijing Li, Hengda Zhang, Weijun Xu, Qiankun Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.26971v1.pdf) | [![GitHub](https://img.shields.io/github/stars/luqi-glory/TempJail?style=social)](https://github.com/luqi-glory/TempJail)  
  Keywords: evaluation, dit, image-to-video, video generation, video synthesis, i2v  
- **[Direct, Parallel, or Sequential? A Comparative Study of Training-Free Multi-Subject Image-to-Video Generation](https://arxiv.org/abs/2608.22819v1)**  
  Authors: Yanliang Qi, Kexi Chen, Muchao Ye, Haomiao Ni  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.22819v1.pdf)  
  Keywords: dit, image-to-video, temporal consistency, video generation, controllable, i2v  
- **[CaliBench: Are the Stochastic Dynamics of Video World Models Physically Calibrated?](https://arxiv.org/abs/2608.16829v1)**  
  Authors: Jonathan Sadeghi, Jenny Seidenschwarz, Jesse Allardice, Sirish Srinivasan, Benjamin Graham, Jeffrey Hawke  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.16829v1.pdf)  
  Keywords: physical, benchmark, image-to-video, world model, dynamics  
- **[EditStream: A Unified Autoregressive Framework for Interactive Video Generation and Editing](https://arxiv.org/abs/2608.21424v1)**  
  Authors: Yuqian Zhou, Zhenghong Zhou, Zongze Wu, Cameron Smith, Richard Zhang, Jiebo Luo, Eli Shechtman, Zhe Lin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.21424v1.pdf)  
  Keywords: autoregressive, dit, efficient, interactive, image-to-video, video generation, video-to-video, creative, text-to-video, video editing, streaming, distillation  
- **[RigidBench: Evaluating Rigid-Body Physics in Video Generation Models](https://arxiv.org/abs/2608.15555v1)**  
  Authors: Swarnim Jain, Shangzhe Wu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.15555v1.pdf)  
  Keywords: diffusion transformer, benchmark, identity, denoising, video generation, physics, trajectory, i2v  
- **[HPSD: Hybrid-Policy Self-Distillation for Text-Image-to-Video Diffusion Models](https://arxiv.org/abs/2608.13205v1)**  
  Authors: Jiazi Bu, Pengyang Ling, Yujie Zhou, Yibin Wang, Yuhang Zang, Xuanlang Dai, Shengyuan Ding, Tianyi Wei, Xiaohang Zhan, Jiaqi Wang, Tong Wu, Dahua Lin, Xingang Pan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.13205v1.pdf)  
  Keywords: distillation, dit, diffusion model, architecture, t2v, image-to-video, video diffusion, text-to-video, trajectory, i2v  
- **[Beyond Trial-and-Error: Agentic Optimization for Image-to-Video Adherence](https://arxiv.org/abs/2608.12290v1)**  
  Authors: Aman Tyagi, Hemanth Boinpally, Jonathan Chen, Douglas Gebert, Steven Hickson  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.12290v1.pdf)  
  Keywords: evaluation, efficient, image-to-video, video generation, video synthesis, i2v  
- **[SparSTAR: Sparse Attention for SpaceTime AutoRegressive Video Synthesis](https://arxiv.org/abs/2608.10519v2)**  
  Authors: Jongbeom Lee, Hyunwoo Yu, Jincheol Yang, Jaemin Choi, Suk-Ju Kang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.10519v2.pdf)  
  Keywords: autoregressive, dit, image-to-video, video generation, video synthesis, text-to-video  
- **[Bridging Event Streams and DiT: Event-Guided Video Frame Interpolation](https://arxiv.org/abs/2608.10479v2)**  
  Authors: Guixu Lin, Yuyang Yu, Xiang Ji, Linyao Chen, Zhengwei Yin, Mengshun Hu, Mingdeng Cao, Shengfeng He, Yinqiang Zheng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.10479v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://joseph-lin-tech.github.io/BridgeEventDiT-VFI)  
  Keywords: dit, diffusion model, frame interpolation, benchmark, image-to-video, video diffusion  
- **[Alpha as an Efficiency Signal: Visibility-Routed RGBA Image-to-Video Generation](https://arxiv.org/abs/2608.09355v1)**  
  Authors: Zhe Li, Honghao Qiao, Zhixin Xu, Qijie Wang, Bo Peng, Dawei Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.09355v1.pdf)  
  Keywords: evaluation, dit, style, denoising, image-to-video, video generation  

### Long Video Generation

*Showing the latest 50 out of 120 papers*

- **[Tether the Subject, Release the Scene: Query-Aware Memory Routing for Long-Horizon Autoregressive Video Generation](https://arxiv.org/abs/2608.26902v1)**  
  Authors: Chen Li, Peng Zhang, Hanyu Zhou, Jialong Zuo, Fei Wang, Daiguo Zhou, Nong Sang, Changxin Gao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.26902v1.pdf)  
  Keywords: autoregressive, dit, long video, identity, video generation, streaming  
- **[Ring Forcing: Towards Precise Long-Term Memory for Autoregressive Video Diffusion](https://arxiv.org/abs/2608.26794v1)**  
  Authors: Bowen Xue, Brandon Y. Feng, Chenguo Lin, Yuchen Lin, Yujia Zeng, Lvmin Zhang, Maneesh Agrawala, Honglei Yan, Panwang Pan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.26794v1.pdf)  
  Keywords: autoregressive, video diffusion, identity, video generation  
- **[RECAP-Forcing: Retaining Content Appearances for Long Video Generation](https://arxiv.org/abs/2608.26671v1)**  
  Authors: Haiyang Xu, Zheng Ding, Zhuowen Tu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.26671v1.pdf)  
  Keywords: autoregressive, long video, dit, video generation  
- **[StreamAV-Bench: A Comprehensive Benchmark for Streaming Audio-Video Generation](https://arxiv.org/abs/2608.26336v1)**  
  Authors: Kaiqi Liu, Haoxuan Zeng, Jingqi Liu, Jiacong Fang, Ziqi Cai, Yunyao Mao, Henglin Liu, Yu Sheng, Shuchen Weng, Boxin Shi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.26336v1.pdf)  
  Keywords: evaluation, interactive, benchmark, video generation, streaming  
- **[4DStreamCtrl: Interactive Video Generation with Online 4D Control](https://arxiv.org/abs/2608.25479v2)**  
  Authors: Shiqian Li, Chenguo Lin, Zhiguang Liu, Yu Tang, Jiarong Ou, Rui Chen, Yixin Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.25479v2.pdf)  
  Keywords: dit, efficient, interactive, diffusion model, long video, denoising, video diffusion, video generation, controllable, world model, trajectory, streaming  
- **[Scaling Reinforcement Learning for Diffusion Models via Velocity Matching](https://arxiv.org/abs/2608.23664v1)**  
  Authors: Jaemoo Choi, Wei Guo, Yuchen Zhu, Arash Vahdat, Molei Tao, Julius Berner, Yongxin Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.23664v1.pdf)  
  Keywords: autoregressive, dit, diffusion model, denoising, video generation, trajectory  
- **[Long-Horizon Audio-Visual Generation for Persistent Stories and Interactive Worlds](https://arxiv.org/abs/2608.23383v2)**  
  Authors: Nan Duan, Haoyang Huang, Weiyang Jin, Haoran Li, Yaowei Li, Yuming Li, Yijun Liu, Xin Lu, Xiaoxiao Ma, Yanwen Ma, Yaofeng Su, Yilang Sun, Haoyu Wang, Zeyue Xue, Songchun Zhang, Junhao Zhuang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.23383v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://echo-team-joy-future-academy-jd.github.io/Echo-1.5-Page)  
  Keywords: dit, efficient, interactive, long-form, identity, video generation  
- **[Loopy: Seamless Video Loop Generation via Anchored Looping Shift of Positional Embedding](https://arxiv.org/abs/2608.23090v1)**  
  Authors: Haotian Dong, Wenjing Wang, Chen Li, Jing Lyu, Xin Wang, Di Lin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.23090v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://donghaotian123.github.io/Loopy)  
  Keywords: dit, style, identity, temporal consistency, video generation  
- **[Direct, Parallel, or Sequential? A Comparative Study of Training-Free Multi-Subject Image-to-Video Generation](https://arxiv.org/abs/2608.22819v1)**  
  Authors: Yanliang Qi, Kexi Chen, Muchao Ye, Haomiao Ni  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.22819v1.pdf)  
  Keywords: dit, image-to-video, temporal consistency, video generation, controllable, i2v  
- **[TLive-Omni: An Omni-Modal Understanding Model for E-Commerce Live Streaming](https://arxiv.org/abs/2608.20958v1)**  
  Authors: Yibo Hu, Yu Qian, Mao Gu, Yingfan Tao, Yuhao Chen, Yongdong Luo, Zhuoqun Liu, Meiguang Jin, Junfeng Ma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.20958v1.pdf)  
  Keywords: style, long-form, benchmark, streaming  

### Personalization & Customization

*Showing the latest 50 out of 89 papers*

- **[Tether the Subject, Release the Scene: Query-Aware Memory Routing for Long-Horizon Autoregressive Video Generation](https://arxiv.org/abs/2608.26902v1)**  
  Authors: Chen Li, Peng Zhang, Hanyu Zhou, Jialong Zuo, Fei Wang, Daiguo Zhou, Nong Sang, Changxin Gao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.26902v1.pdf)  
  Keywords: autoregressive, dit, long video, identity, video generation, streaming  
- **[Ring Forcing: Towards Precise Long-Term Memory for Autoregressive Video Diffusion](https://arxiv.org/abs/2608.26794v1)**  
  Authors: Bowen Xue, Brandon Y. Feng, Chenguo Lin, Yuchen Lin, Yujia Zeng, Lvmin Zhang, Maneesh Agrawala, Honglei Yan, Panwang Pan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.26794v1.pdf)  
  Keywords: autoregressive, video diffusion, identity, video generation  
- **[Surgical Video Generation From Diffusion to World Models: A Survey](https://arxiv.org/abs/2608.26214v1)**  
  Authors: Fuxiang Huang, Chenxu Zhang, Liang Han, Lei Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.26214v1.pdf)  
  Keywords: multi-modal, dit, physical, survey, simulation, video generation, concept, world model, dynamics  
- **[PhysMLLMs: Spatial Priors for Unified Referring Segmentation and Grounded Reasoning of Images and Videos](https://arxiv.org/abs/2608.24574v1)**  
  Authors: Siyao Yan, Bo Han, Jisheng Dang, Bimei Wang, Shude Wang, Hong Peng, Yulan Guo, Jianhuang Lai, Bin Hu, Tat-SengChua  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.24574v1.pdf) | [![GitHub](https://img.shields.io/github/stars/tusu-code/20260121-icml2026-2.git?style=social)](https://github.com/tusu-code/20260121-icml2026-2.git)  
  Keywords: benchmark, identity, architecture, physics, distillation  
- **[Long-Horizon Audio-Visual Generation for Persistent Stories and Interactive Worlds](https://arxiv.org/abs/2608.23383v2)**  
  Authors: Nan Duan, Haoyang Huang, Weiyang Jin, Haoran Li, Yaowei Li, Yuming Li, Yijun Liu, Xin Lu, Xiaoxiao Ma, Yanwen Ma, Yaofeng Su, Yilang Sun, Haoyu Wang, Zeyue Xue, Songchun Zhang, Junhao Zhuang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.23383v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://echo-team-joy-future-academy-jd.github.io/Echo-1.5-Page)  
  Keywords: dit, efficient, interactive, long-form, identity, video generation  
- **[Loopy: Seamless Video Loop Generation via Anchored Looping Shift of Positional Embedding](https://arxiv.org/abs/2608.23090v1)**  
  Authors: Haotian Dong, Wenjing Wang, Chen Li, Jing Lyu, Xin Wang, Di Lin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.23090v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://donghaotian123.github.io/Loopy)  
  Keywords: dit, style, identity, temporal consistency, video generation  
- **[TLive-Omni: An Omni-Modal Understanding Model for E-Commerce Live Streaming](https://arxiv.org/abs/2608.20958v1)**  
  Authors: Yibo Hu, Yu Qian, Mao Gu, Yingfan Tao, Yuhao Chen, Yongdong Luo, Zhuoqun Liu, Meiguang Jin, Junfeng Ma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.20958v1.pdf)  
  Keywords: style, long-form, benchmark, streaming  
- **[Identity-Preserving Text-to-Video Generation via Agentic Enhancement and Semantic Repair](https://arxiv.org/abs/2608.20749v1)**  
  Authors: Jiayi Gao, Changcheng Hua, Jiaqi Tang, Yuxin Peng, Yang Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.20749v1.pdf) | [![GitHub](https://img.shields.io/github/stars/oceanflowlab/AESR?style=social)](https://github.com/oceanflowlab/AESR)  
  Keywords: evaluation, dit, identity, video generation, text-to-video, video editing  
- **[MoE-ViE: Mixture of Experts Vision Encoder for Efficient Image and Video Understanding](https://arxiv.org/abs/2608.17402v1)**  
  Authors: Bonan Zhang, Shiyu Dong, Quan Hung Tran, Katharina Gschwind, Shuqi Yang, Sijia Chen, Adel Ahmadyan, Seungwhan Moon, Lu Zhang, Ahmed Kirmani, Babak Damavandi, Anuj Kumar  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.17402v1.pdf) | [![GitHub](https://img.shields.io/github/stars/facebookresearch/moe_vie?style=social)](https://github.com/facebookresearch/moe_vie)  
  Keywords: efficient, style, benchmark, architecture, distillation  
- **[Seeing Before Answering: Training-Free Visual Layer Profiling for Vision-Language Models](https://arxiv.org/abs/2608.16263v1)**  
  Authors: Ruchen Liu, Yi Yang, Yiming Xu, Michael Ying Yang, Monika Sester, Bodo Rosenhahn  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.16263v1.pdf)  
  Keywords: style, benchmark  

### Physical Understanding

*Showing the latest 50 out of 143 papers*

- **[CLAP: Cross-Embodiment Video World Models are Zero-Shot Physical Simulators](https://arxiv.org/abs/2608.27406v1)**  
  Authors: Kechen Liu, Ola Shorinwa  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.27406v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://omni-clap.github.io)  
  Keywords: dit, physical, video generation, physics, world model, action-conditioned, dynamics  
- **[PAWBench: How Far Are We from Probabilistically Aligned World Modeling?](https://arxiv.org/abs/2608.27345v1)**  
  Authors: Yuandong Pu, Le Zhuo, Sayak Paul, Gabriel Jorge Menezes, Avram Đorđević, Shiyang Li, Yifan Zhou, Bin Fu, Wenlong Zhang, Junjun He, Yu Qiao, Yihao Liu, Jingbo Xing, Xi Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.27345v1.pdf)  
  Keywords: evaluation, physical, benchmark, video generation, world model, trajectory, dynamics  
- **[Surgical Video Generation From Diffusion to World Models: A Survey](https://arxiv.org/abs/2608.26214v1)**  
  Authors: Fuxiang Huang, Chenxu Zhang, Liang Han, Lei Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.26214v1.pdf)  
  Keywords: multi-modal, dit, physical, survey, simulation, video generation, concept, world model, dynamics  
- **[PhysMLLMs: Spatial Priors for Unified Referring Segmentation and Grounded Reasoning of Images and Videos](https://arxiv.org/abs/2608.24574v1)**  
  Authors: Siyao Yan, Bo Han, Jisheng Dang, Bimei Wang, Shude Wang, Hong Peng, Yulan Guo, Jianhuang Lai, Bin Hu, Tat-SengChua  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.24574v1.pdf) | [![GitHub](https://img.shields.io/github/stars/tusu-code/20260121-icml2026-2.git?style=social)](https://github.com/tusu-code/20260121-icml2026-2.git)  
  Keywords: benchmark, identity, architecture, physics, distillation  
- **[Markerless Pose Estimation for Resistance Training Technique Assessment](https://arxiv.org/abs/2608.24384v1)**  
  Authors: Joseph Turner, Jeff Clark, Nawid Keshtmand  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.24384v1.pdf)  
  Keywords: physical  
- **[GlanceWAM: Sparse Test-Time Imagination for World-Action Models](https://arxiv.org/abs/2608.23927v1)**  
  Authors: Linhan Wang, Zijian An, Mingyuan Zhang, Chen Dai, Yi Xu, Can Cui, Zichong Yang, Yinlin Chen, Lifeng Zhou, Chang-Tien Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.23927v1.pdf) | [![GitHub](https://img.shields.io/github/stars/linhanwang/GlanceWAM?style=social)](https://github.com/linhanwang/GlanceWAM)  
  Keywords: physical, dit, benchmark, video generation  
- **[GeoWAM: Visual Geometry World Action Models for Autonomous Driving](https://arxiv.org/abs/2608.23486v2)**  
  Authors: Yiren Lu, Xin Ye, Jiaming Liu, Philip Jacobson, Jin Yao, Yi-chung Chen, Liam Merino, Dhruva Dixith Kurra, Min Cai, Tom Lampo, Yu Yin, Danhua Guo, Burhan Yaman  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.23486v2.pdf)  
  Keywords: evaluation, dit, autonomous driving, world model, trajectory, dynamics  
- **[From Generation to Simulation: How Far Are World Models from Being True Simulators?](https://arxiv.org/abs/2608.23070v1)**  
  Authors: Tong Wang, Huan Deng, Mucheng Yang, Yang He, Xiaohui Kuang, Gang Zhao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.23070v1.pdf) | [![GitHub](https://img.shields.io/github/stars/AtongWang/world-model-simulators?style=social)](https://github.com/AtongWang/world-model-simulators)  
  Keywords: evaluation, dit, physical, diffusion model, simulation, video generation, physics, world model, dynamics  
- **[GuidedFlow: An Attention-Guided Framework for Anomaly Detection in Additive Manufacturing](https://arxiv.org/abs/2608.22789v1)**  
  Authors: Sosmita Paul, Krishna Roy  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.22789v1.pdf)  
  Keywords: physical, dit, dynamics  
- **[DELE-w0.5: Inferring Action from Future Latent State for Robotic Manipulation](https://arxiv.org/abs/2608.22067v3)**  
  Authors: Fenghao Lei, Zhixiong Huang, Long Yang, Jiabao Chen, Peilin Huang, Han Fu, Zhuo Li, Xiaoxue Ren  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.22067v3.pdf)  
  Keywords: physical, world model, video generation  

### Surveys & Benchmarks

*Showing the latest 50 out of 229 papers*

- **[PAWBench: How Far Are We from Probabilistically Aligned World Modeling?](https://arxiv.org/abs/2608.27345v1)**  
  Authors: Yuandong Pu, Le Zhuo, Sayak Paul, Gabriel Jorge Menezes, Avram Đorđević, Shiyang Li, Yifan Zhou, Bin Fu, Wenlong Zhang, Junjun He, Yu Qiao, Yihao Liu, Jingbo Xing, Xi Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.27345v1.pdf)  
  Keywords: evaluation, physical, benchmark, video generation, world model, trajectory, dynamics  
- **[TempJail: Temporal Jailbreak Attacks against Image-to-Video Generation Models](https://arxiv.org/abs/2608.26971v1)**  
  Authors: Qi Lu, Zehui Guo, David Yuanda Gan, Zijing Li, Hengda Zhang, Weijun Xu, Qiankun Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.26971v1.pdf) | [![GitHub](https://img.shields.io/github/stars/luqi-glory/TempJail?style=social)](https://github.com/luqi-glory/TempJail)  
  Keywords: evaluation, dit, image-to-video, video generation, video synthesis, i2v  
- **[Activation Outliers Matter: Robust Recovery for Quantized Multimodal LLMs](https://arxiv.org/abs/2608.26581v1)**  
  Authors: Tanzila Rahman, Mehran Taghian Jazi, Yunke Peng, Zhuang Ma, Anandharaju Durai Raju, Yao Wang, Xing Huang, Hei Yi Mak, Shadan Golestan, Hoang Le, Yonghan Dong, Wei Guo, Yaoyuan Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.26581v1.pdf)  
  Keywords: efficient, benchmark, video generation  
- **[Multi2AV-Safety: Benchmarking Safety in Multimodal-to-Audio-Video Generation](https://arxiv.org/abs/2608.26535v1)**  
  Authors: Kaichao Jiang, Changtao Miao, Baiqi Wu, Zhiyuan Lu, Kang Yang, Peiwei Zhao, Junchi Chen, Yunfeng Diao, He Liu, Qi Chu, Tao Gong, Nenghai Yu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.26535v1.pdf)  
  Keywords: evaluation, dit, benchmark, video generation  
- **[HUG-VIS: A Multimodal Benchmark for Human-centered Understanding and Generation in Visual Intelligence](https://arxiv.org/abs/2608.26517v1)**  
  Authors: Fei Ma, Zebang Cheng, Minghui Li, Hongbo Xu, Yuyong Tan, Yihua Shao, Hanling Wang, Zhou Liu, Yuqing Gao, Dong Wang, Long Ma, Laizhong Cui, Nicu Sebe, Qi Tian  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.26517v1.pdf) | [![GitHub](https://img.shields.io/github/stars/GML-MMGroup/HUG-VIS?style=social)](https://github.com/GML-MMGroup/HUG-VIS)  
  Keywords: benchmark, video generation  
- **[StreamAV-Bench: A Comprehensive Benchmark for Streaming Audio-Video Generation](https://arxiv.org/abs/2608.26336v1)**  
  Authors: Kaiqi Liu, Haoxuan Zeng, Jingqi Liu, Jiacong Fang, Ziqi Cai, Yunyao Mao, Henglin Liu, Yu Sheng, Shuchen Weng, Boxin Shi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.26336v1.pdf)  
  Keywords: evaluation, interactive, benchmark, video generation, streaming  
- **[Modality Maturity Index: A benchmark for assessing multimodal capabilities of omni models](https://arxiv.org/abs/2608.26317v1)**  
  Authors: Rohit Patel, Dieuwke Hupkes, Sloan Strader  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.26317v1.pdf)  
  Keywords: evaluation, benchmark  
- **[VBVR-Pro: A Scalable and Verifiable Suite for Native Visual Reasoning](https://arxiv.org/abs/2608.26105v1)**  
  Authors: Junxiang Xu, Ruisi Wang, Fanyi Pu, Maijunxian Wang, Ran Ji, Tongxi Zhou, Chenyang Gu, Jing Zuo, Hongcan Xiao, Yimeng Geng, Wanqi Yin, Wei Chen, Oscar Qian, Zhengan Yan, Ziqi Huang, Haiwen Diao, Liang Pan, Bo Li, Xiangyu Fan, Dezhi Luo, Fengyuan Yu, Zehong Zhao, Qingying Gao, Tinghui Zhu, Yilan Zhang, Jingqi Tong, Pinyuan Feng, Zhengze Jiang, Letian Wang, Ziyu Guo, Renrui Zhang, Jieneng Chen, Sonia Joseph, Constantin Venhoff, Saman Motamed, Mengyue Yang, Chandra Sripada, Alan Yuille, Philip Torr, Lvmin Zhang, Vikash Kumar, Daniel Khashabi, Nikolaus Kriegeskorte, Raphaël Millière, Vincent C. Müller, Anyi Rao, Quan Wang, Ziwei Liu, Dahua Lin, Lei Yang, Hokin Deng, Zhongang Cai  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.26105v1.pdf)  
  Keywords: evaluation, efficient, benchmark, video generation, controllable  
- **[Surgical Video Generation From Diffusion to World Models: A Survey](https://arxiv.org/abs/2608.26214v1)**  
  Authors: Fuxiang Huang, Chenxu Zhang, Liang Han, Lei Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.26214v1.pdf)  
  Keywords: multi-modal, dit, physical, survey, simulation, video generation, concept, world model, dynamics  
- **[VGA-BenchV2: An Expanded Unified Benchmark and Multi-Model Framework for Evaluating Video Aesthetics and Generation Quality](https://arxiv.org/abs/2608.25452v1)**  
  Authors: Longteng Jiang, DanDan Zheng, Qianqian Qiao, Heng Huang, Huaye Wang, Yihang Bo, Bao Peng, Jingdong Chen, Jun Zhou, Xin Jin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.25452v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://huggingface.co/datasets/BestiVictoryLab/VGA-Bench.) | [![Dataset](https://img.shields.io/badge/-Dataset-orange)](https://huggingface.co/datasets/BestiVictoryLab/VGA-Bench)  
  Keywords: evaluation, benchmark, video generation, architecture  

### Text-to-Video Generation

*Showing the latest 50 out of 74 papers*

- **[ClusterAttention: A training-free speedup of bidirectional attention](https://arxiv.org/abs/2608.26965v1)**  
  Authors: Kasper Nordenram, Amelie Dittmann  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.26965v1.pdf)  
  Keywords: video generation, t2v  
- **[TurboT2VA: Fast Large-Scale Text-to-Video-Audio Generation via Score-Regularized Consistency Distillation](https://arxiv.org/abs/2608.24674v1)**  
  Authors: Xiaoda Yang, Yuxiang Liu, Kaiwen Zheng, Yuan Liu, Yibo Lai, Shengpeng Ji, Kai Jiang, Jianfei Chen, Xiaobin Hu, Shuicheng Yan, Jintao Zhang, Jun Zhu, Zhou Zhao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.24674v1.pdf) | [![GitHub](https://img.shields.io/github/stars/thu-ml/TurboDiffusion?style=social)](https://github.com/thu-ml/TurboDiffusion)  
  Keywords: evaluation, distillation, dit, t2v, text-to-video, trajectory, architecture  
- **[OmniJudge or OmniBias? Diagnosing Multimodal Judges through Balanced, Decoupled Lenses](https://arxiv.org/abs/2608.24160v1)**  
  Authors: Guangzheng Hu, Ziyue Jiang, Weixu Qiao, Lixin Zhang, Jianye Kang, Yuru Wu, Rong Bao, Niantong Li, Wei Wang, Ziyi Cheng, Xinfa Zhu, HangRui Hu, Ting He, Bing Zhao, Lin Qu, Hu Wei, Jin Xu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.24160v1.pdf)  
  Keywords: evaluation, text-to-video, benchmark, t2v  
- **[FIRM-Video: Check Before You Score for Reliable Text-to-Video Reward Modeling](https://arxiv.org/abs/2608.21839v1)**  
  Authors: Peiyuan Zhang, Xiangyu Zhao, Hongbo Liu, Xiaoxing Hu, Mingxin Liu, Shuran Ma, Yunhang Shen, Jian Hu, Haihan Gao, Haoyu Cao, Xue Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.21839v1.pdf)  
  Keywords: evaluation, text-to-video  
- **[Identity-Preserving Text-to-Video Generation via Agentic Enhancement and Semantic Repair](https://arxiv.org/abs/2608.20749v1)**  
  Authors: Jiayi Gao, Changcheng Hua, Jiaqi Tang, Yuxin Peng, Yang Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.20749v1.pdf) | [![GitHub](https://img.shields.io/github/stars/oceanflowlab/AESR?style=social)](https://github.com/oceanflowlab/AESR)  
  Keywords: evaluation, dit, identity, video generation, text-to-video, video editing  
- **[SQuad: Sub-Quadratic Attention Distillation for Efficient Video Generation](https://arxiv.org/abs/2608.16585v1)**  
  Authors: Animesh Karnewar, Denis Korzhenkov, Amirhossein Habibian, Mohsen Ghafoorian  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.16585v1.pdf)  
  Keywords: evaluation, dit, efficient, diffusion transformer, video diffusion, video generation, text-to-video, distillation  
- **[MLLM-Guided Semantic Correction for Text-to-Video Generation](https://arxiv.org/abs/2608.16513v1)**  
  Authors: Junhao Chen, Zheqi Lv, Keting Yin, Shengyu Zhang, Zhou Zhao, Feiyang Chen, Xinyu Duan, Baoxing Huai, Fei Wu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.16513v1.pdf)  
  Keywords: evaluation, diffusion model, benchmark, temporal consistency, video generation, video synthesis, controllable, text-to-video, trajectory, architecture  
- **[EditStream: A Unified Autoregressive Framework for Interactive Video Generation and Editing](https://arxiv.org/abs/2608.21424v1)**  
  Authors: Yuqian Zhou, Zhenghong Zhou, Zongze Wu, Cameron Smith, Richard Zhang, Jiebo Luo, Eli Shechtman, Zhe Lin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.21424v1.pdf)  
  Keywords: autoregressive, dit, efficient, interactive, image-to-video, video generation, video-to-video, creative, text-to-video, video editing, streaming, distillation  
- **[Beyond Text Conditioning: A Systematic Study of MLLM-DiT Fusion for Video Generation](https://arxiv.org/abs/2608.14043v1)**  
  Authors: Yanbo Ding, Yijia Fan, Caihua Shan, Yifan Yang, Yifei Shen, Weijie Wang, Xirui Hu, Dongsheng Li, Lili Qiu, Yuqing Yang, Yali Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.14043v1.pdf)  
  Keywords: autoregressive, dit, diffusion transformer, video generation, text-to-video, architecture  
- **[HPSD: Hybrid-Policy Self-Distillation for Text-Image-to-Video Diffusion Models](https://arxiv.org/abs/2608.13205v1)**  
  Authors: Jiazi Bu, Pengyang Ling, Yujie Zhou, Yibin Wang, Yuhang Zang, Xuanlang Dai, Shengyuan Ding, Tianyi Wei, Xiaohang Zhan, Jiaqi Wang, Tong Wu, Dahua Lin, Xingang Pan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.13205v1.pdf)  
  Keywords: distillation, dit, diffusion model, architecture, t2v, image-to-video, video diffusion, text-to-video, trajectory, i2v  

### Video Editing

- **[FixAnything: 3D-Consistent Rendering Refinement via Video Generative Priors](https://arxiv.org/abs/2608.23549v1)**  
  Authors: Khiem Vuong, Deva Ramanan, Srinivasa Narasimhan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.23549v1.pdf)  
  Keywords: video translation, architecture, video-to-video  
- **[InfinityEdit: Infinite Video Editing with a Lightweight Edit-Ignition Adapter](https://arxiv.org/abs/2608.20910v1)**  
  Authors: Yunze Tong, Mushui Liu, Canyu Zhao, Shiyi Zhang, Didi Zhu, Peng Zhang, Wanggui He, Jinlong Liu, Ying Chen, Hao Jiang, Pipei Huang, Bo Zheng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.20910v1.pdf)  
  Keywords: denoising, dit, video editing, streaming  
- **[Identity-Preserving Text-to-Video Generation via Agentic Enhancement and Semantic Repair](https://arxiv.org/abs/2608.20749v1)**  
  Authors: Jiayi Gao, Changcheng Hua, Jiaqi Tang, Yuxin Peng, Yang Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.20749v1.pdf) | [![GitHub](https://img.shields.io/github/stars/oceanflowlab/AESR?style=social)](https://github.com/oceanflowlab/AESR)  
  Keywords: evaluation, dit, identity, video generation, text-to-video, video editing  
- **[EditStream: A Unified Autoregressive Framework for Interactive Video Generation and Editing](https://arxiv.org/abs/2608.21424v1)**  
  Authors: Yuqian Zhou, Zhenghong Zhou, Zongze Wu, Cameron Smith, Richard Zhang, Jiebo Luo, Eli Shechtman, Zhe Lin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.21424v1.pdf)  
  Keywords: autoregressive, dit, efficient, interactive, image-to-video, video generation, video-to-video, creative, text-to-video, video editing, streaming, distillation  
- **[Instruction-Based Video Editing by Repurposing an Image Editing Model](https://arxiv.org/abs/2608.14790v3)**  
  Authors: Yunpeng Bai, Yossi Gandelsman, Michaël Gharbi, Qixing Huang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.14790v3.pdf) | [![GitHub](https://img.shields.io/github/stars/yunpeng1998/Qwen-Video-Edit?style=social)](https://github.com/yunpeng1998/Qwen-Video-Edit) | [![Project](https://img.shields.io/badge/-Project-blue)](https://yunpeng1998.github.io/Qwen-Video-Edit-Page) | [![HuggingFace](https://img.shields.io/badge/-HuggingFace-yellow)](https://huggingface.co/yunpeng1998/Qwen-Video-Edit)  
  Keywords: dit, diffusion transformer, denoising, video diffusion, video editing  
- **[EgoPlay: Event-Triggered Video Editing for Egocentric Streams](https://arxiv.org/abs/2607.24560v1)**  
  Authors: Jinjie Mai, Gordon Guocheng Qian, Willi Menapace, Arpit Sahni, Chaoyang Wang, Ashkan Mirzaei, Runjia Li, Sergey Tulyakov, Bernard Ghanem, Peter Wonka, Rameen Abdal  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.24560v1.pdf)  
  Keywords: evaluation, dit, diffusion transformer, benchmark, video diffusion, video-to-video, video editing  
- **[ID-V2V: Identity-Preserving Video Restylization](https://arxiv.org/abs/2607.22830v2)**  
  Authors: Yuancheng Xu, Mingming He, Pablo Salamanca, Li Ma, Yash Kant, Emmett Steven, Paul Debevec, Ning Yu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.22830v2.pdf) | [![GitHub](https://img.shields.io/github/stars/Eyeline-Labs/ID-V2V?style=social)](https://github.com/Eyeline-Labs/ID-V2V)  
  Keywords: dit, style, identity, video-to-video, creative, video synthesis  
- **[OSVE: One Step Video Editing with One Step Diffusion Models](https://arxiv.org/abs/2607.19895v1)**  
  Authors: Habin Lim, Gyeong-Moon Park  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.19895v1.pdf) | [![GitHub](https://img.shields.io/github/stars/KU-VGI/OSVE?style=social)](https://github.com/KU-VGI/OSVE)  
  Keywords: dit, diffusion model, long video, temporal consistency, video editing  
- **[AniGS: Bridging Rendering and Diffusion Prior for 3D Scene Animation](https://arxiv.org/abs/2607.18539v1)**  
  Authors: Yen-Chi Cheng, Chen Gao, Chuhan Chen, Tuotuo Li, Rajvi Shah, Ayush Saraf, Changil Kim, Liangyan Gui, Alexander Schwing, Johannes Kopf, Hung-Yu Tseng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.18539v1.pdf)  
  Keywords: dit, diffusion model, video diffusion, novel view, video-to-video, dynamics  
- **[PE-Field 4D: Video Generation Models as Canvas](https://arxiv.org/abs/2607.15667v1)**  
  Authors: Yunpeng Bai, Haoxiang Li, Qixing Huang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.15667v1.pdf) | [![GitHub](https://img.shields.io/github/stars/MTLab/PE-Field?style=social)](https://github.com/MTLab/PE-Field)  
  Keywords: dit, diffusion model, diffusion transformer, denoising, video diffusion, video generation, video synthesis, controllable, video editing, trajectory  

### Video Inpainting & Completion

- **[V-RAE: Rethinking Video Latent Spaces for Generation](https://arxiv.org/abs/2608.13556v1)**  
  Authors: Minghui Guo, Shengqiong Wu, Hao Fei  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.13556v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://v-rae.github.io)  
  Keywords: dit, latent video, video prediction, video generation, architecture  
- **[GeoRoute: Geometry-Aware Hybrid Inference for Traffic Future-Frame Prediction](https://arxiv.org/abs/2608.09493v1)**  
  Authors: Khang Minh Le, Hieu Dinh Trung Pham, Luu Thanh Danh, Nam-Tien Le, Hieu Anh Ngo, Phuong Huu Vu Tran, Son Nguyen Minh Le, Nguyen Trong Nghia, Tu Tran Thi Cam, Huy Minh Nhat Nguyen, Cuong Tuan Nguyen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.09493v1.pdf)  
  Keywords: dit, diffusion model, benchmark, latent video, video prediction, autonomous driving, video diffusion, architecture  
- **[SimWAM: A Simple World Action Model for End-to-End Autonomous Driving](https://arxiv.org/abs/2608.07468v4)**  
  Authors: Zongchuang Zhao, Xin Zhou, Tianyang Xu, Zhengyang Sun, Kaixuan Zhou, Yu Wu, Honglin Li, Dingkang Liang, Xiang Bai  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.07468v4.pdf) | [![GitHub](https://img.shields.io/github/stars/H-EmbodVis/SimWAM?style=social)](https://github.com/H-EmbodVis/SimWAM)  
  Keywords: efficient, video prediction, autonomous driving, video generation, flow matching, trajectory, dynamics  
- **[MirrorWorld: Taming Video Diffusion Models for Mirror Reflection Generation](https://arxiv.org/abs/2608.07463v1)**  
  Authors: Youjun Zhao, Alex Warren, Gary K. L. Tam, Rynson W. H. Lau  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.07463v1.pdf)  
  Keywords: diffusion model, benchmark, video inpainting, video diffusion, video synthesis, distillation  
- **[UniVVT: A Unified End-to-End Framework for High-Fidelity Video Virtual Try-on](https://arxiv.org/abs/2608.05745v2)**  
  Authors: Yushe Cao, Shikun Feng, Fei Shen, Haikuo Peng, Jianqiang Xia, Yiheng Zhu, Dianxi Shi, Chun Yu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.05745v2.pdf)  
  Keywords: dit, virtual try-on, benchmark, identity, video inpainting, video generation, dynamics  
- **[CrossScope: A Role-Asymmetric World Model for Joint Dual-Scope Surgical Video Prediction](https://arxiv.org/abs/2608.03211v1)**  
  Authors: Wanhao Liu, Jinsong Lin, Rulin Zhou, Chi Kit Ng, Wenbin Pan, Zhiqing Tang, Dongyue Li, Liwei Luo, Yanshen Wu, Panshuo Li, Zhiyong Xiong, Huxin Gao, Tamas Haidegger, Hongliang Ren  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.03211v1.pdf)  
  Keywords: evaluation, benchmark, video prediction, video generation, world model, dynamics  
- **[Schrödinger's Cat: Probabilistic Representation and Prediction of Potential Scene Kinematics](https://arxiv.org/abs/2607.25984v1)**  
  Authors: Timy Phan, Jannik Wiese, Björn Ommer  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.25984v1.pdf)  
  Keywords: dit, efficient, interactive, video prediction, video generation, trajectory  
- **[The Seriality Gap in Video Diffusion Models](https://arxiv.org/abs/2607.13031v1)**  
  Authors: Jorge Diaz Chao, Konpat Preechakul, Yuxi Liu, Yutong Bai  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.13031v1.pdf)  
  Keywords: autoregressive, diffusion model, video prediction, denoising, video diffusion, simulation, dynamics  
- **[Video Generation Models Are Inherent Lighting Estimators](https://arxiv.org/abs/2607.04674v1)**  
  Authors: Ziqi Cai, Shuchen Weng, Kaiqi Liu, Zifeng Wang, Zhiquan Zhang, Minggui Teng, Han Jiang, Boxin Shi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.04674v1.pdf)  
  Keywords: efficient, physical, diffusion model, video inpainting, video diffusion, video generation  

### Video Super-Resolution & Enhancement

*Showing the latest 50 out of 79 papers*

- **[4DStreamCtrl: Interactive Video Generation with Online 4D Control](https://arxiv.org/abs/2608.25479v2)**  
  Authors: Shiqian Li, Chenguo Lin, Zhiguang Liu, Yu Tang, Jiarong Ou, Rui Chen, Yixin Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.25479v2.pdf)  
  Keywords: dit, efficient, interactive, diffusion model, long video, denoising, video diffusion, video generation, controllable, world model, trajectory, streaming  
- **[Generalization, memorization, and overfitting for diffusion models trained in the lazy high-dimensional regime](https://arxiv.org/abs/2608.23938v1)**  
  Authors: Hugo Latourelle-Vigeant, Sinho Chewi, Aram-Alexandre Pooladian, John Sous, Theodor Misiakiewicz  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.23938v1.pdf)  
  Keywords: denoising, diffusion model, video synthesis  
- **[Scaling Reinforcement Learning for Diffusion Models via Velocity Matching](https://arxiv.org/abs/2608.23664v1)**  
  Authors: Jaemoo Choi, Wei Guo, Yuchen Zhu, Arash Vahdat, Molei Tao, Julius Berner, Yongxin Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.23664v1.pdf)  
  Keywords: autoregressive, dit, diffusion model, denoising, video generation, trajectory  
- **[GaussVid: Sparse-View Gaussian Splatting with 3D-Aware Video Diffusion Priors](https://arxiv.org/abs/2608.21849v1)**  
  Authors: Xinhui Liu, Can Wang, Wei Jiang, Wei Wang, Dong Xu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.21849v1.pdf)  
  Keywords: video restoration, 3d-aware, dit, diffusion model, video diffusion, video generation, novel view  
- **[InfinityEdit: Infinite Video Editing with a Lightweight Edit-Ignition Adapter](https://arxiv.org/abs/2608.20910v1)**  
  Authors: Yunze Tong, Mushui Liu, Canyu Zhao, Shiyi Zhang, Didi Zhu, Peng Zhang, Wanggui He, Jinlong Liu, Ying Chen, Hao Jiang, Pipei Huang, Bo Zheng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.20910v1.pdf)  
  Keywords: denoising, dit, video editing, streaming  
- **[4DAnyone: Create Anyone in 4D from a Casual Monocular Video](https://arxiv.org/abs/2608.20335v1)**  
  Authors: Yudong Jin, Tao Xie, Qihang Zhang, Zehong Shen, Zhen Xu, Yujun Shen, Hujun Bao, Xiaowei Zhou, Yinghao Xu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.20335v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://4danyone.github.io)  
  Keywords: denoising, diffusion model, video diffusion, dit  
- **[VGI-Bench: Probing Visual Intelligence in Video Generation Models](https://arxiv.org/abs/2608.19583v3)**  
  Authors: Xuan He, Cong Wei, Yuhao Cheng, Linrui Ma, Yuxuan Zhang, Zuojun Li, Yuhao Wen, Jize Jiang, Zeyi Liu, Yuren Hao, Songcheng Cai, Keming Wu, Penghui Du, Kai Zou, Rui Yang, Chenkai Sun, Ke Yang, Ping Nie, Kelsey R Allen, Chenglong Wang, Michel Galley, Jianfeng Gao, ChengXiang Zhai  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.19583v3.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://hexuan21.github.io/VGI-Bench)  
  Keywords: evaluation, dit, benchmark, denoising, video generation  
- **[Magnitude-Direction Decoupling for Fast Video Generation with Flow Matching Models](https://arxiv.org/abs/2608.17695v1)**  
  Authors: Haonan Xu, Feiyang Chen, Songkui Chen, Hongpeng Pan, Zhefeng Wang, Xinyu Duan, Baoxing Huai, Yang Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.17695v1.pdf)  
  Keywords: flow matching, denoising, video generation, acceleration, trajectory  
- **[DriveCache: Action-Aware Caching for Driving World Model Inference](https://arxiv.org/abs/2608.16354v1)**  
  Authors: Jianchun Yang, Jian Liang, Xianda Guo, Pinhan Fu, Yanlun Peng, Conglang Zhang, Wenke Huang, Mang Ye  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.16354v1.pdf)  
  Keywords: evaluation, acceleration, denoising, simulation, video generation, controllable, world model  
- **[FlowDance: Music-Driven Dance Video Generation with Parallel Pose and RGB Streams](https://arxiv.org/abs/2608.15818v1)**  
  Authors: Genying Li, Boda Lin, Jiachen Li, Zijian Jia, Haojie Zheng, Yiming Wang, Shuchen Weng, Si Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.15818v1.pdf)  
  Keywords: long video, identity, denoising, body motion, video generation, human animation, video synthesis  

### World Models & Simulation

*Showing the latest 50 out of 120 papers*

- **[CLAP: Cross-Embodiment Video World Models are Zero-Shot Physical Simulators](https://arxiv.org/abs/2608.27406v1)**  
  Authors: Kechen Liu, Ola Shorinwa  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.27406v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://omni-clap.github.io)  
  Keywords: dit, physical, video generation, physics, world model, action-conditioned, dynamics  
- **[PAWBench: How Far Are We from Probabilistically Aligned World Modeling?](https://arxiv.org/abs/2608.27345v1)**  
  Authors: Yuandong Pu, Le Zhuo, Sayak Paul, Gabriel Jorge Menezes, Avram Đorđević, Shiyang Li, Yifan Zhou, Bin Fu, Wenlong Zhang, Junjun He, Yu Qiao, Yihao Liu, Jingbo Xing, Xi Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.27345v1.pdf)  
  Keywords: evaluation, physical, benchmark, video generation, world model, trajectory, dynamics  
- **[SpatialCrafter: Single Image World Modeling with Generative 3D Proxies](https://arxiv.org/abs/2608.27073v1)**  
  Authors: Chuan Fang, Lingteng Qiu, Yixun Liang, Rui Chen, Kunming Luo, Zhaohua Zheng, Tongyuan Bai, Feipeng Tian, Zilong Dong, Zihan Zhou, Ping Tan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.27073v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://fangchuan.github.io/SpatialCrafter)  
  Keywords: dit, diffusion model, video diffusion, robotics, world model  
- **[StreamAV-Bench: A Comprehensive Benchmark for Streaming Audio-Video Generation](https://arxiv.org/abs/2608.26336v1)**  
  Authors: Kaiqi Liu, Haoxuan Zeng, Jingqi Liu, Jiacong Fang, Ziqi Cai, Yunyao Mao, Henglin Liu, Yu Sheng, Shuchen Weng, Boxin Shi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.26336v1.pdf)  
  Keywords: evaluation, interactive, benchmark, video generation, streaming  
- **[Surgical Video Generation From Diffusion to World Models: A Survey](https://arxiv.org/abs/2608.26214v1)**  
  Authors: Fuxiang Huang, Chenxu Zhang, Liang Han, Lei Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.26214v1.pdf)  
  Keywords: multi-modal, dit, physical, survey, simulation, video generation, concept, world model, dynamics  
- **[4DStreamCtrl: Interactive Video Generation with Online 4D Control](https://arxiv.org/abs/2608.25479v2)**  
  Authors: Shiqian Li, Chenguo Lin, Zhiguang Liu, Yu Tang, Jiarong Ou, Rui Chen, Yixin Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.25479v2.pdf)  
  Keywords: dit, efficient, interactive, diffusion model, long video, denoising, video diffusion, video generation, controllable, world model, trajectory, streaming  
- **[Primate vision reveals a missing principle for robust dynamic AI](https://arxiv.org/abs/2608.23790v1)**  
  Authors: Matteo Dunnhofer, Christian Micheloni, Kohitij Kar  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.23790v1.pdf)  
  Keywords: world model  
- **[GeoWAM: Visual Geometry World Action Models for Autonomous Driving](https://arxiv.org/abs/2608.23486v2)**  
  Authors: Yiren Lu, Xin Ye, Jiaming Liu, Philip Jacobson, Jin Yao, Yi-chung Chen, Liam Merino, Dhruva Dixith Kurra, Min Cai, Tom Lampo, Yu Yin, Danhua Guo, Burhan Yaman  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.23486v2.pdf)  
  Keywords: evaluation, dit, autonomous driving, world model, trajectory, dynamics  
- **[Long-Horizon Audio-Visual Generation for Persistent Stories and Interactive Worlds](https://arxiv.org/abs/2608.23383v2)**  
  Authors: Nan Duan, Haoyang Huang, Weiyang Jin, Haoran Li, Yaowei Li, Yuming Li, Yijun Liu, Xin Lu, Xiaoxiao Ma, Yanwen Ma, Yaofeng Su, Yilang Sun, Haoyu Wang, Zeyue Xue, Songchun Zhang, Junhao Zhuang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.23383v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://echo-team-joy-future-academy-jd.github.io/Echo-1.5-Page)  
  Keywords: dit, efficient, interactive, long-form, identity, video generation  
- **[From Generation to Simulation: How Far Are World Models from Being True Simulators?](https://arxiv.org/abs/2608.23070v1)**  
  Authors: Tong Wang, Huan Deng, Mucheng Yang, Yang He, Xiaohui Kuang, Gang Zhao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.23070v1.pdf) | [![GitHub](https://img.shields.io/github/stars/AtongWang/world-model-simulators?style=social)](https://github.com/AtongWang/world-model-simulators)  
  Keywords: evaluation, dit, physical, diffusion model, simulation, video generation, physics, world model, dynamics  



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
