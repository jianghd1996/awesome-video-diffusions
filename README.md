# Awesome Video Diffusions [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of latest research papers, projects and resources related to Video Diffusion Models and Video Generation. Content is automatically updated daily.

> Last Update: 2026-07-16 05:31:06

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

- [3D-aware Video Generation](#3d-aware-video-generation) (24 papers) - Video generation with 3D awareness, multi-view consistency, and 4D content creation
- [Applications](#applications) (50 papers) - Domain-specific applications of video diffusion models
- [Architecture & Efficiency](#architecture-&-efficiency) (363 papers) - Architectural innovations (DiT, UNet), flow matching, and training/inference efficiency
- [Audio & Multi-modal](#audio-&-multi-modal) (21 papers) - Audio-driven and multi-modal conditioned video generation
- [Controllable Generation](#controllable-generation) (138 papers) - Controllable video generation with motion, camera, pose, or layout guidance
- [Human & Character Animation](#human-&-character-animation) (23 papers) - Human-centric video generation including talking heads, dance, and character animation
- [Image-to-Video Generation](#image-to-video-generation) (49 papers) - Methods for animating still images into videos
- [Long Video Generation](#long-video-generation) (126 papers) - Generating temporally consistent long-form videos beyond short clips
- [Personalization & Customization](#personalization-&-customization) (94 papers) - Personalized video generation with custom subjects, identities, or styles
- [Physical Understanding](#physical-understanding) (157 papers) - Physics-aware video generation and dynamics modeling
- [Surveys & Benchmarks](#surveys-&-benchmarks) (230 papers) - Survey papers, benchmarks, and evaluation metrics for video generation
- [Text-to-Video Generation](#text-to-video-generation) (74 papers) - Foundation models and methods for generating videos from text prompts
- [Video Editing](#video-editing) (28 papers) - Diffusion-based video editing, style transfer, and manipulation
- [Video Inpainting & Completion](#video-inpainting-&-completion) (11 papers) - Video inpainting, completion, outpainting, and temporal prediction
- [Video Super-Resolution & Enhancement](#video-super-resolution-&-enhancement) (67 papers) - Video quality improvement, upscaling, restoration, and frame interpolation
- [World Models & Simulation](#world-models-&-simulation) (127 papers) - Video generation as world simulators and interactive environment generation



## Table of Contents

- [Categorized Papers](#categorized-papers)
- [Classic Papers](#classic-papers)
- [Open Source Projects](#open-source-projects)
- [Applications](#applications)
- [Tutorials & Blogs](#tutorials--blogs)





## Categorized Papers

### 3D-aware Video Generation

- **[Delving into the Temporal Challenges of Unified Video Protection Against Image-to-Video and Fine-Tuning-based Customization](https://arxiv.org/abs/2607.13336v1)**  
  Authors: Yuxin Huang, Ziming Hong, Mingming Gong, Wanyu Wang, Jing Zhang, Tongliang Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.13336v1.pdf)  
  Keywords: identity, image-to-video, dit, video diffusion, 3d video, video generation, customization, diffusion model  
- **[4D Human-Scene Reconstruction from Low-Overlap Captures](https://arxiv.org/abs/2607.09125v1)**  
  Authors: Minhyuk Hwang, Sangmin Kim, Seunguk Do, Daneul Kim, Jaesik Park  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.09125v1.pdf)  
  Keywords: identity, novel view, video diffusion, trajectory, diffusion model  
- **[SoccerNet 2026 Challenges Results](https://arxiv.org/abs/2607.07320v1)**  
  Authors: Anthony Cioppa, Silvio Giancola, Håkan Ardö, Mohamad Dalal, Jan Held, Jérémie Ochin, Jiayuan Rao, Karen Sanchez, Renaud Vandeghen, Artur Xarles, Olivier Barnich, Albert Clapés, Mathieu Delvaux, Sergio Escalera, Bernard Ghanem, Cédric Hons, Antoine Houet, Sotiris Manitsaris, Tom Michel, Pierre Miralles, Thomas B. Moeslund, Mikael Nilsson, Bogdan Stanciulescu, Marc Van Droogenbroeck, Yanfeng Wang, Weidi Xie, Faisal Altawijri, Mohamed Atef, Semen Budennyy, Vasiliy Chelpanov, Puhua Chen, Yixin Chen, Lechao Cheng, Jianling Chu, Ju-Seong Do, Oleg Durygin, Omar Fetouh, Mirco Fuchs, Youssef Ghallab, Falguni Ghosh, Wonjun Heo, Yufeng Hu, Weixuan Huang, Phuong-Linh Huynh-Ha, Matvey Isupov, Yangguang Ji, Siyuan Jiang, Zhenxiang Jiang, Wonyong Jo, Ho-Young Jung, SeongHeon Kang, MinJae Kim, Youngseon Kim, Jakub Komosa, Artem Konshin, Trung-Hoang Le, Jongmin Lee, Lingling Li, Litao Li, Vadim Linkov, Fang Liu, Haoxuan Ma, Shun Makino, Ismail Mathkour, Konstantin Mitin, Mikhail Moiseev, Takumi Nagaya, Yuki Nakamura, Thanh-Khoi Nguyen, Hoang-Phuc Nguyen, Trong-Thuan Nguyen, Christian Orduz, Kwanyong Park, Fabian Perez, Parthsarthi Rawat, SuHyun Rim, Hoover Rueda-Chacón, Atom Scott, Minori Sugimura, Yuyang Sun, Shengeng Tang, Minh-Triet Tran, Ikuma Uchida, Juan Vanegas, Thanh-Nhan Vo, Jiangtao Wang, Yaxiong Wang, Xiaogang Wang, Ruifeng Wang, Rio Watanabe, Jiali Wen, Yongliang Wu, Di Yang, Xu Yang, Zhuo Yang, Xinyu Ye, Yibo Yu, Zihan Zhai, Yu Zhang, Zhenyu Zhao, Zhun Zhong, Yixi Zhou, Xingyu Zhu, Wenbo Zhu, Julian Ziegler  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.07320v1.pdf)  
  Keywords: dit, benchmark, novel view, evaluation  
- **[MV-Forcing: Long Multi-View Video Generation via 4D-Grounded Spatio-Temporal Self-Forcing](https://arxiv.org/abs/2607.05376v1)**  
  Authors: Gal Fiebelman, Hadar Averbuch-Elor, Sagie Benaim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.05376v1.pdf)  
  Keywords: distillation, autoregressive, video diffusion, denoising, multi-view video, video generation, diffusion model  
- **[HandsOnWorld: Unconstrained Egocentric Video Generation with Camera-Disentangled Hand Control](https://arxiv.org/abs/2607.02075v1)**  
  Authors: Yushuo Chen, Xiaoyu Shi, Xiaoshi Wu, Xintao Wang, Pengfei Wan, Yebin Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.02075v1.pdf)  
  Keywords: 3d-aware, video generation  
- **[NeoMap: Training-free Novel-View Synthesis from Single Images and Videos](https://arxiv.org/abs/2607.01962v1)**  
  Authors: Jinxi Li, Tianyi Zhang, Yafei Yang, Zihui Zhang, Peng Huang, Koon Wing Macgyver Lin, Bo Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.01962v1.pdf)  
  Keywords: novel view, dit, benchmark, denoising, video synthesis  
- **[RayPE: Ray-Space Positional Encoding for 3D-Aware Video Generation](https://arxiv.org/abs/2606.27345v2)**  
  Authors: Minghao Yin, Jiahao Lu, Wenbo Hu, Wang Zhao, Shan Ying, Kai Han  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.27345v2.pdf)  
  Keywords: identity, camera control, dit, video diffusion, 3d-aware, video generation, diffusion transformer  
- **[Follow Your Track: Precise Skeleton Animation Controlled by 3D Trajectories](https://arxiv.org/abs/2606.25344v1)**  
  Authors: Yueting Liu, Yanqin Jiang, Nian Liu, Jingmen Zhou, Zhengjun Zha, Weiming Hu, Jin Gao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.25344v1.pdf)  
  Keywords: body motion, efficient, dit, 4d generation, trajectory, temporal consistency  
- **[OmniDrive: An LLM-Choreographed Multi-Agent World Model with Unified Latent Co-Compression for Multi-View Driving Video Generation](https://arxiv.org/abs/2606.17536v1)**  
  Authors: Zijie Meng, Yufei Liu, Chengqian Ma, Zhiyu Li, Jiyuan Liu, Wenhua Nie, Bingcai Wei, Shuqin Chen, Weichen Xu, Jiquan Yuan, Miao Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17536v1.pdf)  
  Keywords: layout, world model, controllable, dit, autonomous driving, multi-view video, video generation  
- **[R2RDreamer: 3D-aware Data Augmentation for Spatially-generalized 2D Manipulation Policies](https://arxiv.org/abs/2606.17040v1)**  
  Authors: Xiuwei Xu, Haowen Sun, Angyuan Ma, Yiwei Zhang, Zhenyu Wu, Xiaofeng Wang, Bingyao Yu, Zheng Zhu, Jie Zhou, Jiwen Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17040v1.pdf)  
  Keywords: video completion, controllable, image-to-video, simulation, dit, style, 3d-aware  

### Applications

- **[Cyclone: Diffusion Model for Cycle-Consistent Weather Editing from Unpaired Driving Data](https://arxiv.org/abs/2607.13927v1)**  
  Authors: Thang-Anh-Quan Nguyen, Moussab Bennehar, Luis Guillermo Roldao Jimenez, Nathan Piasco, Dzmitry Tsishkou, Laurent Caraffa, Jean-Philippe Tarel, Roland Brémond  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.13927v1.pdf)  
  Keywords: dit, video diffusion, physics, autonomous driving, diffusion model  
- **[ABot-3DWorld 0: A Universal World Model to Explore Any 3D Space](https://arxiv.org/abs/2607.11673v2)**  
  Authors: Mingchao Sun, Luyang Tang, Yu Liu, Xu Yan, Zhan Li, Yunwei Zhang, Fei Yu, Zengye Ge, Yumin Liu, Jiacheng Zhang, Yongchang Zhang, Jiawei Zhang, Zhicheng Liu, Zhongxu Sun, Tianjian Ouyang, Wenzheng Chen, Shixing Yang, Nianfei Fan, Guodong Sun, Huan Li, Zheng Zhou, Yongze Li, Yingliang Peng, Mengmeng Du, Yuan Liu, Haozhe Shi, Chunnuo Gong, Chengzhen Yu, Chunxue Jia, Yang Liu, Shiying Zeng, Junnan Lai, Hang Zhang, Ning Guo, Baoquan Chen, Mu Xu, Hongyu Pan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.11673v2.pdf)  
  Keywords: efficient, trajectory, world model, creative  
- **[Xiaomi-Robotics-U0: Unified Embodied Synthesis with World Foundation Model](https://arxiv.org/abs/2607.11643v1)**  
  Authors: Xinghang Li, Jun Guo, Qiwei Li, Long Qian, Hang Lai, Yueze Wang, Hongyu Yan, Jiahang Cao, Xi Chen, Jingen Qu, Jiaxi Song, Nan Sun, Hanye Zhao, Futeng Liu, Wanli Peng, Heyun Wang, Yunhong Wang, Caoyu Xia, Jack Zhao, Diyun Xiang, Hangjun Ye, Heng Qu, Huaping Liu, Jason Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.11643v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://robotics.xiaomi.com/xiaomi-robotics-u0.html)  
  Keywords: world model, controllable, autoregressive, dynamics, dit, evaluation, video generation, robotics  
- **[Validate the Dream Before You Trust Its Verdict: Admissibility for World-Model Simulators](https://arxiv.org/abs/2607.07196v1)**  
  Authors: Christian Oefinger, Finn Rasmus Schäfer, Korbinian Moller, Mattia Piccinini, Johannes Betz  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.07196v1.pdf)  
  Keywords: world model, simulation, dit, autonomous driving, robotics  
- **[Point as Skeleton: Accumulated Point Cloud Enhanced Autoregressive Generation for Closed-Loop Autonomous Driving Simulation](https://arxiv.org/abs/2607.06516v1)**  
  Authors: Songbur Wong, Xiaosong Jia, Junqi You, Bo Zhang, Pei Xu, Renqiu Xia, Yuping Qiu, Shaofeng Zhang, Zelin Zhao, Xuechao Yan, Yuchen Zhou, Yurui Chen, Wen Guo, Hang Xu, Junchi Yan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.06516v1.pdf) | [![GitHub](https://img.shields.io/github/stars/krauwu/point-as-skeleton?style=social)](https://github.com/krauwu/point-as-skeleton)  
  Keywords: autoregressive, simulation, dit, autonomous driving, video generation  
- **[A Definition and Roadmap for World Models](https://arxiv.org/abs/2607.06401v1)**  
  Authors: Xinyuan Chen, Haoyu Guo, Shi Guo, Bingqi Jiang, Chunhua Shen, Xing Shen, Tianfan Xue, Yufei Xue, Mulin Yu, Weinan Zhang, Bin Zhao, Bowen Zhou, Ming Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.06401v1.pdf)  
  Keywords: physical, world model, dynamics, concept, video generation, robotics  
- **[Benchmarking the Robustness of Autonomous Driving to Environmental Illusions: A Lane Perception Perspective](https://arxiv.org/abs/2607.05783v1)**  
  Authors: Tianyuan Zhang, Xianglong Liu, Aishan Liu, Lu Wang, Yitong Zhang, Peng Yue, Mingchuan Zhang, Siyuan Liang, Dacheng Tao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.05783v1.pdf)  
  Keywords: controllable, simulation, dit, autonomous driving, benchmark, evaluation  
- **[SpheRoPE: Zero-Shot Optimization-Free 360 Panorama Generation with Spherical RoPE](https://arxiv.org/abs/2606.32033v1)**  
  Authors: Or Hirschorn, Aaron Olender, Eli Alshan, Ianir Ideses, Lior Fritz, Sagie Benaim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.32033v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://orhir.github.io/SpheRoPE)  
  Keywords: creative, diffusion transformer  
- **[World Narrative Model for Highly Controllable Video Generation: A Paradigm Shift from Pixel Sampling to Physical World Orchestration](https://arxiv.org/abs/2606.31946v2)**  
  Authors: Ye Chen, Xuanhong Chen, Yupeng Zhu, Liming Tan, Zhewen Wan, Yuxuan Xiong, Tielong Wang, Jinfan Liu, Wuze Zhang, Xiongzhen Zhang, Feifei Li, Xianglin Luo, Zhehan Zhao, Zhifan Zhang, Laisheng Kou, Zhujin Liang, Yugang Chen, Muchun Chen, Xu Miao, Yijing Zhang, Xiaojie Sheng, Qiang Hu, Jialiang Chen, Weimin Zhang, Wenjun Zhang, Bingbing Ni  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.31946v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://glassroom.sjtu.edu.cn/WNM)  
  Keywords: physical, layout, controllable, film, efficient, dit, video generation  
- **[InfiniVerse: Occupancy Guided Unbounded Scene Generation for Autonomous Driving](https://arxiv.org/abs/2606.31109v1)**  
  Authors: Xiaoyu Ye, Leheng Li, Xinyu Ji, Yingjie Cai, Hongda He, Xu Yan, Guanyi Zhao, Ying-Cong Chen, Bingbing Liu, Shuguang Cui, Zhen Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.31109v1.pdf)  
  Keywords: controllable, autoregressive, video diffusion, dit, autonomous driving, benchmark, evaluation, diffusion model  

### Architecture & Efficiency

*Showing the latest 50 out of 363 papers*

- **[VideoRAE: Taming Video Foundation Models for Generative Modeling via Representation Autoencoders](https://arxiv.org/abs/2607.14088v1)**  
  Authors: Zhihao Xie, Junfeng Wu, Xinting Hu, Junchao Huang, Li Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.14088v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://zhxie0117.github.io/VideoRAE)  
  Keywords: text-to-video, dit, diffusion transformer, autoregressive  
- **[From Pixels to States: Rethinking Interactive World Models as Game Engines](https://arxiv.org/abs/2607.14076v1)**  
  Authors: Zhen Li, Zian Meng, Shuwei Shi, Mingliang Zhai, Jiaming Tan, Chuanhao Li, Kaipeng Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.14076v1.pdf)  
  Keywords: interactive, world model, dit, dynamics  
- **[Cyclone: Diffusion Model for Cycle-Consistent Weather Editing from Unpaired Driving Data](https://arxiv.org/abs/2607.13927v1)**  
  Authors: Thang-Anh-Quan Nguyen, Moussab Bennehar, Luis Guillermo Roldao Jimenez, Nathan Piasco, Dzmitry Tsishkou, Laurent Caraffa, Jean-Philippe Tarel, Roland Brémond  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.13927v1.pdf)  
  Keywords: dit, video diffusion, physics, autonomous driving, diffusion model  
- **[Kaleido: Algorithm-Hardware Co-Design for Video Diffusion Transformers by Exploiting Latent Space Correlations](https://arxiv.org/abs/2607.13770v1)**  
  Authors: Wenxuan Miao, Haosong Liu, Weiming Hu, Zihan Liu, Aiyue Chen, Jianlin Yu, Yiwu Yao, Yiming Gan, Jieru Zhao, Jingwen Leng, Minyi Guo, Yu Feng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.13770v1.pdf)  
  Keywords: efficient, acceleration, video diffusion, dit, evaluation, diffusion transformer  
- **[VGIF-Score: Interpretable and Diagnostic Evaluation of Spatio-Temporal Instruction Following in Video Generation](https://arxiv.org/abs/2607.13527v1)**  
  Authors: Songyu Xu, Xin Wang, Qiang Chen, Xinran Wang, Muxi Diao, Yuxuan Zhang, Kongming Liang, Rui Lin, Zhanyu Ma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.13527v1.pdf) | [![GitHub](https://img.shields.io/github/stars/PRIS-CV/VGIF-SCORE?style=social)](https://github.com/PRIS-CV/VGIF-SCORE)  
  Keywords: dit, physics, benchmark, evaluation, video generation  
- **[Bring Music The Horizon: Music-Driven 360$^\circ$ Video Generation](https://arxiv.org/abs/2607.13471v1)**  
  Authors: Kai Hsu Tsai, Yong Wei Fu, Hung I Yang, Yu-Chih Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.13471v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://etoile-et-toi-mp3.github.io/BMTH_Project_Page)  
  Keywords: sound, image-to-video, dynamics, dit, music video, trajectory, video generation  
- **[Delving into the Temporal Challenges of Unified Video Protection Against Image-to-Video and Fine-Tuning-based Customization](https://arxiv.org/abs/2607.13336v1)**  
  Authors: Yuxin Huang, Ziming Hong, Mingming Gong, Wanyu Wang, Jing Zhang, Tongliang Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.13336v1.pdf)  
  Keywords: identity, image-to-video, dit, video diffusion, 3d video, video generation, customization, diffusion model  
- **[Continuously Evolving Deepfake Detection: An Architecture and Public-Benchmark Evaluation of a Dynamic Detection System](https://arxiv.org/abs/2607.13234v1)**  
  Authors: Ken Jon Miyachi, Dylan Uys  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.13234v1.pdf)  
  Keywords: dit, benchmark, evaluation, architecture  
- **[Text2Sign: A Single-GPU Diffusion Baseline for Text-to-Sign Language Video Generation](https://arxiv.org/abs/2607.13164v1)**  
  Authors: Ruize Xia  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.13164v1.pdf) | [![GitHub](https://img.shields.io/github/stars/xiaruize0911/text2sign?style=social)](https://github.com/xiaruize0911/text2sign)  
  Keywords: video diffusion, dit, style, evaluation, denoising, temporal consistency, video generation, diffusion model  
- **[ACID: Adaptive Caching for vIDeo generation](https://arxiv.org/abs/2607.12358v1)**  
  Authors: Om Agrawal, Saurabh Agarwal, Aditya Akella  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.12358v1.pdf)  
  Keywords: acceleration, video diffusion, dit, denoising, evaluation, video generation, diffusion model  

### Audio & Multi-modal

- **[Bring Music The Horizon: Music-Driven 360$^\circ$ Video Generation](https://arxiv.org/abs/2607.13471v1)**  
  Authors: Kai Hsu Tsai, Yong Wei Fu, Hung I Yang, Yu-Chih Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.13471v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://etoile-et-toi-mp3.github.io/BMTH_Project_Page)  
  Keywords: sound, image-to-video, dynamics, dit, music video, trajectory, video generation  
- **[HumanForge: A Human-Centric Deepfake Video Benchmark with Multi-Agent Forgery Rationales](https://arxiv.org/abs/2607.08705v1)**  
  Authors: Wenbo Xu, Zhimin Chen, Xiaojie Liang, Hengrui Liu, Wei Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.08705v1.pdf)  
  Keywords: multi-modal, text-to-video, video diffusion, dit, benchmark, video synthesis, diffusion model  
- **[AVTok: 1D Unified Tokenization for Holistic Audio-Video Generation](https://arxiv.org/abs/2606.30811v1)**  
  Authors: Kien T. Pham, I Chieh Chen, Qifeng Chen, Long Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.30811v1.pdf)  
  Keywords: sound, efficient, audio-to-video, dit, architecture, video generation  
- **[TRUST: Efficient Abdominal Trauma Recognition via Image-to-Ultrasound-Video Transfer Learning](https://arxiv.org/abs/2606.27777v1)**  
  Authors: Enguang Wang, Hao Zhou, Shuo Gao, Tuo Liu, Guangquan Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.27777v1.pdf)  
  Keywords: sound, dynamics, efficient, image-to-video, dit  
- **[PhyEditBench: A Real-World Multi-Stage Benchmark for Physics-Aware Image Editing](https://arxiv.org/abs/2606.26551v2)**  
  Authors: Shengbin Guo, Shaokang He, Chaoyue Meng, Shengpeng Xiao, Xunzhi Xiang, Shaofeng Zhang, Qi Fan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.26551v2.pdf) | [![GitHub](https://img.shields.io/github/stars/Previsior/PhyEditBench?style=social)](https://github.com/Previsior/PhyEditBench)  
  Keywords: multi-modal, physical, physics-aware, dynamics, dit, physics, benchmark, evaluation, video generation  
- **[Wan-Streamer v0.1: End-to-end Real-time Interactive Foundation Models](https://arxiv.org/abs/2606.25041v3)**  
  Authors: Lianghua Huang, Zhi-Fan Wu, Wei Wang, Yupeng Shi, Mengyang Feng, Junjie He, Chen-Wei Xie, Yu Liu, Jingren Zhou, Ang Wang, Bang Zhang, Baole Ai, Chen Liang, Cheng Yu, Chongyang Zhong, Jinwei Qi, Kai Zhu, Pandeng Li, Peng Zhang, Wenyuan Zhang, Xinhua Cheng, Yitong Huang, Yun Zheng, Yuzheng Wang, Zoubin Bi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.25041v3.pdf)  
  Keywords: audio-driven, interactive, streaming, avatar  
- **[InteractiveAvatar: Real-Time Streaming Video Generation for Consistent and Intent-Aware Avatars](https://arxiv.org/abs/2606.22905v2)**  
  Authors: Quanyue Song, Yishan He, Yanfei Zhang, Shihao Cheng, Zhixiang He, Zhizhi Guo, Chi Zhang, Xuelong Li, Caigui Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.22905v2.pdf)  
  Keywords: distillation, avatar, autoregressive, interactive, streaming, temporal consistency, video generation, audio-driven  
- **[T-MOR: Learning Motion-Aware Skeleton Representations for Human Action Recognition](https://arxiv.org/abs/2606.21607v1)**  
  Authors: Di Yang, Mahmoud Ali, Quan Kong, Gianpiero Francesca, Francois Bremond  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.21607v1.pdf)  
  Keywords: physical, multi-modal, dit, benchmark, human motion  
- **[PermaVid: Consistent Video Generation Across Edits via Disentangled Context Memory](https://arxiv.org/abs/2606.16449v2)**  
  Authors: Shuai Yang, Bingjie Gao, Ziwei Liu, Jiaqi Wang, Dahua Lin, Tong Wu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16449v2.pdf)  
  Keywords: multi-modal, layout, dit, video generation  
- **[ReFree: Towards Realistic Co-Speech Video Generation via Reward-Free RL and Multilevel Speech Guidance](https://arxiv.org/abs/2606.13304v1)**  
  Authors: Salaheldin Mohamed, M. Hamza Mughal, Rishabh Dabral, Christian Theobalt  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13304v1.pdf)  
  Keywords: evaluation, speech-driven, video generation  

### Controllable Generation

*Showing the latest 50 out of 138 papers*

- **[Bring Music The Horizon: Music-Driven 360$^\circ$ Video Generation](https://arxiv.org/abs/2607.13471v1)**  
  Authors: Kai Hsu Tsai, Yong Wei Fu, Hung I Yang, Yu-Chih Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.13471v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://etoile-et-toi-mp3.github.io/BMTH_Project_Page)  
  Keywords: sound, image-to-video, dynamics, dit, music video, trajectory, video generation  
- **[FlowWAM: Optical Flow as a Unified Action Representation for World Action Models](https://arxiv.org/abs/2607.13017v1)**  
  Authors: Yixiang Chen, Peiyan Li, Yuan Xu, Qisen Ma, Jiabing Yang, Kai Wang, Jianhua Yang, Dong An, He Guan, Gaoteng Liu, Jianlou Si, Jun Huang, Jing Liu, Nianfeng Liu, Yan Huang, Liang Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.13017v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://flow-wam.github.io)  
  Keywords: trajectory, world model, video generation  
- **[ABot-3DWorld 0: A Universal World Model to Explore Any 3D Space](https://arxiv.org/abs/2607.11673v2)**  
  Authors: Mingchao Sun, Luyang Tang, Yu Liu, Xu Yan, Zhan Li, Yunwei Zhang, Fei Yu, Zengye Ge, Yumin Liu, Jiacheng Zhang, Yongchang Zhang, Jiawei Zhang, Zhicheng Liu, Zhongxu Sun, Tianjian Ouyang, Wenzheng Chen, Shixing Yang, Nianfei Fan, Guodong Sun, Huan Li, Zheng Zhou, Yongze Li, Yingliang Peng, Mengmeng Du, Yuan Liu, Haozhe Shi, Chunnuo Gong, Chengzhen Yu, Chunxue Jia, Yang Liu, Shiying Zeng, Junnan Lai, Hang Zhang, Ning Guo, Baoquan Chen, Mu Xu, Hongyu Pan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.11673v2.pdf)  
  Keywords: efficient, trajectory, world model, creative  
- **[Xiaomi-Robotics-U0: Unified Embodied Synthesis with World Foundation Model](https://arxiv.org/abs/2607.11643v1)**  
  Authors: Xinghang Li, Jun Guo, Qiwei Li, Long Qian, Hang Lai, Yueze Wang, Hongyu Yan, Jiahang Cao, Xi Chen, Jingen Qu, Jiaxi Song, Nan Sun, Hanye Zhao, Futeng Liu, Wanli Peng, Heyun Wang, Yunhong Wang, Caoyu Xia, Jack Zhao, Diyun Xiang, Hangjun Ye, Heng Qu, Huaping Liu, Jason Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.11643v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://robotics.xiaomi.com/xiaomi-robotics-u0.html)  
  Keywords: world model, controllable, autoregressive, dynamics, dit, evaluation, video generation, robotics  
- **[Controlling Motion Transfer in Diffusion Transformers via Attention Heads](https://arxiv.org/abs/2607.11081v1)**  
  Authors: Sunyoung Jung, Jiwoo Park, Yoonseok Choi, Kyobin Choo, Ming-Hsuan Yang, Seong Jae Hwang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.11081v1.pdf)  
  Keywords: dit, controllable, diffusion transformer, video generation  
- **[Is Energy Guidance All You Need? Training-Free Norm Injection for Driving World Models](https://arxiv.org/abs/2607.10781v1)**  
  Authors: Xiyan Su, Frank Diermeyer, Markus Lienkamp  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.10781v1.pdf)  
  Keywords: layout, world model, controllable, dit, trajectory  
- **[GenVid2Robot: From Video Generation to Robot Manipulation via Rigid-Geometric Consistency](https://arxiv.org/abs/2607.09191v1)**  
  Authors: Haohui Huang, Xi Yuan, Panpan Liao, Tao Teng, Chenguang Yang, Jing Guo, Yi Guo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.09191v1.pdf)  
  Keywords: physical, trajectory, dit, video generation  
- **[4D Human-Scene Reconstruction from Low-Overlap Captures](https://arxiv.org/abs/2607.09125v1)**  
  Authors: Minhyuk Hwang, Sangmin Kim, Seunguk Do, Daneul Kim, Jaesik Park  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.09125v1.pdf)  
  Keywords: identity, novel view, video diffusion, trajectory, diffusion model  
- **[OPSD-V: On-Policy Self-Distillation for Post-Training Few-Step Autoregressive Video Generators](https://arxiv.org/abs/2607.08766v1)**  
  Authors: Hongyu Liu, Chun Wang, Feng Gao, Xuanhua He, Yue Ma, Ziyu Wan, Yong Zhang, Xiaoming Wei, Qifeng Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.08766v1.pdf)  
  Keywords: long video, distillation, autoregressive, dynamics, video diffusion, dit, denoising, trajectory, diffusion model  
- **[LightCrafter: PBR-Conditioned Video Diffusion Refinement for Controllable and Consistent Relighting](https://arxiv.org/abs/2607.08016v2)**  
  Authors: Zixin Guo, Yehonathan Litman, Yifeng He, John Miller, Chuhan Chen, Deva Ramanan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.08016v2.pdf)  
  Keywords: physical, controllable, video translation, video diffusion, dit, long-form, concept, benchmark, video-to-video, temporal consistency, video generation, diffusion model  

### Human & Character Animation

- **[Wan-Dancer: A Hierarchical Framework for Minute-scale Coherent Music-to-Dance Generation](https://arxiv.org/abs/2607.09581v2)**  
  Authors: Mingyang Huang, Peng Zhang, Li Hu, Guangyuan Wang, Bang Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.09581v2.pdf)  
  Keywords: identity, dit, long-form, video synthesis, diffusion model, dance generation  
- **[Behavior Foundations for Quadruped Robots: ABot-C0 Technical Report](https://arxiv.org/abs/2607.07370v2)**  
  Authors: Xufeng Zhao, Fuzhi Yang, Jianhui Chen, Li Gao, Zhang Meng, Jie Gao, Yao Zheng, Congyang Zhao, Tianxiong Lv, Menglin Yang, Minqi Gu, Yaru Zhao, Wenyu Liu, Honglin Han, Shihui Su, Zixiao Tang, Liu Liu, Mu Xu, Yang Cai, Wenbin Tang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.07370v2.pdf)  
  Keywords: physical, efficient, motion control, dit, style, human motion  
- **[ProxyPose: 6-DoF Pose Tracking via Video-to-Video Translation](https://arxiv.org/abs/2607.06555v1)**  
  Authors: Ruihang Zhang, Felix Taubner, Pooja Ravi, Kiriakos N. Kutulakos, David B. Lindell  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.06555v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://ruihangzhang97.github.io/proxypose)  
  Keywords: identity, video translation, body motion, video diffusion, dit, trajectory, video-to-video, diffusion model  
- **[VendorBench-100: A Unified Cross-Paradigm Benchmark for Deepfake Image Detection](https://arxiv.org/abs/2607.06254v1)**  
  Authors: Sharayu N. Deshmukh, Md Rashidunnabi, Nelton Tiago Gemo, Kurundkar G. D., Mahamune M. R., Nilesh K. Deshmukh  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.06254v1.pdf) | [![GitHub](https://img.shields.io/github/stars/sharayu-20/vendorbench-100?style=social)](https://github.com/sharayu-20/vendorbench-100)  
  Keywords: avatar, text-to-video, efficient, dit, benchmark, evaluation  
- **[3D Scene-Adaptive Trajectory-Controllable Human Image Animation with Camera Movement](https://arxiv.org/abs/2606.30514v2)**  
  Authors: Deyin Liu, Jicheng Xu, Lin Yuanbo Wu, Xiaowei Zhao, Xiatian Zhu, Zhe Jin, Anjan Dutta  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.30514v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://robinhood256100.github.io/web-disp)  
  Keywords: controllable, camera control, dit, benchmark, trajectory, human motion, image animation, video generation  
- **[OmniDance: Multimodal Driven Dance Video Generation with Large-scale Internet Data](https://arxiv.org/abs/2606.30019v1)**  
  Authors: Kaixing Yang, Jiashu Zhu, Xulong Tang, Ziqiao Peng, Xiangyue Zhang, Chubin Chen, Puwei Wang, Jiahong Wu, Xiangxiang Chu, Hongyan Liu, Jun He  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.30019v1.pdf) | [![GitHub](https://img.shields.io/github/stars/AMAP-ML/OmniDance?style=social)](https://github.com/AMAP-ML/OmniDance)  
  Keywords: i2v, dynamics, dit, architecture, human motion, video generation  
- **[EMOSH: Expressive Motion and Shape Disentanglement for Human Animation](https://arxiv.org/abs/2606.28026v1)**  
  Authors: Dongbin Zhang, Hao Liu, Binquan Dai, Kangjie Chen, Chuming Wang, Chen Li, Jing Lyu, Haoqian Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.28026v1.pdf)  
  Keywords: avatar, controllable, identity, human animation, dit, gesture, video generation  
- **[Directing the World: Fast Autoregressive Video Generation with Compositional Human-Camera Control](https://arxiv.org/abs/2606.27964v1)**  
  Authors: Haoyuan Wang, Yabo Chen, Haibin Huang, Chi Zhang, Xuelong Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.27964v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://whydahuzi.github.io/Directing-the-World.github.io)  
  Keywords: world model, controllable, camera control, autoregressive, dynamics, motion control, trajectory, interactive, human motion, video generation  
- **[Follow Your Track: Precise Skeleton Animation Controlled by 3D Trajectories](https://arxiv.org/abs/2606.25344v1)**  
  Authors: Yueting Liu, Yanqin Jiang, Nian Liu, Jingmen Zhou, Zhengjun Zha, Weiming Hu, Jin Gao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.25344v1.pdf)  
  Keywords: body motion, efficient, dit, 4d generation, trajectory, temporal consistency  
- **[Wan-Streamer v0.1: End-to-end Real-time Interactive Foundation Models](https://arxiv.org/abs/2606.25041v3)**  
  Authors: Lianghua Huang, Zhi-Fan Wu, Wei Wang, Yupeng Shi, Mengyang Feng, Junjie He, Chen-Wei Xie, Yu Liu, Jingren Zhou, Ang Wang, Bang Zhang, Baole Ai, Chen Liang, Cheng Yu, Chongyang Zhong, Jinwei Qi, Kai Zhu, Pandeng Li, Peng Zhang, Wenyuan Zhang, Xinhua Cheng, Yitong Huang, Yun Zheng, Yuzheng Wang, Zoubin Bi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.25041v3.pdf)  
  Keywords: audio-driven, interactive, streaming, avatar  

### Image-to-Video Generation

- **[Bring Music The Horizon: Music-Driven 360$^\circ$ Video Generation](https://arxiv.org/abs/2607.13471v1)**  
  Authors: Kai Hsu Tsai, Yong Wei Fu, Hung I Yang, Yu-Chih Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.13471v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://etoile-et-toi-mp3.github.io/BMTH_Project_Page)  
  Keywords: sound, image-to-video, dynamics, dit, music video, trajectory, video generation  
- **[Delving into the Temporal Challenges of Unified Video Protection Against Image-to-Video and Fine-Tuning-based Customization](https://arxiv.org/abs/2607.13336v1)**  
  Authors: Yuxin Huang, Ziming Hong, Mingming Gong, Wanyu Wang, Jing Zhang, Tongliang Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.13336v1.pdf)  
  Keywords: identity, image-to-video, dit, video diffusion, 3d video, video generation, customization, diffusion model  
- **[AU-Guided Synthetic Video Generation for Micro-Expression Recognition](https://arxiv.org/abs/2607.10860v1)**  
  Authors: Pei-Sze Tan, Sailaja Rajanala, Yee-Fan Tan, Raphael C. -W. Phan, Huey-Fang Ong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.10860v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://kirito-blade.github.io/me-vlm)  
  Keywords: image-to-video, architecture, dit, video generation  
- **[OpenCoF: Learning to Reason Through Video Generation](https://arxiv.org/abs/2607.08763v1)**  
  Authors: Xinyan Chen, Ziyu Guo, Renrui Zhang, Dongzhi Jiang, Hongsheng Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.08763v1.pdf)  
  Keywords: benchmark, denoising, i2v, video generation  
- **[CineMobile: On-Device Image-to-Video Diffusion for Cinematic Camera Motion Generation](https://arxiv.org/abs/2607.03803v1)**  
  Authors: Xuyao Huang, Zelai Deng, Xu Wang, Xizhong Xiao, Zhijie Deng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.03803v1.pdf)  
  Keywords: distillation, image-to-video, efficient, video diffusion, dit, architecture, denoising, video generation, diffusion transformer  
- **[OrbitQuant: Data-Agnostic Quantization for Image and Video Diffusion Transformers](https://arxiv.org/abs/2607.02461v1)**  
  Authors: Donghyun Lee, Jitesh Chavan, Duy Nguyen, Sam Huang, Liming Jiang, Priyadarshini Panda, Timo Mertens, Saurabh Shukla  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.02461v1.pdf)  
  Keywords: dit, video diffusion, image to video, video generation, diffusion transformer  
- **[QWERTY: Training-Free Motion Control via Query-Warped Video Diffusion Transformers](https://arxiv.org/abs/2607.01869v1)**  
  Authors: Kyobin Choo, Youngmin Kim, Hyunkyung Han, Geunrip Park, Chanyoung Kim, Sunyoung Jung, Seong Jae Hwang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.01869v1.pdf)  
  Keywords: image-to-video, motion control, video diffusion, dit, trajectory, diffusion transformer, diffusion model  
- **[Anti-Prompt: Image Protection against Text-Guided Image-to-Video Generation](https://arxiv.org/abs/2607.01499v2)**  
  Authors: Yeonghwan Song, Chanhui Lee, Jinsoo Park, Jeany Son  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.01499v2.pdf)  
  Keywords: i2v, image-to-video, dit, architecture, evaluation, denoising, temporal consistency, video generation  
- **[TrajLoc: Trajectory-Attention Localization for Multi-Object Motion Control](https://arxiv.org/abs/2607.00861v1)**  
  Authors: Omer Sela, Inbar Huberman-Spiegelglas, Michael Rotman, Sagie Benaim, Avi Ben-Cohen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.00861v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://sela-omer.github.io/traj-loc)  
  Keywords: i2v, identity, image-to-video, motion control, dit, evaluation, trajectory  
- **[3D Scene-Adaptive Trajectory-Controllable Human Image Animation with Camera Movement](https://arxiv.org/abs/2606.30514v2)**  
  Authors: Deyin Liu, Jicheng Xu, Lin Yuanbo Wu, Xiaowei Zhao, Xiatian Zhu, Zhe Jin, Anjan Dutta  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.30514v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://robinhood256100.github.io/web-disp)  
  Keywords: controllable, camera control, dit, benchmark, trajectory, human motion, image animation, video generation  

### Long Video Generation

*Showing the latest 50 out of 126 papers*

- **[VideoRAE: Taming Video Foundation Models for Generative Modeling via Representation Autoencoders](https://arxiv.org/abs/2607.14088v1)**  
  Authors: Zhihao Xie, Junfeng Wu, Xinting Hu, Junchao Huang, Li Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.14088v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://zhxie0117.github.io/VideoRAE)  
  Keywords: text-to-video, dit, diffusion transformer, autoregressive  
- **[Text2Sign: A Single-GPU Diffusion Baseline for Text-to-Sign Language Video Generation](https://arxiv.org/abs/2607.13164v1)**  
  Authors: Ruize Xia  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.13164v1.pdf) | [![GitHub](https://img.shields.io/github/stars/xiaruize0911/text2sign?style=social)](https://github.com/xiaruize0911/text2sign)  
  Keywords: video diffusion, dit, style, evaluation, denoising, temporal consistency, video generation, diffusion model  
- **[The Seriality Gap in Video Diffusion Models](https://arxiv.org/abs/2607.13031v1)**  
  Authors: Jorge Diaz Chao, Konpat Preechakul, Yuxi Liu, Yutong Bai  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.13031v1.pdf)  
  Keywords: autoregressive, dynamics, simulation, video diffusion, denoising, video prediction, diffusion model  
- **[WanToFight: Real-Time Generative Game Engine for Multi-Player Combat Interaction](https://arxiv.org/abs/2607.12592v1)**  
  Authors: Li Hu, Guangyuan Wang, Peng Zhang, Bang Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.12592v1.pdf)  
  Keywords: physical, identity, autoregressive, video diffusion, streaming, diffusion transformer  
- **[Cycle-World: Mitigating Error Accumulation in Long-term Video World Models via Reverse-Prediction Cycle Consistency](https://arxiv.org/abs/2607.11836v1)**  
  Authors: Zihan Su, Teng Hu, Jiangning Zhang, Ruiyan Wang, Ran Yi, Lizhuang Ma, Dacheng Tao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.11836v1.pdf)  
  Keywords: world model, autoregressive, efficient, benchmark, video synthesis, temporal consistency, video generation, diffusion model  
- **[Xiaomi-Robotics-U0: Unified Embodied Synthesis with World Foundation Model](https://arxiv.org/abs/2607.11643v1)**  
  Authors: Xinghang Li, Jun Guo, Qiwei Li, Long Qian, Hang Lai, Yueze Wang, Hongyu Yan, Jiahang Cao, Xi Chen, Jingen Qu, Jiaxi Song, Nan Sun, Hanye Zhao, Futeng Liu, Wanli Peng, Heyun Wang, Yunhong Wang, Caoyu Xia, Jack Zhao, Diyun Xiang, Hangjun Ye, Heng Qu, Huaping Liu, Jason Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.11643v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://robotics.xiaomi.com/xiaomi-robotics-u0.html)  
  Keywords: world model, controllable, autoregressive, dynamics, dit, evaluation, video generation, robotics  
- **[Wan-Dancer: A Hierarchical Framework for Minute-scale Coherent Music-to-Dance Generation](https://arxiv.org/abs/2607.09581v2)**  
  Authors: Mingyang Huang, Peng Zhang, Li Hu, Guangyuan Wang, Bang Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.09581v2.pdf)  
  Keywords: identity, dit, long-form, video synthesis, diffusion model, dance generation  
- **[LongE2V: Long-Horizon Event-based Video Reconstruction, Prediction, and Frame Interpolation with Video Diffusion Models](https://arxiv.org/abs/2607.08770v1)**  
  Authors: Cheng-De Fan, Chun-Wei Tuan Mu, Chen-Wei Chang, Chin-Yang Lin, Kun-Ru Wu, Yu-Chee Tseng, Yu-Lun Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.08770v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://cdfan0627.github.io/LongE2V-page)  
  Keywords: autoregressive, video diffusion, frame interpolation, benchmark, diffusion model  
- **[OPSD-V: On-Policy Self-Distillation for Post-Training Few-Step Autoregressive Video Generators](https://arxiv.org/abs/2607.08766v1)**  
  Authors: Hongyu Liu, Chun Wang, Feng Gao, Xuanhua He, Yue Ma, Ziyu Wan, Yong Zhang, Xiaoming Wei, Qifeng Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.08766v1.pdf)  
  Keywords: long video, distillation, autoregressive, dynamics, video diffusion, dit, denoising, trajectory, diffusion model  
- **[Spectral Origins of the Self-Correction Blind Spot in Autoregressive Generation](https://arxiv.org/abs/2607.09803v1)**  
  Authors: Ingrid Petrova, Luan Vejsiu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.09803v1.pdf)  
  Keywords: autoregressive, dit, video generation  

### Personalization & Customization

*Showing the latest 50 out of 94 papers*

- **[Delving into the Temporal Challenges of Unified Video Protection Against Image-to-Video and Fine-Tuning-based Customization](https://arxiv.org/abs/2607.13336v1)**  
  Authors: Yuxin Huang, Ziming Hong, Mingming Gong, Wanyu Wang, Jing Zhang, Tongliang Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.13336v1.pdf)  
  Keywords: identity, image-to-video, dit, video diffusion, 3d video, video generation, customization, diffusion model  
- **[Text2Sign: A Single-GPU Diffusion Baseline for Text-to-Sign Language Video Generation](https://arxiv.org/abs/2607.13164v1)**  
  Authors: Ruize Xia  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.13164v1.pdf) | [![GitHub](https://img.shields.io/github/stars/xiaruize0911/text2sign?style=social)](https://github.com/xiaruize0911/text2sign)  
  Keywords: video diffusion, dit, style, evaluation, denoising, temporal consistency, video generation, diffusion model  
- **[WanToFight: Real-Time Generative Game Engine for Multi-Player Combat Interaction](https://arxiv.org/abs/2607.12592v1)**  
  Authors: Li Hu, Guangyuan Wang, Peng Zhang, Bang Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.12592v1.pdf)  
  Keywords: physical, identity, autoregressive, video diffusion, streaming, diffusion transformer  
- **[SymbOmni: Evolving Agentic Omni Models via Symbolic Concept Learning](https://arxiv.org/abs/2607.12042v1)**  
  Authors: Jinxiu Liu, Jianru Li, Tanqing Kuang, Xuanming Liu, Kangfu Mei, Yandong Wen, Weiyang Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.12042v1.pdf)  
  Keywords: efficient, concept, benchmark, interactive, video synthesis  
- **[Wan-Dancer: A Hierarchical Framework for Minute-scale Coherent Music-to-Dance Generation](https://arxiv.org/abs/2607.09581v2)**  
  Authors: Mingyang Huang, Peng Zhang, Li Hu, Guangyuan Wang, Bang Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.09581v2.pdf)  
  Keywords: identity, dit, long-form, video synthesis, diffusion model, dance generation  
- **[Generative Communications: Overview, Technologies, and Trends](https://arxiv.org/abs/2607.09183v1)**  
  Authors: Wenjun Zhang, Zhiyong Chen, Tong Wu, Guo Lu, Li Song, Feng Yang, Meixia Tao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.09183v1.pdf)  
  Keywords: efficient, concept, dit, architecture  
- **[4D Human-Scene Reconstruction from Low-Overlap Captures](https://arxiv.org/abs/2607.09125v1)**  
  Authors: Minhyuk Hwang, Sangmin Kim, Seunguk Do, Daneul Kim, Jaesik Park  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.09125v1.pdf)  
  Keywords: identity, novel view, video diffusion, trajectory, diffusion model  
- **[Applying JEPA-Style Predictive Learning to JA4-Derived Network Fingerprints](https://arxiv.org/abs/2607.08465v1)**  
  Authors: Javier Izquierdo, Aygul Zagidullina  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.08465v1.pdf)  
  Keywords: style  
- **[LightCrafter: PBR-Conditioned Video Diffusion Refinement for Controllable and Consistent Relighting](https://arxiv.org/abs/2607.08016v2)**  
  Authors: Zixin Guo, Yehonathan Litman, Yifeng He, John Miller, Chuhan Chen, Deva Ramanan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.08016v2.pdf)  
  Keywords: physical, controllable, video translation, video diffusion, dit, long-form, concept, benchmark, video-to-video, temporal consistency, video generation, diffusion model  
- **[Behavior Foundations for Quadruped Robots: ABot-C0 Technical Report](https://arxiv.org/abs/2607.07370v2)**  
  Authors: Xufeng Zhao, Fuzhi Yang, Jianhui Chen, Li Gao, Zhang Meng, Jie Gao, Yao Zheng, Congyang Zhao, Tianxiong Lv, Menglin Yang, Minqi Gu, Yaru Zhao, Wenyu Liu, Honglin Han, Shihui Su, Zixiao Tang, Liu Liu, Mu Xu, Yang Cai, Wenbin Tang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.07370v2.pdf)  
  Keywords: physical, efficient, motion control, dit, style, human motion  

### Physical Understanding

*Showing the latest 50 out of 157 papers*

- **[From Pixels to States: Rethinking Interactive World Models as Game Engines](https://arxiv.org/abs/2607.14076v1)**  
  Authors: Zhen Li, Zian Meng, Shuwei Shi, Mingliang Zhai, Jiaming Tan, Chuanhao Li, Kaipeng Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.14076v1.pdf)  
  Keywords: interactive, world model, dit, dynamics  
- **[Cyclone: Diffusion Model for Cycle-Consistent Weather Editing from Unpaired Driving Data](https://arxiv.org/abs/2607.13927v1)**  
  Authors: Thang-Anh-Quan Nguyen, Moussab Bennehar, Luis Guillermo Roldao Jimenez, Nathan Piasco, Dzmitry Tsishkou, Laurent Caraffa, Jean-Philippe Tarel, Roland Brémond  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.13927v1.pdf)  
  Keywords: dit, video diffusion, physics, autonomous driving, diffusion model  
- **[VGIF-Score: Interpretable and Diagnostic Evaluation of Spatio-Temporal Instruction Following in Video Generation](https://arxiv.org/abs/2607.13527v1)**  
  Authors: Songyu Xu, Xin Wang, Qiang Chen, Xinran Wang, Muxi Diao, Yuxuan Zhang, Kongming Liang, Rui Lin, Zhanyu Ma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.13527v1.pdf) | [![GitHub](https://img.shields.io/github/stars/PRIS-CV/VGIF-SCORE?style=social)](https://github.com/PRIS-CV/VGIF-SCORE)  
  Keywords: dit, physics, benchmark, evaluation, video generation  
- **[Bring Music The Horizon: Music-Driven 360$^\circ$ Video Generation](https://arxiv.org/abs/2607.13471v1)**  
  Authors: Kai Hsu Tsai, Yong Wei Fu, Hung I Yang, Yu-Chih Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.13471v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://etoile-et-toi-mp3.github.io/BMTH_Project_Page)  
  Keywords: sound, image-to-video, dynamics, dit, music video, trajectory, video generation  
- **[The Seriality Gap in Video Diffusion Models](https://arxiv.org/abs/2607.13031v1)**  
  Authors: Jorge Diaz Chao, Konpat Preechakul, Yuxi Liu, Yutong Bai  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.13031v1.pdf)  
  Keywords: autoregressive, dynamics, simulation, video diffusion, denoising, video prediction, diffusion model  
- **[WanToFight: Real-Time Generative Game Engine for Multi-Player Combat Interaction](https://arxiv.org/abs/2607.12592v1)**  
  Authors: Li Hu, Guangyuan Wang, Peng Zhang, Bang Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.12592v1.pdf)  
  Keywords: physical, identity, autoregressive, video diffusion, streaming, diffusion transformer  
- **[Xiaomi-Robotics-U0: Unified Embodied Synthesis with World Foundation Model](https://arxiv.org/abs/2607.11643v1)**  
  Authors: Xinghang Li, Jun Guo, Qiwei Li, Long Qian, Hang Lai, Yueze Wang, Hongyu Yan, Jiahang Cao, Xi Chen, Jingen Qu, Jiaxi Song, Nan Sun, Hanye Zhao, Futeng Liu, Wanli Peng, Heyun Wang, Yunhong Wang, Caoyu Xia, Jack Zhao, Diyun Xiang, Hangjun Ye, Heng Qu, Huaping Liu, Jason Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.11643v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://robotics.xiaomi.com/xiaomi-robotics-u0.html)  
  Keywords: world model, controllable, autoregressive, dynamics, dit, evaluation, video generation, robotics  
- **[GenVid2Robot: From Video Generation to Robot Manipulation via Rigid-Geometric Consistency](https://arxiv.org/abs/2607.09191v1)**  
  Authors: Haohui Huang, Xi Yuan, Panpan Liao, Tao Teng, Chenguang Yang, Jing Guo, Yi Guo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.09191v1.pdf)  
  Keywords: physical, trajectory, dit, video generation  
- **[Video Generation Models are General-Purpose Vision Learners](https://arxiv.org/abs/2607.09024v1)**  
  Authors: Letian Wang, Chuhan Zhang, Rishabh Kabra, Jasper Uijlings, Steven Waslander, Andrew Zisserman, Joao Carreira, Kaiming He, Misha Andriluka, Eduard Gabriel Bazavan, Andrei Zanfir, Cristian Sminchisescu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.09024v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://genception.github.io)  
  Keywords: physical, text-to-video, video generation  
- **[OPSD-V: On-Policy Self-Distillation for Post-Training Few-Step Autoregressive Video Generators](https://arxiv.org/abs/2607.08766v1)**  
  Authors: Hongyu Liu, Chun Wang, Feng Gao, Xuanhua He, Yue Ma, Ziyu Wan, Yong Zhang, Xiaoming Wei, Qifeng Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.08766v1.pdf)  
  Keywords: long video, distillation, autoregressive, dynamics, video diffusion, dit, denoising, trajectory, diffusion model  

### Surveys & Benchmarks

*Showing the latest 50 out of 230 papers*

- **[Kaleido: Algorithm-Hardware Co-Design for Video Diffusion Transformers by Exploiting Latent Space Correlations](https://arxiv.org/abs/2607.13770v1)**  
  Authors: Wenxuan Miao, Haosong Liu, Weiming Hu, Zihan Liu, Aiyue Chen, Jianlin Yu, Yiwu Yao, Yiming Gan, Jieru Zhao, Jingwen Leng, Minyi Guo, Yu Feng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.13770v1.pdf)  
  Keywords: efficient, acceleration, video diffusion, dit, evaluation, diffusion transformer  
- **[VGIF-Score: Interpretable and Diagnostic Evaluation of Spatio-Temporal Instruction Following in Video Generation](https://arxiv.org/abs/2607.13527v1)**  
  Authors: Songyu Xu, Xin Wang, Qiang Chen, Xinran Wang, Muxi Diao, Yuxuan Zhang, Kongming Liang, Rui Lin, Zhanyu Ma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.13527v1.pdf) | [![GitHub](https://img.shields.io/github/stars/PRIS-CV/VGIF-SCORE?style=social)](https://github.com/PRIS-CV/VGIF-SCORE)  
  Keywords: dit, physics, benchmark, evaluation, video generation  
- **[Continuously Evolving Deepfake Detection: An Architecture and Public-Benchmark Evaluation of a Dynamic Detection System](https://arxiv.org/abs/2607.13234v1)**  
  Authors: Ken Jon Miyachi, Dylan Uys  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.13234v1.pdf)  
  Keywords: dit, benchmark, evaluation, architecture  
- **[Text2Sign: A Single-GPU Diffusion Baseline for Text-to-Sign Language Video Generation](https://arxiv.org/abs/2607.13164v1)**  
  Authors: Ruize Xia  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.13164v1.pdf) | [![GitHub](https://img.shields.io/github/stars/xiaruize0911/text2sign?style=social)](https://github.com/xiaruize0911/text2sign)  
  Keywords: video diffusion, dit, style, evaluation, denoising, temporal consistency, video generation, diffusion model  
- **[ACID: Adaptive Caching for vIDeo generation](https://arxiv.org/abs/2607.12358v1)**  
  Authors: Om Agrawal, Saurabh Agarwal, Aditya Akella  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.12358v1.pdf)  
  Keywords: acceleration, video diffusion, dit, denoising, evaluation, video generation, diffusion model  
- **[MobileSAM2: Lightweight Segment Anything for Spatial Intelligence](https://arxiv.org/abs/2607.12297v1)**  
  Authors: Kai Jiang, Jiaxing Huang, Jingyi Zhang, Weiying Xie, Yunsong Li, Yufei Wang, Aoran Xiao, Dacheng Tao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.12297v1.pdf)  
  Keywords: benchmark, distillation, architecture  
- **[SymbOmni: Evolving Agentic Omni Models via Symbolic Concept Learning](https://arxiv.org/abs/2607.12042v1)**  
  Authors: Jinxiu Liu, Jianru Li, Tanqing Kuang, Xuanming Liu, Kangfu Mei, Yandong Wen, Weiyang Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.12042v1.pdf)  
  Keywords: efficient, concept, benchmark, interactive, video synthesis  
- **[Cycle-World: Mitigating Error Accumulation in Long-term Video World Models via Reverse-Prediction Cycle Consistency](https://arxiv.org/abs/2607.11836v1)**  
  Authors: Zihan Su, Teng Hu, Jiangning Zhang, Ruiyan Wang, Ran Yi, Lizhuang Ma, Dacheng Tao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.11836v1.pdf)  
  Keywords: world model, autoregressive, efficient, benchmark, video synthesis, temporal consistency, video generation, diffusion model  
- **[Xiaomi-Robotics-U0: Unified Embodied Synthesis with World Foundation Model](https://arxiv.org/abs/2607.11643v1)**  
  Authors: Xinghang Li, Jun Guo, Qiwei Li, Long Qian, Hang Lai, Yueze Wang, Hongyu Yan, Jiahang Cao, Xi Chen, Jingen Qu, Jiaxi Song, Nan Sun, Hanye Zhao, Futeng Liu, Wanli Peng, Heyun Wang, Yunhong Wang, Caoyu Xia, Jack Zhao, Diyun Xiang, Hangjun Ye, Heng Qu, Huaping Liu, Jason Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.11643v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://robotics.xiaomi.com/xiaomi-robotics-u0.html)  
  Keywords: world model, controllable, autoregressive, dynamics, dit, evaluation, video generation, robotics  
- **[Prompting-MammAlps: Fine-Grained Text-to-Video Retrieval for Camera-Trap Data](https://arxiv.org/abs/2607.09876v1)**  
  Authors: Valentin Gabeff, Baptiste Maquignaz, Jennifer Shan, Sepideh Mamooler, Gencer Sumbul, Blair Costelloe, Devis Tuia, Alexander Mathis  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.09876v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://cnai.epfl.ch/prompting-mammalps)  
  Keywords: benchmark, text-to-video  

### Text-to-Video Generation

*Showing the latest 50 out of 74 papers*

- **[VideoRAE: Taming Video Foundation Models for Generative Modeling via Representation Autoencoders](https://arxiv.org/abs/2607.14088v1)**  
  Authors: Zhihao Xie, Junfeng Wu, Xinting Hu, Junchao Huang, Li Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.14088v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://zhxie0117.github.io/VideoRAE)  
  Keywords: text-to-video, dit, diffusion transformer, autoregressive  
- **[Prompting-MammAlps: Fine-Grained Text-to-Video Retrieval for Camera-Trap Data](https://arxiv.org/abs/2607.09876v1)**  
  Authors: Valentin Gabeff, Baptiste Maquignaz, Jennifer Shan, Sepideh Mamooler, Gencer Sumbul, Blair Costelloe, Devis Tuia, Alexander Mathis  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.09876v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://cnai.epfl.ch/prompting-mammalps)  
  Keywords: benchmark, text-to-video  
- **[Video Generation Models are General-Purpose Vision Learners](https://arxiv.org/abs/2607.09024v1)**  
  Authors: Letian Wang, Chuhan Zhang, Rishabh Kabra, Jasper Uijlings, Steven Waslander, Andrew Zisserman, Joao Carreira, Kaiming He, Misha Andriluka, Eduard Gabriel Bazavan, Andrei Zanfir, Cristian Sminchisescu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.09024v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://genception.github.io)  
  Keywords: physical, text-to-video, video generation  
- **[HumanForge: A Human-Centric Deepfake Video Benchmark with Multi-Agent Forgery Rationales](https://arxiv.org/abs/2607.08705v1)**  
  Authors: Wenbo Xu, Zhimin Chen, Xiaojie Liang, Hengrui Liu, Wei Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.08705v1.pdf)  
  Keywords: multi-modal, text-to-video, video diffusion, dit, benchmark, video synthesis, diffusion model  
- **[Prompt-Adapter Context Routing for Parameter-Efficient Multi-Shot Long Video Extrapolation](https://arxiv.org/abs/2607.06481v1)**  
  Authors: Anna Córdoba, Adam Puente Tercero, Nerea Angulo Hijo, Mar Linares Tercero, Julia Barrientos, Ainhoa Miranda, Jesús Olivera  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.06481v1.pdf)  
  Keywords: long video, text-to-video, controllable, identity, efficient, video diffusion, dit, style, benchmark, streaming, diffusion transformer  
- **[FADRA: Frequency-Aware Diffusion with Residual Adaptation for Video Face Restoration](https://arxiv.org/abs/2607.06389v1)**  
  Authors: Jin Jiang, Jia Wang, Panwen Hu, Weiran Zhao, Shengcai Liao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.06389v1.pdf)  
  Keywords: text-to-video, efficient, video diffusion, temporal consistency, diffusion model  
- **[VendorBench-100: A Unified Cross-Paradigm Benchmark for Deepfake Image Detection](https://arxiv.org/abs/2607.06254v1)**  
  Authors: Sharayu N. Deshmukh, Md Rashidunnabi, Nelton Tiago Gemo, Kurundkar G. D., Mahamune M. R., Nilesh K. Deshmukh  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.06254v1.pdf) | [![GitHub](https://img.shields.io/github/stars/sharayu-20/vendorbench-100?style=social)](https://github.com/sharayu-20/vendorbench-100)  
  Keywords: avatar, text-to-video, efficient, dit, benchmark, evaluation  
- **[Enhancing Video Physical Consistency via Role-aware Joint Training and Modality-decoupled Denoising](https://arxiv.org/abs/2607.04653v2)**  
  Authors: Guangting Zheng, Haojing Chen, Hao Li, Jingtao Zhang, Zhen Yang, Xiaosong Jia, Xue Yang, Shaofeng Zhang, Yanyong Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.04653v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://tom-zgt.github.io/VPT)  
  Keywords: physical, dynamics, t2v, video diffusion, physics, benchmark, denoising, diffusion model  
- **[Lights, Camera, Carbon: Architectural Scaling Laws for Video Generation Energy Consumption](https://arxiv.org/abs/2607.04553v1)**  
  Authors: Nidhal Jegham, Boris Gamazaychikov, Sasha Luccioni  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.04553v1.pdf)  
  Keywords: text-to-video, efficient, t2v, video diffusion, dit, architecture, benchmark, video generation, diffusion model  
- **[HyperVAttention: Efficient Sparse Attention with Spatio-Temporal Clustering for Video Diffusion](https://arxiv.org/abs/2607.03012v1)**  
  Authors: Dongyeun Lee, Amir Zandieh, Vahab Mirrokni, Junmo Kim, Insu Han  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.03012v1.pdf)  
  Keywords: text-to-video, efficient, video diffusion, dit, denoising, video generation, diffusion transformer  

### Video Editing

- **[LightCrafter: PBR-Conditioned Video Diffusion Refinement for Controllable and Consistent Relighting](https://arxiv.org/abs/2607.08016v2)**  
  Authors: Zixin Guo, Yehonathan Litman, Yifeng He, John Miller, Chuhan Chen, Deva Ramanan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.08016v2.pdf)  
  Keywords: physical, controllable, video translation, video diffusion, dit, long-form, concept, benchmark, video-to-video, temporal consistency, video generation, diffusion model  
- **[ProxyPose: 6-DoF Pose Tracking via Video-to-Video Translation](https://arxiv.org/abs/2607.06555v1)**  
  Authors: Ruihang Zhang, Felix Taubner, Pooja Ravi, Kiriakos N. Kutulakos, David B. Lindell  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.06555v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://ruihangzhang97.github.io/proxypose)  
  Keywords: identity, video translation, body motion, video diffusion, dit, trajectory, video-to-video, diffusion model  
- **[Consistent and Editable: A Balanced Framework for Text-Guided Video Editing](https://arxiv.org/abs/2607.05056v1)**  
  Authors: Tao Jin, Li Xiao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.05056v1.pdf)  
  Keywords: temporal consistency, video editing, dit, diffusion model  
- **[ProxyUp: Training-Free Proxy-Conditioned Video Generation for Controllable Dynamics](https://arxiv.org/abs/2607.03732v1)**  
  Authors: Zanwei Zhou, Jiazhong Cen, Jiemin Fang, Yumeng He, Chen Yang, Sikuang Li, Fanpeng Meng, Zhikuan Bao, Wei Shen, Qi Tian  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.03732v1.pdf)  
  Keywords: physical, controllable, dynamics, simulation, dit, video editing, physics, video generation  
- **[LiveEdit: Towards Real-Time Diffusion-Based Streaming Video Editing](https://arxiv.org/abs/2606.26740v2)**  
  Authors: Xinyu Wang, Chongbo Zhao, Fangneng Zhan, Yue Ma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.26740v2.pdf)  
  Keywords: distillation, efficient, video editing, dit, benchmark, evaluation, streaming, interactive, video generation  
- **[Vera: A Layered Diffusion Model for Content-Preserving Video Editing](https://arxiv.org/abs/2606.23610v1)**  
  Authors: Hongkai Zheng, Ta-Ying Cheng, Benjamin Klein, Yisong Yue, Zhuoning Yuan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.23610v1.pdf)  
  Keywords: text-to-video, creative, dynamics, video editing, video diffusion, dit, architecture, benchmark, video generation, diffusion model  
- **[SteerVTE: Seamless Video Text Editing with Style and Glyph Control](https://arxiv.org/abs/2606.23254v1)**  
  Authors: Kai Zeng, Moran Li, Zhengwei Wang, Yingchen Yu, Yiheng Lin, Ruichuan An, Ming Lu, Qi She, Wentao Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.23254v1.pdf)  
  Keywords: video editing, video diffusion, dit, style, image to video, diffusion transformer, diffusion model  
- **[Generative Relightable Avatars](https://arxiv.org/abs/2606.22718v1)**  
  Authors: Kunwar Maheep Singh, Christian Theobalt, Rishabh Dabral  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.22718v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://vcai.mpi-inf.mpg.de/projects/GRA)  
  Keywords: long video, physical, avatar, controllable, dynamics, video diffusion, physics, evaluation, video-to-video, diffusion model  
- **[ReGenHuman: Re-Generating Human Appearances for Realistic Full-Body Video Anonymization](https://arxiv.org/abs/2606.14972v1)**  
  Authors: Adam Sun, Eshaan Barkataki, Arnold Milstein, Gordon Wetzstein, Ehsan Adeli  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.14972v1.pdf)  
  Keywords: dit, video-to-video, identity, video diffusion  
- **[Lip Forcing: Few-Step Autoregressive Diffusion for Real-time Lip Synchronization](https://arxiv.org/abs/2606.11180v1)**  
  Authors: Paul Hyunbin Cho, Jinhyuk Jang, SeokYoung Lee, Joungbin Lee, Siyoon Jin, Heeseong Shin, Jung Yi, Yunjin Park, Chulmin Park, Seungryong Kim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.11180v1.pdf)  
  Keywords: autoregressive, video diffusion, dit, denoising, trajectory, video-to-video, streaming, diffusion model  

### Video Inpainting & Completion

- **[The Seriality Gap in Video Diffusion Models](https://arxiv.org/abs/2607.13031v1)**  
  Authors: Jorge Diaz Chao, Konpat Preechakul, Yuxi Liu, Yutong Bai  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.13031v1.pdf)  
  Keywords: autoregressive, dynamics, simulation, video diffusion, denoising, video prediction, diffusion model  
- **[Video Generation Models Are Inherent Lighting Estimators](https://arxiv.org/abs/2607.04674v1)**  
  Authors: Ziqi Cai, Shuchen Weng, Kaiqi Liu, Zifeng Wang, Zhiquan Zhang, Minggui Teng, Han Jiang, Boxin Shi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.04674v1.pdf)  
  Keywords: video inpainting, physical, efficient, video diffusion, video generation, diffusion model  
- **[ImageWAM: Do World Action Models Really Need Video Generation, or Just Image Editing?](https://arxiv.org/abs/2606.19531v1)**  
  Authors: Yuyang Zhang, Wenyao Zhang, Zekun Qi, He Zhang, Haitao Lin, Jingbo Zhang, Yao Mu, Xiaokang Yang, Wenjun Zeng, Xin Jin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.19531v1.pdf)  
  Keywords: world model, dit, denoising, video generation, video prediction  
- **[R2RDreamer: 3D-aware Data Augmentation for Spatially-generalized 2D Manipulation Policies](https://arxiv.org/abs/2606.17040v1)**  
  Authors: Xiuwei Xu, Haowen Sun, Angyuan Ma, Yiwei Zhang, Zhenyu Wu, Xiaofeng Wang, Bingyao Yu, Zheng Zhu, Jie Zhou, Jiwen Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17040v1.pdf)  
  Keywords: video completion, controllable, image-to-video, simulation, dit, style, 3d-aware  
- **[PointAction: 3D Points as Universal Action Representations for Robot Control](https://arxiv.org/abs/2606.03943v1)**  
  Authors: Mutian Tong, Han Jiang, Qiao Feng, Lingjie Liu, Jiatao Gu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.03943v1.pdf)  
  Keywords: dynamics, simulation, video diffusion, 4d generation, video generation, video prediction, diffusion model  
- **[World Models: A Comprehensive Survey of Architectures, Methodologies, Reasoning Paradigms, and Applications](https://arxiv.org/abs/2606.00133v1)**  
  Authors: Arif Hassan Zidan, Yi Pan, Hanqi Jiang, Ruiyu Yan, Wei Ruan, Zihao Wu, Lifeng Chen, Weihang You, Xinliang Li, Bowen Chen, Huawen Hu, Peilong Wang, Sizhuang Liu, Jing Zhang, Siyuan Li, Zhengliang Liu, Yu Bao, Lin Zhao, Lichao Sun, Dajiang Zhu, Xiang Li, Jinglei Lv, Quanzheng Li, Wei Liu, Tianming Liu, Wei Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.00133v1.pdf)  
  Keywords: world model, dynamics, education, medical, architecture, physics, benchmark, evaluation, interactive, autonomous driving, video generation, robotics, survey, video prediction  
- **[Full-4D: Generating Full-Scope 4D Scenes from a Single-View Video](https://arxiv.org/abs/2605.25500v1)**  
  Authors: Tingxi Chen, Ke Hao, Yabo Chen, Zhengxue Cheng, Rong Xie, Li Song, Haibin Huang, Chi Zhang, Xuelong Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25500v1.pdf)  
  Keywords: physical, distillation, dit, video diffusion, 4d generation, multi-view video, interactive, flow matching, video synthesis, video interpolation, diffusion model  
- **[CRONOS: Benchmarking Counterfactual Physical Consistency in Video Models](https://arxiv.org/abs/2605.23699v1)**  
  Authors: León Begiristain, Olaf Dünkel, Adam Kortylewski  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.23699v1.pdf)  
  Keywords: physical, world model, dynamics, dit, benchmark, evaluation, video prediction  
- **[GEM-4D: Geometry-Enhanced Video World Models for Robot Manipulation](https://arxiv.org/abs/2605.22882v3)**  
  Authors: Kaichen Zhou, Yuzhen Chen, Fangneng Zhan, Hang Hua, Grace Chen, Xinhai Chang, Ao Qu, Yilun Du, Zhuang Liu, Paul Pu Liang, Mengyu Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.22882v3.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://gem-4d.github.io)  
  Keywords: physical, world model, dynamics, simulation, dit, architecture, video prediction  
- **[Goodbye Drift: Anchored Tree Sampling for Long-Horizon Video-to-Video Generation](https://arxiv.org/abs/2605.20476v1)**  
  Authors: Matthew Bendel, Stephen W. Bailey, Mithilesh Vaidya, Sumukh Badam, Xingzhe He  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20476v1.pdf)  
  Keywords: outpainting, distillation, autoregressive, t2v, dit, style, video-to-video, video generation  

### Video Super-Resolution & Enhancement

*Showing the latest 50 out of 67 papers*

- **[Text2Sign: A Single-GPU Diffusion Baseline for Text-to-Sign Language Video Generation](https://arxiv.org/abs/2607.13164v1)**  
  Authors: Ruize Xia  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.13164v1.pdf) | [![GitHub](https://img.shields.io/github/stars/xiaruize0911/text2sign?style=social)](https://github.com/xiaruize0911/text2sign)  
  Keywords: video diffusion, dit, style, evaluation, denoising, temporal consistency, video generation, diffusion model  
- **[The Seriality Gap in Video Diffusion Models](https://arxiv.org/abs/2607.13031v1)**  
  Authors: Jorge Diaz Chao, Konpat Preechakul, Yuxi Liu, Yutong Bai  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.13031v1.pdf)  
  Keywords: autoregressive, dynamics, simulation, video diffusion, denoising, video prediction, diffusion model  
- **[ACID: Adaptive Caching for vIDeo generation](https://arxiv.org/abs/2607.12358v1)**  
  Authors: Om Agrawal, Saurabh Agarwal, Aditya Akella  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.12358v1.pdf)  
  Keywords: acceleration, video diffusion, dit, denoising, evaluation, video generation, diffusion model  
- **[LongE2V: Long-Horizon Event-based Video Reconstruction, Prediction, and Frame Interpolation with Video Diffusion Models](https://arxiv.org/abs/2607.08770v1)**  
  Authors: Cheng-De Fan, Chun-Wei Tuan Mu, Chen-Wei Chang, Chin-Yang Lin, Kun-Ru Wu, Yu-Chee Tseng, Yu-Lun Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.08770v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://cdfan0627.github.io/LongE2V-page)  
  Keywords: autoregressive, video diffusion, frame interpolation, benchmark, diffusion model  
- **[OPSD-V: On-Policy Self-Distillation for Post-Training Few-Step Autoregressive Video Generators](https://arxiv.org/abs/2607.08766v1)**  
  Authors: Hongyu Liu, Chun Wang, Feng Gao, Xuanhua He, Yue Ma, Ziyu Wan, Yong Zhang, Xiaoming Wei, Qifeng Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.08766v1.pdf)  
  Keywords: long video, distillation, autoregressive, dynamics, video diffusion, dit, denoising, trajectory, diffusion model  
- **[OpenCoF: Learning to Reason Through Video Generation](https://arxiv.org/abs/2607.08763v1)**  
  Authors: Xinyan Chen, Ziyu Guo, Renrui Zhang, Dongzhi Jiang, Hongsheng Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.08763v1.pdf)  
  Keywords: benchmark, denoising, i2v, video generation  
- **[Dynamic-in-Few-Step: Unifying Dynamic Computation and Few-Step Distillation for Efficient Video Generation](https://arxiv.org/abs/2607.06631v1)**  
  Authors: Yu Cheng, Siyue Yao, Zhongang Qi, Shanyan Guan, Wei Li, Fajie Yuan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.06631v1.pdf)  
  Keywords: distillation, efficient, acceleration, video diffusion, architecture, denoising, video generation, diffusion model  
- **[MV-Forcing: Long Multi-View Video Generation via 4D-Grounded Spatio-Temporal Self-Forcing](https://arxiv.org/abs/2607.05376v1)**  
  Authors: Gal Fiebelman, Hadar Averbuch-Elor, Sagie Benaim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.05376v1.pdf)  
  Keywords: distillation, autoregressive, video diffusion, denoising, multi-view video, video generation, diffusion model  
- **[Enhancing Video Physical Consistency via Role-aware Joint Training and Modality-decoupled Denoising](https://arxiv.org/abs/2607.04653v2)**  
  Authors: Guangting Zheng, Haojing Chen, Hao Li, Jingtao Zhang, Zhen Yang, Xiaosong Jia, Xue Yang, Shaofeng Zhang, Yanyong Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.04653v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://tom-zgt.github.io/VPT)  
  Keywords: physical, dynamics, t2v, video diffusion, physics, benchmark, denoising, diffusion model  
- **[CineMobile: On-Device Image-to-Video Diffusion for Cinematic Camera Motion Generation](https://arxiv.org/abs/2607.03803v1)**  
  Authors: Xuyao Huang, Zelai Deng, Xu Wang, Xizhong Xiao, Zhijie Deng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.03803v1.pdf)  
  Keywords: distillation, image-to-video, efficient, video diffusion, dit, architecture, denoising, video generation, diffusion transformer  

### World Models & Simulation

*Showing the latest 50 out of 127 papers*

- **[From Pixels to States: Rethinking Interactive World Models as Game Engines](https://arxiv.org/abs/2607.14076v1)**  
  Authors: Zhen Li, Zian Meng, Shuwei Shi, Mingliang Zhai, Jiaming Tan, Chuanhao Li, Kaipeng Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.14076v1.pdf)  
  Keywords: interactive, world model, dit, dynamics  
- **[The Seriality Gap in Video Diffusion Models](https://arxiv.org/abs/2607.13031v1)**  
  Authors: Jorge Diaz Chao, Konpat Preechakul, Yuxi Liu, Yutong Bai  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.13031v1.pdf)  
  Keywords: autoregressive, dynamics, simulation, video diffusion, denoising, video prediction, diffusion model  
- **[FlowWAM: Optical Flow as a Unified Action Representation for World Action Models](https://arxiv.org/abs/2607.13017v1)**  
  Authors: Yixiang Chen, Peiyan Li, Yuan Xu, Qisen Ma, Jiabing Yang, Kai Wang, Jianhua Yang, Dong An, He Guan, Gaoteng Liu, Jianlou Si, Jun Huang, Jing Liu, Nianfeng Liu, Yan Huang, Liang Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.13017v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://flow-wam.github.io)  
  Keywords: trajectory, world model, video generation  
- **[SymbOmni: Evolving Agentic Omni Models via Symbolic Concept Learning](https://arxiv.org/abs/2607.12042v1)**  
  Authors: Jinxiu Liu, Jianru Li, Tanqing Kuang, Xuanming Liu, Kangfu Mei, Yandong Wen, Weiyang Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.12042v1.pdf)  
  Keywords: efficient, concept, benchmark, interactive, video synthesis  
- **[Cycle-World: Mitigating Error Accumulation in Long-term Video World Models via Reverse-Prediction Cycle Consistency](https://arxiv.org/abs/2607.11836v1)**  
  Authors: Zihan Su, Teng Hu, Jiangning Zhang, Ruiyan Wang, Ran Yi, Lizhuang Ma, Dacheng Tao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.11836v1.pdf)  
  Keywords: world model, autoregressive, efficient, benchmark, video synthesis, temporal consistency, video generation, diffusion model  
- **[ABot-3DWorld 0: A Universal World Model to Explore Any 3D Space](https://arxiv.org/abs/2607.11673v2)**  
  Authors: Mingchao Sun, Luyang Tang, Yu Liu, Xu Yan, Zhan Li, Yunwei Zhang, Fei Yu, Zengye Ge, Yumin Liu, Jiacheng Zhang, Yongchang Zhang, Jiawei Zhang, Zhicheng Liu, Zhongxu Sun, Tianjian Ouyang, Wenzheng Chen, Shixing Yang, Nianfei Fan, Guodong Sun, Huan Li, Zheng Zhou, Yongze Li, Yingliang Peng, Mengmeng Du, Yuan Liu, Haozhe Shi, Chunnuo Gong, Chengzhen Yu, Chunxue Jia, Yang Liu, Shiying Zeng, Junnan Lai, Hang Zhang, Ning Guo, Baoquan Chen, Mu Xu, Hongyu Pan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.11673v2.pdf)  
  Keywords: efficient, trajectory, world model, creative  
- **[Xiaomi-Robotics-U0: Unified Embodied Synthesis with World Foundation Model](https://arxiv.org/abs/2607.11643v1)**  
  Authors: Xinghang Li, Jun Guo, Qiwei Li, Long Qian, Hang Lai, Yueze Wang, Hongyu Yan, Jiahang Cao, Xi Chen, Jingen Qu, Jiaxi Song, Nan Sun, Hanye Zhao, Futeng Liu, Wanli Peng, Heyun Wang, Yunhong Wang, Caoyu Xia, Jack Zhao, Diyun Xiang, Hangjun Ye, Heng Qu, Huaping Liu, Jason Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.11643v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://robotics.xiaomi.com/xiaomi-robotics-u0.html)  
  Keywords: world model, controllable, autoregressive, dynamics, dit, evaluation, video generation, robotics  
- **[Is Energy Guidance All You Need? Training-Free Norm Injection for Driving World Models](https://arxiv.org/abs/2607.10781v1)**  
  Authors: Xiyan Su, Frank Diermeyer, Markus Lienkamp  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.10781v1.pdf)  
  Keywords: layout, world model, controllable, dit, trajectory  
- **[Unlocking Temporal Generalization in Hamiltonian Video Dynamics Models](https://arxiv.org/abs/2607.07763v1)**  
  Authors: Eli Laird, Corey Clark  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.07763v1.pdf)  
  Keywords: dynamics, physical, world model, video generation  
- **[Validate the Dream Before You Trust Its Verdict: Admissibility for World-Model Simulators](https://arxiv.org/abs/2607.07196v1)**  
  Authors: Christian Oefinger, Finn Rasmus Schäfer, Korbinian Moller, Mattia Piccinini, Johannes Betz  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.07196v1.pdf)  
  Keywords: world model, simulation, dit, autonomous driving, robotics  



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
