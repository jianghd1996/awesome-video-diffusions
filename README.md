# Awesome Video Diffusions [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of latest research papers, projects and resources related to Video Diffusion Models and Video Generation. Content is automatically updated daily.

> Last Update: 2026-07-10 03:19:50

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
- [Applications](#applications) (47 papers) - Domain-specific applications of video diffusion models
- [Architecture & Efficiency](#architecture-&-efficiency) (362 papers) - Architectural innovations (DiT, UNet), flow matching, and training/inference efficiency
- [Audio & Multi-modal](#audio-&-multi-modal) (21 papers) - Audio-driven and multi-modal conditioned video generation
- [Controllable Generation](#controllable-generation) (143 papers) - Controllable video generation with motion, camera, pose, or layout guidance
- [Human & Character Animation](#human-&-character-animation) (23 papers) - Human-centric video generation including talking heads, dance, and character animation
- [Image-to-Video Generation](#image-to-video-generation) (50 papers) - Methods for animating still images into videos
- [Long Video Generation](#long-video-generation) (131 papers) - Generating temporally consistent long-form videos beyond short clips
- [Personalization & Customization](#personalization-&-customization) (92 papers) - Personalized video generation with custom subjects, identities, or styles
- [Physical Understanding](#physical-understanding) (157 papers) - Physics-aware video generation and dynamics modeling
- [Surveys & Benchmarks](#surveys-&-benchmarks) (236 papers) - Survey papers, benchmarks, and evaluation metrics for video generation
- [Text-to-Video Generation](#text-to-video-generation) (73 papers) - Foundation models and methods for generating videos from text prompts
- [Video Editing](#video-editing) (32 papers) - Diffusion-based video editing, style transfer, and manipulation
- [Video Inpainting & Completion](#video-inpainting-&-completion) (10 papers) - Video inpainting, completion, outpainting, and temporal prediction
- [Video Super-Resolution & Enhancement](#video-super-resolution-&-enhancement) (72 papers) - Video quality improvement, upscaling, restoration, and frame interpolation
- [World Models & Simulation](#world-models-&-simulation) (129 papers) - Video generation as world simulators and interactive environment generation



## Table of Contents

- [Categorized Papers](#categorized-papers)
- [Classic Papers](#classic-papers)
- [Open Source Projects](#open-source-projects)
- [Applications](#applications)
- [Tutorials & Blogs](#tutorials--blogs)





## Categorized Papers

### 3D-aware Video Generation

- **[SoccerNet 2026 Challenges Results](https://arxiv.org/abs/2607.07320v1)**  
  Authors: Anthony Cioppa, Silvio Giancola, Håkan Ardö, Mohamad Dalal, Jan Held, Jérémie Ochin, Jiayuan Rao, Karen Sanchez, Renaud Vandeghen, Artur Xarles, Olivier Barnich, Albert Clapés, Mathieu Delvaux, Sergio Escalera, Bernard Ghanem, Cédric Hons, Antoine Houet, Sotiris Manitsaris, Tom Michel, Pierre Miralles, Thomas B. Moeslund, Mikael Nilsson, Bogdan Stanciulescu, Marc Van Droogenbroeck, Yanfeng Wang, Weidi Xie, Faisal Altawijri, Mohamed Atef, Semen Budennyy, Vasiliy Chelpanov, Puhua Chen, Yixin Chen, Lechao Cheng, Jianling Chu, Ju-Seong Do, Oleg Durygin, Omar Fetouh, Mirco Fuchs, Youssef Ghallab, Falguni Ghosh, Wonjun Heo, Yufeng Hu, Weixuan Huang, Phuong-Linh Huynh-Ha, Matvey Isupov, Yangguang Ji, Siyuan Jiang, Zhenxiang Jiang, Wonyong Jo, Ho-Young Jung, SeongHeon Kang, MinJae Kim, Youngseon Kim, Jakub Komosa, Artem Konshin, Trung-Hoang Le, Jongmin Lee, Lingling Li, Litao Li, Vadim Linkov, Fang Liu, Haoxuan Ma, Shun Makino, Ismail Mathkour, Konstantin Mitin, Mikhail Moiseev, Takumi Nagaya, Yuki Nakamura, Thanh-Khoi Nguyen, Hoang-Phuc Nguyen, Trong-Thuan Nguyen, Christian Orduz, Kwanyong Park, Fabian Perez, Parthsarthi Rawat, SuHyun Rim, Hoover Rueda-Chacón, Atom Scott, Minori Sugimura, Yuyang Sun, Shengeng Tang, Minh-Triet Tran, Ikuma Uchida, Juan Vanegas, Thanh-Nhan Vo, Jiangtao Wang, Yaxiong Wang, Xiaogang Wang, Ruifeng Wang, Rio Watanabe, Jiali Wen, Yongliang Wu, Di Yang, Xu Yang, Zhuo Yang, Xinyu Ye, Yibo Yu, Zihan Zhai, Yu Zhang, Zhenyu Zhao, Zhun Zhong, Yixi Zhou, Xingyu Zhu, Wenbo Zhu, Julian Ziegler  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.07320v1.pdf)  
  Keywords: benchmark, evaluation, dit, novel view  
- **[MV-Forcing: Long Multi-View Video Generation via 4D-Grounded Spatio-Temporal Self-Forcing](https://arxiv.org/abs/2607.05376v1)**  
  Authors: Gal Fiebelman, Hadar Averbuch-Elor, Sagie Benaim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.05376v1.pdf)  
  Keywords: distillation, denoising, diffusion model, video generation, autoregressive, video diffusion, multi-view video  
- **[HandsOnWorld: Unconstrained Egocentric Video Generation with Camera-Disentangled Hand Control](https://arxiv.org/abs/2607.02075v1)**  
  Authors: Yushuo Chen, Xiaoyu Shi, Xiaoshi Wu, Xintao Wang, Pengfei Wan, Yebin Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.02075v1.pdf)  
  Keywords: video generation, 3d-aware  
- **[NeoMap: Training-free Novel-View Synthesis from Single Images and Videos](https://arxiv.org/abs/2607.01962v1)**  
  Authors: Jinxi Li, Tianyi Zhang, Yafei Yang, Zihui Zhang, Peng Huang, Koon Wing Macgyver Lin, Bo Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.01962v1.pdf)  
  Keywords: dit, denoising, video synthesis, novel view, benchmark  
- **[RayPE: Ray-Space Positional Encoding for 3D-Aware Video Generation](https://arxiv.org/abs/2606.27345v2)**  
  Authors: Minghao Yin, Jiahao Lu, Wenbo Hu, Wang Zhao, Shan Ying, Kai Han  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.27345v2.pdf)  
  Keywords: dit, diffusion transformer, identity, video generation, camera control, video diffusion, 3d-aware  
- **[Follow Your Track: Precise Skeleton Animation Controlled by 3D Trajectories](https://arxiv.org/abs/2606.25344v1)**  
  Authors: Yueting Liu, Yanqin Jiang, Nian Liu, Jingmen Zhou, Zhengjun Zha, Weiming Hu, Jin Gao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.25344v1.pdf)  
  Keywords: temporal consistency, dit, trajectory, body motion, efficient, 4d generation  
- **[OmniDrive: An LLM-Choreographed Multi-Agent World Model with Unified Latent Co-Compression for Multi-View Driving Video Generation](https://arxiv.org/abs/2606.17536v1)**  
  Authors: Zijie Meng, Yufei Liu, Chengqian Ma, Zhiyu Li, Jiyuan Liu, Wenhua Nie, Bingcai Wei, Shuqin Chen, Weichen Xu, Jiquan Yuan, Miao Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17536v1.pdf)  
  Keywords: dit, layout, world model, video generation, autonomous driving, controllable, multi-view video  
- **[R2RDreamer: 3D-aware Data Augmentation for Spatially-generalized 2D Manipulation Policies](https://arxiv.org/abs/2606.17040v1)**  
  Authors: Xiuwei Xu, Haowen Sun, Angyuan Ma, Yiwei Zhang, Zhenyu Wu, Xiaofeng Wang, Bingyao Yu, Zheng Zhu, Jie Zhou, Jiwen Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17040v1.pdf)  
  Keywords: dit, video completion, style, simulation, image-to-video, controllable, 3d-aware  
- **[Flex4DHuman: Flexible Multi-view Video Diffusion for 4D Human Reconstruction](https://arxiv.org/abs/2606.13655v2)**  
  Authors: Jen-Hao Cheng, Yipeng Wang, Hao Zhang, Gengshan Yang, Jenq-Neng Hwang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13655v2.pdf)  
  Keywords: dit, architecture, diffusion model, simulation, text-to-video, video diffusion, multi-view video  
- **[Latent Spatial Memory for Video World Models](https://arxiv.org/abs/2606.09828v1)**  
  Authors: Weijie Wang, Haoyu Zhao, Yifan Yang, Feng Chen, Zeyu Zhang, Yefei He, Zicheng Duan, Donny Y. Chen, Yuqing Yang, Bohan Zhuang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.09828v1.pdf)  
  Keywords: world model, diffusion model, video generation, depth-guided, novel view  

### Applications

- **[Validate the Dream Before You Trust Its Verdict: Admissibility for World-Model Simulators](https://arxiv.org/abs/2607.07196v1)**  
  Authors: Christian Oefinger, Finn Rasmus Schäfer, Korbinian Moller, Mattia Piccinini, Johannes Betz  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.07196v1.pdf)  
  Keywords: dit, world model, simulation, robotics, autonomous driving  
- **[Point as Skeleton: Accumulated Point Cloud Enhanced Autoregressive Generation for Closed-Loop Autonomous Driving Simulation](https://arxiv.org/abs/2607.06516v1)**  
  Authors: Songbur Wong, Xiaosong Jia, Junqi You, Bo Zhang, Pei Xu, Renqiu Xia, Yuping Qiu, Shaofeng Zhang, Zelin Zhao, Xuechao Yan, Yuchen Zhou, Yurui Chen, Wen Guo, Hang Xu, Junchi Yan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.06516v1.pdf) | [![GitHub](https://img.shields.io/github/stars/krauwu/point-as-skeleton?style=social)](https://github.com/krauwu/point-as-skeleton)  
  Keywords: dit, video generation, simulation, autoregressive, autonomous driving  
- **[A Definition and Roadmap for World Models](https://arxiv.org/abs/2607.06401v1)**  
  Authors: Xinyuan Chen, Haoyu Guo, Shi Guo, Bingqi Jiang, Chunhua Shen, Xing Shen, Tianfan Xue, Yufei Xue, Mulin Yu, Weinan Zhang, Bin Zhao, Bowen Zhou, Ming Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.06401v1.pdf)  
  Keywords: dynamics, world model, video generation, robotics, concept, physical  
- **[Benchmarking the Robustness of Autonomous Driving to Environmental Illusions: A Lane Perception Perspective](https://arxiv.org/abs/2607.05783v1)**  
  Authors: Tianyuan Zhang, Xianglong Liu, Aishan Liu, Lu Wang, Yitong Zhang, Peng Yue, Mingchuan Zhang, Siyuan Liang, Dacheng Tao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.05783v1.pdf)  
  Keywords: dit, evaluation, simulation, autonomous driving, benchmark, controllable  
- **[SpheRoPE: Zero-Shot Optimization-Free 360 Panorama Generation with Spherical RoPE](https://arxiv.org/abs/2606.32033v1)**  
  Authors: Or Hirschorn, Aaron Olender, Eli Alshan, Ianir Ideses, Lior Fritz, Sagie Benaim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.32033v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://orhir.github.io/SpheRoPE)  
  Keywords: creative, diffusion transformer  
- **[World Narrative Model for Highly Controllable Video Generation: A Paradigm Shift from Pixel Sampling to Physical World Orchestration](https://arxiv.org/abs/2606.31946v1)**  
  Authors: Ye Chen, Xuanhong Chen, Yupeng Zhu, Liming Tan, Zhewen Wan, Yuxuan Xiong, Tielong Wang, Jinfan Liu, Wuze Zhang, Xiongzhen Zhang, Feifei Li, Xianglin Luo, Zhehan Zhao, Zhifan Zhang, Laisheng Kou, Zhujing Liang, Yugang Chen, Muchun Chen, Xu Miao, Yijing Zhang, Xiaojie Sheng, Qiang Hu, Jialiang Chen, Weimin Zhang, Wenjun Zhang, Bingbing Ni  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.31946v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://glassroom.sjtu.edu.cn/WNM)  
  Keywords: dit, layout, film, video generation, efficient, physical, controllable  
- **[InfiniVerse: Occupancy Guided Unbounded Scene Generation for Autonomous Driving](https://arxiv.org/abs/2606.31109v1)**  
  Authors: Xiaoyu Ye, Leheng Li, Xinyu Ji, Yingjie Cai, Hongda He, Xu Yan, Guanyi Zhao, Ying-Cong Chen, Bingbing Liu, Shuguang Cui, Zhen Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.31109v1.pdf)  
  Keywords: dit, evaluation, diffusion model, autoregressive, autonomous driving, benchmark, video diffusion, controllable  
- **[Vertigo Vertigo: Reconstructing a Cinematic Ideal through its Predictive AI Double](https://arxiv.org/abs/2607.00047v2)**  
  Authors: Adam Cole, Mick Grierson  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.00047v2.pdf)  
  Keywords: dit, frame interpolation, acceleration, film, diffusion model, video diffusion  
- **[UnfoldArt: Zero-Shot Recovery of Full Articulated 3D Objects from Text or Image](https://arxiv.org/abs/2606.30608v2)**  
  Authors: Mohamed el Amine Boudjoghra, Ivan Laptev, Angela Dai  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.30608v2.pdf)  
  Keywords: dit, robotics, interactive  
- **[Semantic-Aware, Physics-Informed, Geometry-Grounded Weather Video Synthesis](https://arxiv.org/abs/2606.29020v1)**  
  Authors: Chenghao Qian, Nedko Savov, Lingdong Kong, Yeying Jin, Rui Song, Wenjing Li, Zhun Zhong, Jiaqi Ma, Gustav Markkula, Luc Van Gool  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.29020v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://jumponthemoon.github.io/w-crafter)  
  Keywords: dit, video synthesis, dynamics, identity, simulation, physics, physical, autonomous driving  

### Architecture & Efficiency

*Showing the latest 50 out of 362 papers*

- **[OPSD-V: On-Policy Self-Distillation for Post-Training Few-Step Autoregressive Video Generators](https://arxiv.org/abs/2607.08766v1)**  
  Authors: Hongyu Liu, Chun Wang, Feng Gao, Xuanhua He, Yue Ma, Ziyu Wan, Yong Zhang, Xiaoming Wei, Qifeng Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.08766v1.pdf)  
  Keywords: distillation, dit, trajectory, denoising, dynamics, diffusion model, autoregressive, long video, video diffusion  
- **[HumanForge: A Human-Centric Deepfake Video Benchmark with Multi-Agent Forgery Rationales](https://arxiv.org/abs/2607.08705v1)**  
  Authors: Wenbo Xu, Zhimin Chen, Xiaojie Liang, Hengrui Liu, Wei Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.08705v1.pdf)  
  Keywords: dit, video synthesis, diffusion model, multi-modal, text-to-video, benchmark, video diffusion  
- **[Native Video-Action Pretraining for Generalizable Robot Control](https://arxiv.org/abs/2607.08639v1)**  
  Authors: Qihang Zhang, Lin Li, Luyao Zhang, Shuai Yang, Yiming Luo, Shuaiting Li, Ruilin Wang, Junke Wang, Jiahao Shao, Gangwei Xu, Jiaming Zhou, Yishu Shen, Yudong Jin, Fangyi Xu, Shuailei Ma, Jiaqi Liao, Guanxing Lu, Zifan Shi, Yongkun Wen, Yujie Zhao, Weixuan Tang, Xinyang Wang, Chaojian Li, Jiapeng Zhu, Ka Leong Cheng, Nan Xue, Xing Zhu, Yujun Shen, Yinghao Xu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.08639v1.pdf)  
  Keywords: dit, architecture, physical, dynamics  
- **[SAGA: Stable Acceleration Guidance for Autoregressive Video Generation](https://arxiv.org/abs/2607.08020v1)**  
  Authors: Thanh-Nhan Vo, Trong-Thuan Nguyen, Trung-Hoang Le, Tam V. Nguyen, Minh-Triet Tran  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.08020v1.pdf)  
  Keywords: streaming, acceleration, diffusion model, video generation, efficient, autoregressive, video diffusion  
- **[LightCrafter: PBR-Conditioned Video Diffusion Refinement for Controllable and Consistent Relighting](https://arxiv.org/abs/2607.08016v1)**  
  Authors: Zixin Guo, Yehonathan Litman, Yifeng He, John Miller, Chuhan Chen, Deva Ramanan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.08016v1.pdf)  
  Keywords: temporal consistency, dit, physical, diffusion model, video translation, video generation, long-form, concept, benchmark, video diffusion, controllable, video-to-video  
- **[Scaling Mixture-of-Experts Video Pretraining for Embodied Intelligence](https://arxiv.org/abs/2607.07675v1)**  
  Authors: Shuailei Ma, Jiaqi Liao, Xinyang Wang, Jingjing Wang, Chaoran Feng, Zijing Hu, Chong Bao, Zichen Xi, Yuqi Gan, Weisen Wang, Yanhong Zeng, Qin Zhao, Zifan Shi, Wei Wu, Hao Ouyang, Qiuyu Wang, Shangzhan Zhang, Jiahao Shao, Yipengjing Sun, Liangxiao Hu, Lunke Pan, Nan Xue, Kecheng Zheng, Yinghao Xu, Xing Zhu, Yujun Shen, Ka Leong Cheng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.07675v1.pdf)  
  Keywords: dit, evaluation, dynamics, architecture, physical  
- **[Behavior Foundations for Quadruped Robots: ABot-C0 Technical Report](https://arxiv.org/abs/2607.07370v2)**  
  Authors: Xufeng Zhao, Fuzhi Yang, Jianhui Chen, Li Gao, Zhang Meng, Jie Gao, Yao Zheng, Congyang Zhao, Tianxiong Lv, Menglin Yang, Minqi Gu, Yaru Zhao, Wenyu Liu, Honglin Han, Shihui Su, Zixiao Tang, Liu Liu, Mu Xu, Yang Cai, Wenbin Tang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.07370v2.pdf)  
  Keywords: motion control, dit, style, human motion, efficient, physical  
- **[SoccerNet 2026 Challenges Results](https://arxiv.org/abs/2607.07320v1)**  
  Authors: Anthony Cioppa, Silvio Giancola, Håkan Ardö, Mohamad Dalal, Jan Held, Jérémie Ochin, Jiayuan Rao, Karen Sanchez, Renaud Vandeghen, Artur Xarles, Olivier Barnich, Albert Clapés, Mathieu Delvaux, Sergio Escalera, Bernard Ghanem, Cédric Hons, Antoine Houet, Sotiris Manitsaris, Tom Michel, Pierre Miralles, Thomas B. Moeslund, Mikael Nilsson, Bogdan Stanciulescu, Marc Van Droogenbroeck, Yanfeng Wang, Weidi Xie, Faisal Altawijri, Mohamed Atef, Semen Budennyy, Vasiliy Chelpanov, Puhua Chen, Yixin Chen, Lechao Cheng, Jianling Chu, Ju-Seong Do, Oleg Durygin, Omar Fetouh, Mirco Fuchs, Youssef Ghallab, Falguni Ghosh, Wonjun Heo, Yufeng Hu, Weixuan Huang, Phuong-Linh Huynh-Ha, Matvey Isupov, Yangguang Ji, Siyuan Jiang, Zhenxiang Jiang, Wonyong Jo, Ho-Young Jung, SeongHeon Kang, MinJae Kim, Youngseon Kim, Jakub Komosa, Artem Konshin, Trung-Hoang Le, Jongmin Lee, Lingling Li, Litao Li, Vadim Linkov, Fang Liu, Haoxuan Ma, Shun Makino, Ismail Mathkour, Konstantin Mitin, Mikhail Moiseev, Takumi Nagaya, Yuki Nakamura, Thanh-Khoi Nguyen, Hoang-Phuc Nguyen, Trong-Thuan Nguyen, Christian Orduz, Kwanyong Park, Fabian Perez, Parthsarthi Rawat, SuHyun Rim, Hoover Rueda-Chacón, Atom Scott, Minori Sugimura, Yuyang Sun, Shengeng Tang, Minh-Triet Tran, Ikuma Uchida, Juan Vanegas, Thanh-Nhan Vo, Jiangtao Wang, Yaxiong Wang, Xiaogang Wang, Ruifeng Wang, Rio Watanabe, Jiali Wen, Yongliang Wu, Di Yang, Xu Yang, Zhuo Yang, Xinyu Ye, Yibo Yu, Zihan Zhai, Yu Zhang, Zhenyu Zhao, Zhun Zhong, Yixi Zhou, Xingyu Zhu, Wenbo Zhu, Julian Ziegler  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.07320v1.pdf)  
  Keywords: benchmark, evaluation, dit, novel view  
- **[Validate the Dream Before You Trust Its Verdict: Admissibility for World-Model Simulators](https://arxiv.org/abs/2607.07196v1)**  
  Authors: Christian Oefinger, Finn Rasmus Schäfer, Korbinian Moller, Mattia Piccinini, Johannes Betz  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.07196v1.pdf)  
  Keywords: dit, world model, simulation, robotics, autonomous driving  
- **[AnchorPrune: Relevance-Anchored Contextual Expansion for Visual Token Pruning](https://arxiv.org/abs/2607.07033v1)**  
  Authors: Kyuan Oh, Bumsoo Kim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.07033v1.pdf) | [![GitHub](https://img.shields.io/github/stars/MULTI-cau/AnchorPrune?style=social)](https://github.com/MULTI-cau/AnchorPrune)  
  Keywords: benchmark, architecture, efficient  

### Audio & Multi-modal

- **[HumanForge: A Human-Centric Deepfake Video Benchmark with Multi-Agent Forgery Rationales](https://arxiv.org/abs/2607.08705v1)**  
  Authors: Wenbo Xu, Zhimin Chen, Xiaojie Liang, Hengrui Liu, Wei Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.08705v1.pdf)  
  Keywords: dit, video synthesis, diffusion model, multi-modal, text-to-video, benchmark, video diffusion  
- **[AVTok: 1D Unified Tokenization for Holistic Audio-Video Generation](https://arxiv.org/abs/2606.30811v1)**  
  Authors: Kien T. Pham, I Chieh Chen, Qifeng Chen, Long Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.30811v1.pdf)  
  Keywords: dit, video generation, efficient, audio-to-video, sound, architecture  
- **[TRUST: Efficient Abdominal Trauma Recognition via Image-to-Ultrasound-Video Transfer Learning](https://arxiv.org/abs/2606.27777v1)**  
  Authors: Enguang Wang, Hao Zhou, Shuo Gao, Tuo Liu, Guangquan Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.27777v1.pdf)  
  Keywords: dit, dynamics, efficient, sound, image-to-video  
- **[PhyEditBench: A Real-World Multi-Stage Benchmark for Physics-Aware Image Editing](https://arxiv.org/abs/2606.26551v2)**  
  Authors: Shengbin Guo, Shaokang He, Chaoyue Meng, Shengpeng Xiao, Xunzhi Xiang, Shaofeng Zhang, Qi Fan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.26551v2.pdf) | [![GitHub](https://img.shields.io/github/stars/Previsior/PhyEditBench?style=social)](https://github.com/Previsior/PhyEditBench)  
  Keywords: dit, physics-aware, evaluation, dynamics, video generation, multi-modal, physics, benchmark, physical  
- **[Wan-Streamer v0.1: End-to-end Real-time Interactive Foundation Models](https://arxiv.org/abs/2606.25041v3)**  
  Authors: Lianghua Huang, Zhi-Fan Wu, Wei Wang, Yupeng Shi, Mengyang Feng, Junjie He, Chen-Wei Xie, Yu Liu, Jingren Zhou, Ang Wang, Bang Zhang, Baole Ai, Chen Liang, Cheng Yu, Chongyang Zhong, Jinwei Qi, Kai Zhu, Pandeng Li, Peng Zhang, Wenyuan Zhang, Xinhua Cheng, Yitong Huang, Yun Zheng, Yuzheng Wang, Zoubin Bi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.25041v3.pdf)  
  Keywords: avatar, streaming, interactive, audio-driven  
- **[InteractiveAvatar: Real-Time Streaming Video Generation for Consistent and Intent-Aware Avatars](https://arxiv.org/abs/2606.22905v2)**  
  Authors: Quanyue Song, Yishan He, Yanfei Zhang, Shihao Cheng, Zhixiang He, Zhizhi Guo, Chi Zhang, Xuelong Li, Caigui Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.22905v2.pdf)  
  Keywords: temporal consistency, distillation, streaming, avatar, video generation, autoregressive, interactive, audio-driven  
- **[T-MOR: Learning Motion-Aware Skeleton Representations for Human Action Recognition](https://arxiv.org/abs/2606.21607v1)**  
  Authors: Di Yang, Mahmoud Ali, Quan Kong, Gianpiero Francesca, Francois Bremond  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.21607v1.pdf)  
  Keywords: dit, multi-modal, human motion, benchmark, physical  
- **[PermaVid: Consistent Video Generation Across Edits via Disentangled Context Memory](https://arxiv.org/abs/2606.16449v2)**  
  Authors: Shuai Yang, Bingjie Gao, Ziwei Liu, Jiaqi Wang, Dahua Lin, Tong Wu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.16449v2.pdf)  
  Keywords: layout, video generation, multi-modal, dit  
- **[ReFree: Towards Realistic Co-Speech Video Generation via Reward-Free RL and Multilevel Speech Guidance](https://arxiv.org/abs/2606.13304v1)**  
  Authors: Salaheldin Mohamed, M. Hamza Mughal, Rishabh Dabral, Christian Theobalt  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.13304v1.pdf)  
  Keywords: video generation, evaluation, speech-driven  
- **[MSUE: Multi-Modal Soccer Understanding Expert](https://arxiv.org/abs/2606.12106v1)**  
  Authors: Litao Li, Yibo Yu, Yufeng Hu, Zhuo Yang, Jiali Wen, Yixin Chen, Yixi Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.12106v1.pdf)  
  Keywords: benchmark, architecture, multi-modal, long-form  

### Controllable Generation

*Showing the latest 50 out of 143 papers*

- **[OPSD-V: On-Policy Self-Distillation for Post-Training Few-Step Autoregressive Video Generators](https://arxiv.org/abs/2607.08766v1)**  
  Authors: Hongyu Liu, Chun Wang, Feng Gao, Xuanhua He, Yue Ma, Ziyu Wan, Yong Zhang, Xiaoming Wei, Qifeng Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.08766v1.pdf)  
  Keywords: distillation, dit, trajectory, denoising, dynamics, diffusion model, autoregressive, long video, video diffusion  
- **[LightCrafter: PBR-Conditioned Video Diffusion Refinement for Controllable and Consistent Relighting](https://arxiv.org/abs/2607.08016v1)**  
  Authors: Zixin Guo, Yehonathan Litman, Yifeng He, John Miller, Chuhan Chen, Deva Ramanan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.08016v1.pdf)  
  Keywords: temporal consistency, dit, physical, diffusion model, video translation, video generation, long-form, concept, benchmark, video diffusion, controllable, video-to-video  
- **[Behavior Foundations for Quadruped Robots: ABot-C0 Technical Report](https://arxiv.org/abs/2607.07370v2)**  
  Authors: Xufeng Zhao, Fuzhi Yang, Jianhui Chen, Li Gao, Zhang Meng, Jie Gao, Yao Zheng, Congyang Zhao, Tianxiong Lv, Menglin Yang, Minqi Gu, Yaru Zhao, Wenyu Liu, Honglin Han, Shihui Su, Zixiao Tang, Liu Liu, Mu Xu, Yang Cai, Wenbin Tang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.07370v2.pdf)  
  Keywords: motion control, dit, style, human motion, efficient, physical  
- **[ProxyPose: 6-DoF Pose Tracking via Video-to-Video Translation](https://arxiv.org/abs/2607.06555v1)**  
  Authors: Ruihang Zhang, Felix Taubner, Pooja Ravi, Kiriakos N. Kutulakos, David B. Lindell  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.06555v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://ruihangzhang97.github.io/proxypose)  
  Keywords: dit, trajectory, identity, diffusion model, video translation, body motion, video diffusion, video-to-video  
- **[Prompt-Adapter Context Routing for Parameter-Efficient Multi-Shot Long Video Extrapolation](https://arxiv.org/abs/2607.06481v1)**  
  Authors: Anna Córdoba, Adam Puente Tercero, Nerea Angulo Hijo, Mar Linares Tercero, Julia Barrientos, Ainhoa Miranda, Jesús Olivera  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.06481v1.pdf)  
  Keywords: dit, streaming, diffusion transformer, identity, style, efficient, text-to-video, long video, benchmark, video diffusion, controllable  
- **[Benchmarking the Robustness of Autonomous Driving to Environmental Illusions: A Lane Perception Perspective](https://arxiv.org/abs/2607.05783v1)**  
  Authors: Tianyuan Zhang, Xianglong Liu, Aishan Liu, Lu Wang, Yitong Zhang, Peng Yue, Mingchuan Zhang, Siyuan Liang, Dacheng Tao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.05783v1.pdf)  
  Keywords: dit, evaluation, simulation, autonomous driving, benchmark, controllable  
- **[FORGE: Towards Functional Tool-Use Generalization via Keypoint Trajectory Reasoning](https://arxiv.org/abs/2607.05780v1)**  
  Authors: Chuhao Zhou, Liquan Wang, Shuxin Cao, Xiangyu Chen, Yuxuan Hu, Boyu Ma, Animesh Garg, Jianfei Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.05780v1.pdf)  
  Keywords: benchmark, simulation, trajectory  
- **[Mask2Real-WM: Segmentation Masks as a Sim-to-Real Bridge for Controllable Dexterous World Models](https://arxiv.org/abs/2607.04546v1)**  
  Authors: Riccardo O. Feingold, Davide Liconti, Chenyu Yang, Robert K. Katzschmann  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.04546v1.pdf)  
  Keywords: dit, evaluation, action-conditioned, physical, dynamics, world model, simulation, benchmark, video diffusion, controllable  
- **[Aura: Consistent Multi-Subject Video Generation via VLM-Grounded Semantic Alignment](https://arxiv.org/abs/2607.04311v2)**  
  Authors: Zixiang Zhou, Zhentao Yu, Yifeng Ma, Hongmei Wang, Wenqing Yu, Cong Wang, Zilin Yang, Rui Chen, Jiarong Ou, Yezhou Liu, Yuan Zhou, Qinglin Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.04311v2.pdf)  
  Keywords: dit, diffusion transformer, subject-driven, video synthesis, dynamics, identity, video generation, controllable  
- **[Worldscape-MoE: A Unified Mixture-of-Experts World Model for Scalable Heterogeneous Action Control](https://arxiv.org/abs/2607.03964v1)**  
  Authors: Jianjie Fang, Yongyan Xu, Ziyou Wang, Chen Gao, Yuchao Huang, Zhaolu Wang, Rongze Tang, Mingyuan Jia, Baining Zhao, Weichen Zhang, Xin Zhang, Haisheng Su, Yu Shang, Wei Wu, Xinlei Chen, Yong Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.03964v1.pdf)  
  Keywords: dit, diffusion transformer, dynamics, world model, controllable, video generation, physical, interactive  

### Human & Character Animation

- **[Behavior Foundations for Quadruped Robots: ABot-C0 Technical Report](https://arxiv.org/abs/2607.07370v2)**  
  Authors: Xufeng Zhao, Fuzhi Yang, Jianhui Chen, Li Gao, Zhang Meng, Jie Gao, Yao Zheng, Congyang Zhao, Tianxiong Lv, Menglin Yang, Minqi Gu, Yaru Zhao, Wenyu Liu, Honglin Han, Shihui Su, Zixiao Tang, Liu Liu, Mu Xu, Yang Cai, Wenbin Tang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.07370v2.pdf)  
  Keywords: motion control, dit, style, human motion, efficient, physical  
- **[ProxyPose: 6-DoF Pose Tracking via Video-to-Video Translation](https://arxiv.org/abs/2607.06555v1)**  
  Authors: Ruihang Zhang, Felix Taubner, Pooja Ravi, Kiriakos N. Kutulakos, David B. Lindell  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.06555v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://ruihangzhang97.github.io/proxypose)  
  Keywords: dit, trajectory, identity, diffusion model, video translation, body motion, video diffusion, video-to-video  
- **[VendorBench-100: A Unified Cross-Paradigm Benchmark for Deepfake Image Detection](https://arxiv.org/abs/2607.06254v1)**  
  Authors: Sharayu N. Deshmukh, Md Rashidunnabi, Nelton Tiago Gemo, Kurundkar G. D., Mahamune M. R., Nilesh K. Deshmukh  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.06254v1.pdf) | [![GitHub](https://img.shields.io/github/stars/sharayu-20/vendorbench-100?style=social)](https://github.com/sharayu-20/vendorbench-100)  
  Keywords: dit, evaluation, avatar, efficient, text-to-video, benchmark  
- **[3D Scene-Adaptive Trajectory-Controllable Human Image Animation with Camera Movement](https://arxiv.org/abs/2606.30514v2)**  
  Authors: Deyin Liu, Jicheng Xu, Lin Yuanbo Wu, Xiaowei Zhao, Xiatian Zhu, Zhe Jin, Anjan Dutta  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.30514v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://robinhood256100.github.io/web-disp)  
  Keywords: dit, trajectory, video generation, camera control, human motion, image animation, benchmark, controllable  
- **[OmniDance: Multimodal Driven Dance Video Generation with Large-scale Internet Data](https://arxiv.org/abs/2606.30019v1)**  
  Authors: Kaixing Yang, Jiashu Zhu, Xulong Tang, Ziqiao Peng, Xiangyue Zhang, Chubin Chen, Puwei Wang, Jiahong Wu, Xiangxiang Chu, Hongyan Liu, Jun He  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.30019v1.pdf) | [![GitHub](https://img.shields.io/github/stars/AMAP-ML/OmniDance?style=social)](https://github.com/AMAP-ML/OmniDance)  
  Keywords: i2v, dit, dynamics, video generation, human motion, architecture  
- **[EMOSH: Expressive Motion and Shape Disentanglement for Human Animation](https://arxiv.org/abs/2606.28026v1)**  
  Authors: Dongbin Zhang, Hao Liu, Binquan Dai, Kangjie Chen, Chuming Wang, Chen Li, Jing Lyu, Haoqian Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.28026v1.pdf)  
  Keywords: dit, avatar, human animation, identity, video generation, gesture, controllable  
- **[Directing the World: Fast Autoregressive Video Generation with Compositional Human-Camera Control](https://arxiv.org/abs/2606.27964v1)**  
  Authors: Haoyuan Wang, Yabo Chen, Haibin Huang, Chi Zhang, Xuelong Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.27964v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://whydahuzi.github.io/Directing-the-World.github.io)  
  Keywords: motion control, interactive, trajectory, dynamics, world model, video generation, camera control, human motion, autoregressive, controllable  
- **[Follow Your Track: Precise Skeleton Animation Controlled by 3D Trajectories](https://arxiv.org/abs/2606.25344v1)**  
  Authors: Yueting Liu, Yanqin Jiang, Nian Liu, Jingmen Zhou, Zhengjun Zha, Weiming Hu, Jin Gao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.25344v1.pdf)  
  Keywords: temporal consistency, dit, trajectory, body motion, efficient, 4d generation  
- **[Wan-Streamer v0.1: End-to-end Real-time Interactive Foundation Models](https://arxiv.org/abs/2606.25041v3)**  
  Authors: Lianghua Huang, Zhi-Fan Wu, Wei Wang, Yupeng Shi, Mengyang Feng, Junjie He, Chen-Wei Xie, Yu Liu, Jingren Zhou, Ang Wang, Bang Zhang, Baole Ai, Chen Liang, Cheng Yu, Chongyang Zhong, Jinwei Qi, Kai Zhu, Pandeng Li, Peng Zhang, Wenyuan Zhang, Xinhua Cheng, Yitong Huang, Yun Zheng, Yuzheng Wang, Zoubin Bi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.25041v3.pdf)  
  Keywords: avatar, streaming, interactive, audio-driven  
- **[InteractiveAvatar: Real-Time Streaming Video Generation for Consistent and Intent-Aware Avatars](https://arxiv.org/abs/2606.22905v2)**  
  Authors: Quanyue Song, Yishan He, Yanfei Zhang, Shihao Cheng, Zhixiang He, Zhizhi Guo, Chi Zhang, Xuelong Li, Caigui Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.22905v2.pdf)  
  Keywords: temporal consistency, distillation, streaming, avatar, video generation, autoregressive, interactive, audio-driven  

### Image-to-Video Generation

- **[OpenCoF: Learning to Reason Through Video Generation](https://arxiv.org/abs/2607.08763v1)**  
  Authors: Xinyan Chen, Ziyu Guo, Renrui Zhang, Dongzhi Jiang, Hongsheng Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.08763v1.pdf)  
  Keywords: i2v, benchmark, video generation, denoising  
- **[CineMobile: On-Device Image-to-Video Diffusion for Cinematic Camera Motion Generation](https://arxiv.org/abs/2607.03803v1)**  
  Authors: Xuyao Huang, Zelai Deng, Xu Wang, Xizhong Xiao, Zhijie Deng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.03803v1.pdf)  
  Keywords: distillation, dit, diffusion transformer, denoising, architecture, video generation, efficient, image-to-video, video diffusion  
- **[OrbitQuant: Data-Agnostic Quantization for Image and Video Diffusion Transformers](https://arxiv.org/abs/2607.02461v1)**  
  Authors: Donghyun Lee, Jitesh Chavan, Duy Nguyen, Sam Huang, Liming Jiang, Priyadarshini Panda, Timo Mertens, Saurabh Shukla  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.02461v1.pdf)  
  Keywords: image to video, dit, diffusion transformer, video generation, video diffusion  
- **[QWERTY: Training-Free Motion Control via Query-Warped Video Diffusion Transformers](https://arxiv.org/abs/2607.01869v1)**  
  Authors: Kyobin Choo, Youngmin Kim, Hyunkyung Han, Geunrip Park, Chanyoung Kim, Sunyoung Jung, Seong Jae Hwang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.01869v1.pdf)  
  Keywords: motion control, dit, trajectory, diffusion transformer, diffusion model, image-to-video, video diffusion  
- **[Anti-Prompt: Image Protection against Text-Guided Image-to-Video Generation](https://arxiv.org/abs/2607.01499v2)**  
  Authors: Yeonghwan Song, Chanhui Lee, Jinsoo Park, Jeany Son  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.01499v2.pdf)  
  Keywords: i2v, temporal consistency, dit, evaluation, denoising, video generation, image-to-video, architecture  
- **[TrajLoc: Trajectory-Attention Localization for Multi-Object Motion Control](https://arxiv.org/abs/2607.00861v1)**  
  Authors: Omer Sela, Inbar Huberman-Spiegelglas, Michael Rotman, Sagie Benaim, Avi Ben-Cohen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.00861v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://sela-omer.github.io/traj-loc)  
  Keywords: i2v, motion control, dit, evaluation, trajectory, identity, image-to-video  
- **[3D Scene-Adaptive Trajectory-Controllable Human Image Animation with Camera Movement](https://arxiv.org/abs/2606.30514v2)**  
  Authors: Deyin Liu, Jicheng Xu, Lin Yuanbo Wu, Xiaowei Zhao, Xiatian Zhu, Zhe Jin, Anjan Dutta  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.30514v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://robinhood256100.github.io/web-disp)  
  Keywords: dit, trajectory, video generation, camera control, human motion, image animation, benchmark, controllable  
- **[OmniDance: Multimodal Driven Dance Video Generation with Large-scale Internet Data](https://arxiv.org/abs/2606.30019v1)**  
  Authors: Kaixing Yang, Jiashu Zhu, Xulong Tang, Ziqiao Peng, Xiangyue Zhang, Chubin Chen, Puwei Wang, Jiahong Wu, Xiangxiang Chu, Hongyan Liu, Jun He  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.30019v1.pdf) | [![GitHub](https://img.shields.io/github/stars/AMAP-ML/OmniDance?style=social)](https://github.com/AMAP-ML/OmniDance)  
  Keywords: i2v, dit, dynamics, video generation, human motion, architecture  
- **[PhysisForcing: Physics Reinforced World Simulator for Robotic Manipulation](https://arxiv.org/abs/2606.28128v1)**  
  Authors: Peiwen Zhang, Yufan Deng, Shangkun Sun, Juncheng Ma, Duomin Wang, Jonas Du, Zilin Pan, Ye Huang, Hao Liang, Songyan Huang, Ruihua Zhang, Enze Xie, Ming-Yu Liu, Daquan Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.28128v1.pdf)  
  Keywords: i2v, dit, trajectory, world simulator, world model, video generation, simulation, physics, physical  
- **[TRUST: Efficient Abdominal Trauma Recognition via Image-to-Ultrasound-Video Transfer Learning](https://arxiv.org/abs/2606.27777v1)**  
  Authors: Enguang Wang, Hao Zhou, Shuo Gao, Tuo Liu, Guangquan Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.27777v1.pdf)  
  Keywords: dit, dynamics, efficient, sound, image-to-video  

### Long Video Generation

*Showing the latest 50 out of 131 papers*

- **[LongE2V: Long-Horizon Event-based Video Reconstruction, Prediction, and Frame Interpolation with Video Diffusion Models](https://arxiv.org/abs/2607.08770v1)**  
  Authors: Cheng-De Fan, Chun-Wei Tuan Mu, Chen-Wei Chang, Chin-Yang Lin, Kun-Ru Wu, Yu-Chee Tseng, Yu-Lun Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.08770v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://cdfan0627.github.io/LongE2V-page)  
  Keywords: frame interpolation, diffusion model, autoregressive, benchmark, video diffusion  
- **[OPSD-V: On-Policy Self-Distillation for Post-Training Few-Step Autoregressive Video Generators](https://arxiv.org/abs/2607.08766v1)**  
  Authors: Hongyu Liu, Chun Wang, Feng Gao, Xuanhua He, Yue Ma, Ziyu Wan, Yong Zhang, Xiaoming Wei, Qifeng Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.08766v1.pdf)  
  Keywords: distillation, dit, trajectory, denoising, dynamics, diffusion model, autoregressive, long video, video diffusion  
- **[SAGA: Stable Acceleration Guidance for Autoregressive Video Generation](https://arxiv.org/abs/2607.08020v1)**  
  Authors: Thanh-Nhan Vo, Trong-Thuan Nguyen, Trung-Hoang Le, Tam V. Nguyen, Minh-Triet Tran  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.08020v1.pdf)  
  Keywords: streaming, acceleration, diffusion model, video generation, efficient, autoregressive, video diffusion  
- **[LightCrafter: PBR-Conditioned Video Diffusion Refinement for Controllable and Consistent Relighting](https://arxiv.org/abs/2607.08016v1)**  
  Authors: Zixin Guo, Yehonathan Litman, Yifeng He, John Miller, Chuhan Chen, Deva Ramanan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.08016v1.pdf)  
  Keywords: temporal consistency, dit, physical, diffusion model, video translation, video generation, long-form, concept, benchmark, video diffusion, controllable, video-to-video  
- **[Point as Skeleton: Accumulated Point Cloud Enhanced Autoregressive Generation for Closed-Loop Autonomous Driving Simulation](https://arxiv.org/abs/2607.06516v1)**  
  Authors: Songbur Wong, Xiaosong Jia, Junqi You, Bo Zhang, Pei Xu, Renqiu Xia, Yuping Qiu, Shaofeng Zhang, Zelin Zhao, Xuechao Yan, Yuchen Zhou, Yurui Chen, Wen Guo, Hang Xu, Junchi Yan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.06516v1.pdf) | [![GitHub](https://img.shields.io/github/stars/krauwu/point-as-skeleton?style=social)](https://github.com/krauwu/point-as-skeleton)  
  Keywords: dit, video generation, simulation, autoregressive, autonomous driving  
- **[Prompt-Adapter Context Routing for Parameter-Efficient Multi-Shot Long Video Extrapolation](https://arxiv.org/abs/2607.06481v1)**  
  Authors: Anna Córdoba, Adam Puente Tercero, Nerea Angulo Hijo, Mar Linares Tercero, Julia Barrientos, Ainhoa Miranda, Jesús Olivera  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.06481v1.pdf)  
  Keywords: dit, streaming, diffusion transformer, identity, style, efficient, text-to-video, long video, benchmark, video diffusion, controllable  
- **[FADRA: Frequency-Aware Diffusion with Residual Adaptation for Video Face Restoration](https://arxiv.org/abs/2607.06389v1)**  
  Authors: Jin Jiang, Jia Wang, Panwen Hu, Weiran Zhao, Shengcai Liao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.06389v1.pdf)  
  Keywords: temporal consistency, diffusion model, efficient, text-to-video, video diffusion  
- **[MobileWan: Closing the Quality Gap for Mobile Video Diffusion](https://arxiv.org/abs/2607.06173v1)**  
  Authors: Mohsen Ghafoorian, Denis Korzhenkov, Adil Karjauv, Ioannis Lelekas, Noor Fathima, Spyridon Stasis, Hanno Ackermann, Boris van Breugel, Markus Nagel, Fatih Porikli, Animesh Karnewar, Amirhossein Habibian  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.06173v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://qualcomm-ai-research.github.io/mobilewan)  
  Keywords: distillation, diffusion transformer, architecture, diffusion model, video generation, efficient, autoregressive, video diffusion  
- **[SparseCtrl-HOI: Sparse Temporal Control for Human-Object Interaction Video Generation](https://arxiv.org/abs/2607.05994v1)**  
  Authors: Shenbo Xie, Mingrui Cai, Xu Yang, Yifei Liu, Changxing Ding  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.05994v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://mpi-lab.github.io/SparseCtrl-HOI)  
  Keywords: streaming, evaluation, dynamics, video generation, physical  
- **[MV-Forcing: Long Multi-View Video Generation via 4D-Grounded Spatio-Temporal Self-Forcing](https://arxiv.org/abs/2607.05376v1)**  
  Authors: Gal Fiebelman, Hadar Averbuch-Elor, Sagie Benaim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.05376v1.pdf)  
  Keywords: distillation, denoising, diffusion model, video generation, autoregressive, video diffusion, multi-view video  

### Personalization & Customization

*Showing the latest 50 out of 92 papers*

- **[Applying JEPA-Style Predictive Learning to JA4-Derived Network Fingerprints](https://arxiv.org/abs/2607.08465v1)**  
  Authors: Javier Izquierdo, Aygul Zagidullina  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.08465v1.pdf)  
  Keywords: style  
- **[LightCrafter: PBR-Conditioned Video Diffusion Refinement for Controllable and Consistent Relighting](https://arxiv.org/abs/2607.08016v1)**  
  Authors: Zixin Guo, Yehonathan Litman, Yifeng He, John Miller, Chuhan Chen, Deva Ramanan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.08016v1.pdf)  
  Keywords: temporal consistency, dit, physical, diffusion model, video translation, video generation, long-form, concept, benchmark, video diffusion, controllable, video-to-video  
- **[Behavior Foundations for Quadruped Robots: ABot-C0 Technical Report](https://arxiv.org/abs/2607.07370v2)**  
  Authors: Xufeng Zhao, Fuzhi Yang, Jianhui Chen, Li Gao, Zhang Meng, Jie Gao, Yao Zheng, Congyang Zhao, Tianxiong Lv, Menglin Yang, Minqi Gu, Yaru Zhao, Wenyu Liu, Honglin Han, Shihui Su, Zixiao Tang, Liu Liu, Mu Xu, Yang Cai, Wenbin Tang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.07370v2.pdf)  
  Keywords: motion control, dit, style, human motion, efficient, physical  
- **[ProxyPose: 6-DoF Pose Tracking via Video-to-Video Translation](https://arxiv.org/abs/2607.06555v1)**  
  Authors: Ruihang Zhang, Felix Taubner, Pooja Ravi, Kiriakos N. Kutulakos, David B. Lindell  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.06555v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://ruihangzhang97.github.io/proxypose)  
  Keywords: dit, trajectory, identity, diffusion model, video translation, body motion, video diffusion, video-to-video  
- **[Prompt-Adapter Context Routing for Parameter-Efficient Multi-Shot Long Video Extrapolation](https://arxiv.org/abs/2607.06481v1)**  
  Authors: Anna Córdoba, Adam Puente Tercero, Nerea Angulo Hijo, Mar Linares Tercero, Julia Barrientos, Ainhoa Miranda, Jesús Olivera  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.06481v1.pdf)  
  Keywords: dit, streaming, diffusion transformer, identity, style, efficient, text-to-video, long video, benchmark, video diffusion, controllable  
- **[A Definition and Roadmap for World Models](https://arxiv.org/abs/2607.06401v1)**  
  Authors: Xinyuan Chen, Haoyu Guo, Shi Guo, Bingqi Jiang, Chunhua Shen, Xing Shen, Tianfan Xue, Yufei Xue, Mulin Yu, Weinan Zhang, Bin Zhao, Bowen Zhou, Ming Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.06401v1.pdf)  
  Keywords: dynamics, world model, video generation, robotics, concept, physical  
- **[Aura: Consistent Multi-Subject Video Generation via VLM-Grounded Semantic Alignment](https://arxiv.org/abs/2607.04311v2)**  
  Authors: Zixiang Zhou, Zhentao Yu, Yifeng Ma, Hongmei Wang, Wenqing Yu, Cong Wang, Zilin Yang, Rui Chen, Jiarong Ou, Yezhou Liu, Yuan Zhou, Qinglin Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.04311v2.pdf)  
  Keywords: dit, diffusion transformer, subject-driven, video synthesis, dynamics, identity, video generation, controllable  
- **[G$^2$TAM: Geometry Grounded Track Anything Model](https://arxiv.org/abs/2607.03789v1)**  
  Authors: Chenming Zhu, Peizhou Cao, Jingli Lin, Wenbo Hu, Yunlong Ran, Jiangmiao Pang, Tai Wang, Xihui Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.03789v1.pdf)  
  Keywords: interactive, benchmark, evaluation, identity  
- **[TrajLoc: Trajectory-Attention Localization for Multi-Object Motion Control](https://arxiv.org/abs/2607.00861v1)**  
  Authors: Omer Sela, Inbar Huberman-Spiegelglas, Michael Rotman, Sagie Benaim, Avi Ben-Cohen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.00861v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://sela-omer.github.io/traj-loc)  
  Keywords: i2v, motion control, dit, evaluation, trajectory, identity, image-to-video  
- **[Towards Memory-Efficient Autoregressive Video Generation via Instance-Specific Parametric Absorption](https://arxiv.org/abs/2607.00712v1)**  
  Authors: Xiaomeng Fu, Jia Li, Yiming Hu, Yong Wang, Hayden Kwok-Hay So, Jiao Dai, Xiangxiang Chu, Jizhong Han  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.00712v1.pdf)  
  Keywords: streaming, identity, video generation, efficient, autoregressive, long video, architecture  

### Physical Understanding

*Showing the latest 50 out of 157 papers*

- **[OPSD-V: On-Policy Self-Distillation for Post-Training Few-Step Autoregressive Video Generators](https://arxiv.org/abs/2607.08766v1)**  
  Authors: Hongyu Liu, Chun Wang, Feng Gao, Xuanhua He, Yue Ma, Ziyu Wan, Yong Zhang, Xiaoming Wei, Qifeng Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.08766v1.pdf)  
  Keywords: distillation, dit, trajectory, denoising, dynamics, diffusion model, autoregressive, long video, video diffusion  
- **[Native Video-Action Pretraining for Generalizable Robot Control](https://arxiv.org/abs/2607.08639v1)**  
  Authors: Qihang Zhang, Lin Li, Luyao Zhang, Shuai Yang, Yiming Luo, Shuaiting Li, Ruilin Wang, Junke Wang, Jiahao Shao, Gangwei Xu, Jiaming Zhou, Yishu Shen, Yudong Jin, Fangyi Xu, Shuailei Ma, Jiaqi Liao, Guanxing Lu, Zifan Shi, Yongkun Wen, Yujie Zhao, Weixuan Tang, Xinyang Wang, Chaojian Li, Jiapeng Zhu, Ka Leong Cheng, Nan Xue, Xing Zhu, Yujun Shen, Yinghao Xu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.08639v1.pdf)  
  Keywords: dit, architecture, physical, dynamics  
- **[LightCrafter: PBR-Conditioned Video Diffusion Refinement for Controllable and Consistent Relighting](https://arxiv.org/abs/2607.08016v1)**  
  Authors: Zixin Guo, Yehonathan Litman, Yifeng He, John Miller, Chuhan Chen, Deva Ramanan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.08016v1.pdf)  
  Keywords: temporal consistency, dit, physical, diffusion model, video translation, video generation, long-form, concept, benchmark, video diffusion, controllable, video-to-video  
- **[Scaling Mixture-of-Experts Video Pretraining for Embodied Intelligence](https://arxiv.org/abs/2607.07675v1)**  
  Authors: Shuailei Ma, Jiaqi Liao, Xinyang Wang, Jingjing Wang, Chaoran Feng, Zijing Hu, Chong Bao, Zichen Xi, Yuqi Gan, Weisen Wang, Yanhong Zeng, Qin Zhao, Zifan Shi, Wei Wu, Hao Ouyang, Qiuyu Wang, Shangzhan Zhang, Jiahao Shao, Yipengjing Sun, Liangxiao Hu, Lunke Pan, Nan Xue, Kecheng Zheng, Yinghao Xu, Xing Zhu, Yujun Shen, Ka Leong Cheng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.07675v1.pdf)  
  Keywords: dit, evaluation, dynamics, architecture, physical  
- **[Unlocking Temporal Generalization in Hamiltonian Video Dynamics Models](https://arxiv.org/abs/2607.07763v1)**  
  Authors: Eli Laird, Corey Clark  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.07763v1.pdf)  
  Keywords: dynamics, video generation, physical, world model  
- **[Behavior Foundations for Quadruped Robots: ABot-C0 Technical Report](https://arxiv.org/abs/2607.07370v2)**  
  Authors: Xufeng Zhao, Fuzhi Yang, Jianhui Chen, Li Gao, Zhang Meng, Jie Gao, Yao Zheng, Congyang Zhao, Tianxiong Lv, Menglin Yang, Minqi Gu, Yaru Zhao, Wenyu Liu, Honglin Han, Shihui Su, Zixiao Tang, Liu Liu, Mu Xu, Yang Cai, Wenbin Tang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.07370v2.pdf)  
  Keywords: motion control, dit, style, human motion, efficient, physical  
- **[A Definition and Roadmap for World Models](https://arxiv.org/abs/2607.06401v1)**  
  Authors: Xinyuan Chen, Haoyu Guo, Shi Guo, Bingqi Jiang, Chunhua Shen, Xing Shen, Tianfan Xue, Yufei Xue, Mulin Yu, Weinan Zhang, Bin Zhao, Bowen Zhou, Ming Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.06401v1.pdf)  
  Keywords: dynamics, world model, video generation, robotics, concept, physical  
- **[SparseCtrl-HOI: Sparse Temporal Control for Human-Object Interaction Video Generation](https://arxiv.org/abs/2607.05994v1)**  
  Authors: Shenbo Xie, Mingrui Cai, Xu Yang, Yifei Liu, Changxing Ding  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.05994v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://mpi-lab.github.io/SparseCtrl-HOI)  
  Keywords: streaming, evaluation, dynamics, video generation, physical  
- **[FlowMark: Mask-Guided Video Watermarking](https://arxiv.org/abs/2607.05261v1)**  
  Authors: Vishal Asnani, Shruti Agarwal, John Collomosse  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.05261v1.pdf)  
  Keywords: dit, architecture, dynamics  
- **[DSWAM: A Dual-System World Action Foundation Model for Fine-Grained Robot Manipulation](https://arxiv.org/abs/2607.04927v1)**  
  Authors: Jian Zhu, Jianjun Zhang, Taiyi Su, Tianbin Liu, Zhangyuan Wang, Kai Xie, Zitai Huang, Chong Ma, Youzhang He, Tianjian Wang, Hanyang Wang, Weihao Ding, Yi Xu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.04927v1.pdf)  
  Keywords: evaluation, acceleration, world model, video generation, physical  

### Surveys & Benchmarks

*Showing the latest 50 out of 236 papers*

- **[LongE2V: Long-Horizon Event-based Video Reconstruction, Prediction, and Frame Interpolation with Video Diffusion Models](https://arxiv.org/abs/2607.08770v1)**  
  Authors: Cheng-De Fan, Chun-Wei Tuan Mu, Chen-Wei Chang, Chin-Yang Lin, Kun-Ru Wu, Yu-Chee Tseng, Yu-Lun Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.08770v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://cdfan0627.github.io/LongE2V-page)  
  Keywords: frame interpolation, diffusion model, autoregressive, benchmark, video diffusion  
- **[OpenCoF: Learning to Reason Through Video Generation](https://arxiv.org/abs/2607.08763v1)**  
  Authors: Xinyan Chen, Ziyu Guo, Renrui Zhang, Dongzhi Jiang, Hongsheng Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.08763v1.pdf)  
  Keywords: i2v, benchmark, video generation, denoising  
- **[HumanForge: A Human-Centric Deepfake Video Benchmark with Multi-Agent Forgery Rationales](https://arxiv.org/abs/2607.08705v1)**  
  Authors: Wenbo Xu, Zhimin Chen, Xiaojie Liang, Hengrui Liu, Wei Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.08705v1.pdf)  
  Keywords: dit, video synthesis, diffusion model, multi-modal, text-to-video, benchmark, video diffusion  
- **[LightCrafter: PBR-Conditioned Video Diffusion Refinement for Controllable and Consistent Relighting](https://arxiv.org/abs/2607.08016v1)**  
  Authors: Zixin Guo, Yehonathan Litman, Yifeng He, John Miller, Chuhan Chen, Deva Ramanan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.08016v1.pdf)  
  Keywords: temporal consistency, dit, physical, diffusion model, video translation, video generation, long-form, concept, benchmark, video diffusion, controllable, video-to-video  
- **[Scaling Mixture-of-Experts Video Pretraining for Embodied Intelligence](https://arxiv.org/abs/2607.07675v1)**  
  Authors: Shuailei Ma, Jiaqi Liao, Xinyang Wang, Jingjing Wang, Chaoran Feng, Zijing Hu, Chong Bao, Zichen Xi, Yuqi Gan, Weisen Wang, Yanhong Zeng, Qin Zhao, Zifan Shi, Wei Wu, Hao Ouyang, Qiuyu Wang, Shangzhan Zhang, Jiahao Shao, Yipengjing Sun, Liangxiao Hu, Lunke Pan, Nan Xue, Kecheng Zheng, Yinghao Xu, Xing Zhu, Yujun Shen, Ka Leong Cheng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.07675v1.pdf)  
  Keywords: dit, evaluation, dynamics, architecture, physical  
- **[SoccerNet 2026 Challenges Results](https://arxiv.org/abs/2607.07320v1)**  
  Authors: Anthony Cioppa, Silvio Giancola, Håkan Ardö, Mohamad Dalal, Jan Held, Jérémie Ochin, Jiayuan Rao, Karen Sanchez, Renaud Vandeghen, Artur Xarles, Olivier Barnich, Albert Clapés, Mathieu Delvaux, Sergio Escalera, Bernard Ghanem, Cédric Hons, Antoine Houet, Sotiris Manitsaris, Tom Michel, Pierre Miralles, Thomas B. Moeslund, Mikael Nilsson, Bogdan Stanciulescu, Marc Van Droogenbroeck, Yanfeng Wang, Weidi Xie, Faisal Altawijri, Mohamed Atef, Semen Budennyy, Vasiliy Chelpanov, Puhua Chen, Yixin Chen, Lechao Cheng, Jianling Chu, Ju-Seong Do, Oleg Durygin, Omar Fetouh, Mirco Fuchs, Youssef Ghallab, Falguni Ghosh, Wonjun Heo, Yufeng Hu, Weixuan Huang, Phuong-Linh Huynh-Ha, Matvey Isupov, Yangguang Ji, Siyuan Jiang, Zhenxiang Jiang, Wonyong Jo, Ho-Young Jung, SeongHeon Kang, MinJae Kim, Youngseon Kim, Jakub Komosa, Artem Konshin, Trung-Hoang Le, Jongmin Lee, Lingling Li, Litao Li, Vadim Linkov, Fang Liu, Haoxuan Ma, Shun Makino, Ismail Mathkour, Konstantin Mitin, Mikhail Moiseev, Takumi Nagaya, Yuki Nakamura, Thanh-Khoi Nguyen, Hoang-Phuc Nguyen, Trong-Thuan Nguyen, Christian Orduz, Kwanyong Park, Fabian Perez, Parthsarthi Rawat, SuHyun Rim, Hoover Rueda-Chacón, Atom Scott, Minori Sugimura, Yuyang Sun, Shengeng Tang, Minh-Triet Tran, Ikuma Uchida, Juan Vanegas, Thanh-Nhan Vo, Jiangtao Wang, Yaxiong Wang, Xiaogang Wang, Ruifeng Wang, Rio Watanabe, Jiali Wen, Yongliang Wu, Di Yang, Xu Yang, Zhuo Yang, Xinyu Ye, Yibo Yu, Zihan Zhai, Yu Zhang, Zhenyu Zhao, Zhun Zhong, Yixi Zhou, Xingyu Zhu, Wenbo Zhu, Julian Ziegler  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.07320v1.pdf)  
  Keywords: benchmark, evaluation, dit, novel view  
- **[AnchorPrune: Relevance-Anchored Contextual Expansion for Visual Token Pruning](https://arxiv.org/abs/2607.07033v1)**  
  Authors: Kyuan Oh, Bumsoo Kim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.07033v1.pdf) | [![GitHub](https://img.shields.io/github/stars/MULTI-cau/AnchorPrune?style=social)](https://github.com/MULTI-cau/AnchorPrune)  
  Keywords: benchmark, architecture, efficient  
- **[Prompt-Adapter Context Routing for Parameter-Efficient Multi-Shot Long Video Extrapolation](https://arxiv.org/abs/2607.06481v1)**  
  Authors: Anna Córdoba, Adam Puente Tercero, Nerea Angulo Hijo, Mar Linares Tercero, Julia Barrientos, Ainhoa Miranda, Jesús Olivera  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.06481v1.pdf)  
  Keywords: dit, streaming, diffusion transformer, identity, style, efficient, text-to-video, long video, benchmark, video diffusion, controllable  
- **[VendorBench-100: A Unified Cross-Paradigm Benchmark for Deepfake Image Detection](https://arxiv.org/abs/2607.06254v1)**  
  Authors: Sharayu N. Deshmukh, Md Rashidunnabi, Nelton Tiago Gemo, Kurundkar G. D., Mahamune M. R., Nilesh K. Deshmukh  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.06254v1.pdf) | [![GitHub](https://img.shields.io/github/stars/sharayu-20/vendorbench-100?style=social)](https://github.com/sharayu-20/vendorbench-100)  
  Keywords: dit, evaluation, avatar, efficient, text-to-video, benchmark  
- **[SparseCtrl-HOI: Sparse Temporal Control for Human-Object Interaction Video Generation](https://arxiv.org/abs/2607.05994v1)**  
  Authors: Shenbo Xie, Mingrui Cai, Xu Yang, Yifei Liu, Changxing Ding  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.05994v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://mpi-lab.github.io/SparseCtrl-HOI)  
  Keywords: streaming, evaluation, dynamics, video generation, physical  

### Text-to-Video Generation

*Showing the latest 50 out of 73 papers*

- **[HumanForge: A Human-Centric Deepfake Video Benchmark with Multi-Agent Forgery Rationales](https://arxiv.org/abs/2607.08705v1)**  
  Authors: Wenbo Xu, Zhimin Chen, Xiaojie Liang, Hengrui Liu, Wei Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.08705v1.pdf)  
  Keywords: dit, video synthesis, diffusion model, multi-modal, text-to-video, benchmark, video diffusion  
- **[Prompt-Adapter Context Routing for Parameter-Efficient Multi-Shot Long Video Extrapolation](https://arxiv.org/abs/2607.06481v1)**  
  Authors: Anna Córdoba, Adam Puente Tercero, Nerea Angulo Hijo, Mar Linares Tercero, Julia Barrientos, Ainhoa Miranda, Jesús Olivera  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.06481v1.pdf)  
  Keywords: dit, streaming, diffusion transformer, identity, style, efficient, text-to-video, long video, benchmark, video diffusion, controllable  
- **[FADRA: Frequency-Aware Diffusion with Residual Adaptation for Video Face Restoration](https://arxiv.org/abs/2607.06389v1)**  
  Authors: Jin Jiang, Jia Wang, Panwen Hu, Weiran Zhao, Shengcai Liao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.06389v1.pdf)  
  Keywords: temporal consistency, diffusion model, efficient, text-to-video, video diffusion  
- **[VendorBench-100: A Unified Cross-Paradigm Benchmark for Deepfake Image Detection](https://arxiv.org/abs/2607.06254v1)**  
  Authors: Sharayu N. Deshmukh, Md Rashidunnabi, Nelton Tiago Gemo, Kurundkar G. D., Mahamune M. R., Nilesh K. Deshmukh  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.06254v1.pdf) | [![GitHub](https://img.shields.io/github/stars/sharayu-20/vendorbench-100?style=social)](https://github.com/sharayu-20/vendorbench-100)  
  Keywords: dit, evaluation, avatar, efficient, text-to-video, benchmark  
- **[Enhancing Video Physical Consistency via Role-aware Joint Training and Modality-decoupled Denoising](https://arxiv.org/abs/2607.04653v2)**  
  Authors: Guangting Zheng, Haojing Chen, Hao Li, Jingtao Zhang, Zhen Yang, Xiaosong Jia, Xue Yang, Shaofeng Zhang, Yanyong Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.04653v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://tom-zgt.github.io/VPT)  
  Keywords: denoising, dynamics, diffusion model, physics, benchmark, video diffusion, physical, t2v  
- **[Lights, Camera, Carbon: Architectural Scaling Laws for Video Generation Energy Consumption](https://arxiv.org/abs/2607.04553v1)**  
  Authors: Nidhal Jegham, Boris Gamazaychikov, Sasha Luccioni  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.04553v1.pdf)  
  Keywords: dit, architecture, diffusion model, video generation, efficient, text-to-video, benchmark, video diffusion, t2v  
- **[HyperVAttention: Efficient Sparse Attention with Spatio-Temporal Clustering for Video Diffusion](https://arxiv.org/abs/2607.03012v1)**  
  Authors: Dongyeun Lee, Amir Zandieh, Vahab Mirrokni, Junmo Kim, Insu Han  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.03012v1.pdf)  
  Keywords: dit, diffusion transformer, denoising, video generation, efficient, text-to-video, video diffusion  
- **[Track the Noise, Move the World:3D-Grounded Motion-Consistent Noise for Controllable Video Generation](https://arxiv.org/abs/2607.02798v1)**  
  Authors: Long Vu, Tan Ngo, Animesh Karnewar, Amir Habibian, Binh-Son Hua, Hung Bui, Minh Hoai Nguyen, Phong Nguyen-Ha  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.02798v1.pdf)  
  Keywords: motion control, temporal consistency, dit, latent video, denoising, diffusion model, video generation, text-to-video, benchmark, video diffusion, controllable  
- **[ICDepth: Taming Video Diffusion Models for Video Depth Estimation via In-Context Conditioning](https://arxiv.org/abs/2607.01677v1)**  
  Authors: Xuanhua He, Jiaxin Xie, Mingzhe Zheng, Qifeng Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.01677v1.pdf)  
  Keywords: temporal consistency, dit, diffusion transformer, diffusion model, text-to-video, benchmark, video diffusion  
- **[Your Data Manifold is Secretly a Reward Model: Shell-LCC for Text-to-Video Generation](https://arxiv.org/abs/2606.30248v1)**  
  Authors: Shihao Zhang, Yuguang Yan, Junzhe Zhang, Wei Zhao, Bohan Wang, Hanwang Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.30248v1.pdf)  
  Keywords: text-to-video, video generation, diffusion model, t2v  

### Video Editing

- **[LightCrafter: PBR-Conditioned Video Diffusion Refinement for Controllable and Consistent Relighting](https://arxiv.org/abs/2607.08016v1)**  
  Authors: Zixin Guo, Yehonathan Litman, Yifeng He, John Miller, Chuhan Chen, Deva Ramanan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.08016v1.pdf)  
  Keywords: temporal consistency, dit, physical, diffusion model, video translation, video generation, long-form, concept, benchmark, video diffusion, controllable, video-to-video  
- **[ProxyPose: 6-DoF Pose Tracking via Video-to-Video Translation](https://arxiv.org/abs/2607.06555v1)**  
  Authors: Ruihang Zhang, Felix Taubner, Pooja Ravi, Kiriakos N. Kutulakos, David B. Lindell  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.06555v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://ruihangzhang97.github.io/proxypose)  
  Keywords: dit, trajectory, identity, diffusion model, video translation, body motion, video diffusion, video-to-video  
- **[Consistent and Editable: A Balanced Framework for Text-Guided Video Editing](https://arxiv.org/abs/2607.05056v1)**  
  Authors: Tao Jin, Li Xiao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.05056v1.pdf)  
  Keywords: diffusion model, dit, temporal consistency, video editing  
- **[ProxyUp: Training-Free Proxy-Conditioned Video Generation for Controllable Dynamics](https://arxiv.org/abs/2607.03732v1)**  
  Authors: Zanwei Zhou, Jiazhong Cen, Jiemin Fang, Yumeng He, Chen Yang, Sikuang Li, Fanpeng Meng, Zhikuan Bao, Wei Shen, Qi Tian  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.03732v1.pdf)  
  Keywords: dit, dynamics, video generation, simulation, physics, physical, controllable, video editing  
- **[LiveEdit: Towards Real-Time Diffusion-Based Streaming Video Editing](https://arxiv.org/abs/2606.26740v1)**  
  Authors: Xinyu Wang, Chongbo Zhao, Fangneng Zhan, Yue Ma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.26740v1.pdf)  
  Keywords: distillation, dit, streaming, evaluation, video generation, efficient, benchmark, interactive, video editing  
- **[Vera: A Layered Diffusion Model for Content-Preserving Video Editing](https://arxiv.org/abs/2606.23610v1)**  
  Authors: Hongkai Zheng, Ta-Ying Cheng, Benjamin Klein, Yisong Yue, Zhuoning Yuan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.23610v1.pdf)  
  Keywords: dit, dynamics, architecture, creative, diffusion model, video generation, text-to-video, benchmark, video diffusion, video editing  
- **[SteerVTE: Seamless Video Text Editing with Style and Glyph Control](https://arxiv.org/abs/2606.23254v1)**  
  Authors: Kai Zeng, Moran Li, Zhengwei Wang, Yingchen Yu, Yiheng Lin, Ruichuan An, Ming Lu, Qi She, Wentao Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.23254v1.pdf)  
  Keywords: image to video, dit, diffusion transformer, style, diffusion model, video diffusion, video editing  
- **[Generative Relightable Avatars](https://arxiv.org/abs/2606.22718v1)**  
  Authors: Kunwar Maheep Singh, Christian Theobalt, Rishabh Dabral  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.22718v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://vcai.mpi-inf.mpg.de/projects/GRA)  
  Keywords: physics, evaluation, physical, avatar, dynamics, diffusion model, long video, video diffusion, controllable, video-to-video  
- **[ReGenHuman: Re-Generating Human Appearances for Realistic Full-Body Video Anonymization](https://arxiv.org/abs/2606.14972v1)**  
  Authors: Adam Sun, Eshaan Barkataki, Arnold Milstein, Gordon Wetzstein, Ehsan Adeli  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.14972v1.pdf)  
  Keywords: dit, video diffusion, identity, video-to-video  
- **[Lip Forcing: Few-Step Autoregressive Diffusion for Real-time Lip Synchronization](https://arxiv.org/abs/2606.11180v1)**  
  Authors: Paul Hyunbin Cho, Jinhyuk Jang, SeokYoung Lee, Joungbin Lee, Siyoon Jin, Heeseong Shin, Jung Yi, Yunjin Park, Chulmin Park, Seungryong Kim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.11180v1.pdf)  
  Keywords: dit, streaming, trajectory, denoising, diffusion model, autoregressive, video diffusion, video-to-video  

### Video Inpainting & Completion

- **[Video Generation Models Are Inherent Lighting Estimators](https://arxiv.org/abs/2607.04674v1)**  
  Authors: Ziqi Cai, Shuchen Weng, Kaiqi Liu, Zifeng Wang, Zhiquan Zhang, Minggui Teng, Han Jiang, Boxin Shi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.04674v1.pdf)  
  Keywords: diffusion model, video generation, efficient, video diffusion, physical, video inpainting  
- **[ImageWAM: Do World Action Models Really Need Video Generation, or Just Image Editing?](https://arxiv.org/abs/2606.19531v1)**  
  Authors: Yuyang Zhang, Wenyao Zhang, Zekun Qi, He Zhang, Haitao Lin, Jingbo Zhang, Yao Mu, Xiaokang Yang, Wenjun Zeng, Xin Jin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.19531v1.pdf)  
  Keywords: dit, denoising, video prediction, world model, video generation  
- **[R2RDreamer: 3D-aware Data Augmentation for Spatially-generalized 2D Manipulation Policies](https://arxiv.org/abs/2606.17040v1)**  
  Authors: Xiuwei Xu, Haowen Sun, Angyuan Ma, Yiwei Zhang, Zhenyu Wu, Xiaofeng Wang, Bingyao Yu, Zheng Zhu, Jie Zhou, Jiwen Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.17040v1.pdf)  
  Keywords: dit, video completion, style, simulation, image-to-video, controllable, 3d-aware  
- **[PointAction: 3D Points as Universal Action Representations for Robot Control](https://arxiv.org/abs/2606.03943v1)**  
  Authors: Mutian Tong, Han Jiang, Qiao Feng, Lingjie Liu, Jiatao Gu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.03943v1.pdf)  
  Keywords: video prediction, dynamics, diffusion model, video generation, simulation, 4d generation, video diffusion  
- **[World Models: A Comprehensive Survey of Architectures, Methodologies, Reasoning Paradigms, and Applications](https://arxiv.org/abs/2606.00133v1)**  
  Authors: Arif Hassan Zidan, Yi Pan, Hanqi Jiang, Ruiyu Yan, Wei Ruan, Zihao Wu, Lifeng Chen, Weihang You, Xinliang Li, Bowen Chen, Huawen Hu, Peilong Wang, Sizhuang Liu, Jing Zhang, Siyuan Li, Zhengliang Liu, Yu Bao, Lin Zhao, Lichao Sun, Dajiang Zhu, Xiang Li, Jinglei Lv, Quanzheng Li, Wei Liu, Tianming Liu, Wei Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2606.00133v1.pdf)  
  Keywords: physics, evaluation, autonomous driving, video prediction, dynamics, world model, video generation, robotics, education, survey, benchmark, architecture, interactive, medical  
- **[Full-4D: Generating Full-Scope 4D Scenes from a Single-View Video](https://arxiv.org/abs/2605.25500v1)**  
  Authors: Tingxi Chen, Ke Hao, Yabo Chen, Zhengxue Cheng, Rong Xie, Li Song, Haibin Huang, Chi Zhang, Xuelong Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.25500v1.pdf)  
  Keywords: distillation, video interpolation, dit, physical, flow matching, video synthesis, diffusion model, 4d generation, video diffusion, interactive, multi-view video  
- **[CRONOS: Benchmarking Counterfactual Physical Consistency in Video Models](https://arxiv.org/abs/2605.23699v1)**  
  Authors: León Begiristain, Olaf Dünkel, Adam Kortylewski  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.23699v1.pdf)  
  Keywords: dit, evaluation, video prediction, dynamics, world model, benchmark, physical  
- **[GEM-4D: Geometry-Enhanced Video World Models for Robot Manipulation](https://arxiv.org/abs/2605.22882v3)**  
  Authors: Kaichen Zhou, Yuzhen Chen, Fangneng Zhan, Hang Hua, Grace Chen, Xinhai Chang, Ao Qu, Yilun Du, Zhuang Liu, Paul Pu Liang, Mengyu Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.22882v3.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://gem-4d.github.io)  
  Keywords: dit, video prediction, dynamics, world model, simulation, architecture, physical  
- **[Goodbye Drift: Anchored Tree Sampling for Long-Horizon Video-to-Video Generation](https://arxiv.org/abs/2605.20476v1)**  
  Authors: Matthew Bendel, Stephen W. Bailey, Mithilesh Vaidya, Sumukh Badam, Xingzhe He  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.20476v1.pdf)  
  Keywords: distillation, dit, t2v, style, outpainting, video generation, autoregressive, video-to-video  
- **[Nano World Models: A Minimalist Implementation of Future Video Prediction](https://arxiv.org/abs/2605.23993v2)**  
  Authors: Siqiao Huang, Partha Kaushik, Michael Chen, Hengkai Pan, Kaiwen Geng, Omar Chehab, Fernando Moreno-Pino, Max Simchowitz  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2605.23993v2.pdf)  
  Keywords: dit, evaluation, video prediction, world model, video generation, simulation, autoregressive, architecture, interactive  

### Video Super-Resolution & Enhancement

*Showing the latest 50 out of 72 papers*

- **[LongE2V: Long-Horizon Event-based Video Reconstruction, Prediction, and Frame Interpolation with Video Diffusion Models](https://arxiv.org/abs/2607.08770v1)**  
  Authors: Cheng-De Fan, Chun-Wei Tuan Mu, Chen-Wei Chang, Chin-Yang Lin, Kun-Ru Wu, Yu-Chee Tseng, Yu-Lun Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.08770v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://cdfan0627.github.io/LongE2V-page)  
  Keywords: frame interpolation, diffusion model, autoregressive, benchmark, video diffusion  
- **[OPSD-V: On-Policy Self-Distillation for Post-Training Few-Step Autoregressive Video Generators](https://arxiv.org/abs/2607.08766v1)**  
  Authors: Hongyu Liu, Chun Wang, Feng Gao, Xuanhua He, Yue Ma, Ziyu Wan, Yong Zhang, Xiaoming Wei, Qifeng Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.08766v1.pdf)  
  Keywords: distillation, dit, trajectory, denoising, dynamics, diffusion model, autoregressive, long video, video diffusion  
- **[OpenCoF: Learning to Reason Through Video Generation](https://arxiv.org/abs/2607.08763v1)**  
  Authors: Xinyan Chen, Ziyu Guo, Renrui Zhang, Dongzhi Jiang, Hongsheng Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.08763v1.pdf)  
  Keywords: i2v, benchmark, video generation, denoising  
- **[Dynamic-in-Few-Step: Unifying Dynamic Computation and Few-Step Distillation for Efficient Video Generation](https://arxiv.org/abs/2607.06631v1)**  
  Authors: Yu Cheng, Siyue Yao, Zhongang Qi, Shanyan Guan, Wei Li, Fajie Yuan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.06631v1.pdf)  
  Keywords: distillation, denoising, acceleration, architecture, diffusion model, video generation, efficient, video diffusion  
- **[MV-Forcing: Long Multi-View Video Generation via 4D-Grounded Spatio-Temporal Self-Forcing](https://arxiv.org/abs/2607.05376v1)**  
  Authors: Gal Fiebelman, Hadar Averbuch-Elor, Sagie Benaim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.05376v1.pdf)  
  Keywords: distillation, denoising, diffusion model, video generation, autoregressive, video diffusion, multi-view video  
- **[Enhancing Video Physical Consistency via Role-aware Joint Training and Modality-decoupled Denoising](https://arxiv.org/abs/2607.04653v2)**  
  Authors: Guangting Zheng, Haojing Chen, Hao Li, Jingtao Zhang, Zhen Yang, Xiaosong Jia, Xue Yang, Shaofeng Zhang, Yanyong Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.04653v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://tom-zgt.github.io/VPT)  
  Keywords: denoising, dynamics, diffusion model, physics, benchmark, video diffusion, physical, t2v  
- **[CineMobile: On-Device Image-to-Video Diffusion for Cinematic Camera Motion Generation](https://arxiv.org/abs/2607.03803v1)**  
  Authors: Xuyao Huang, Zelai Deng, Xu Wang, Xizhong Xiao, Zhijie Deng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.03803v1.pdf)  
  Keywords: distillation, dit, diffusion transformer, denoising, architecture, video generation, efficient, image-to-video, video diffusion  
- **[Flex-Forcing: Towards a Unified Autoregressive and Bidirectional Video Diffusion Model](https://arxiv.org/abs/2607.03509v1)**  
  Authors: Xinyin Ma, Julius Berner, Chao Liu, Arash Vahdat, Weili Nie, Xinchao Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.03509v1.pdf)  
  Keywords: streaming, denoising, diffusion model, video generation, efficient, autoregressive, benchmark, video diffusion  
- **[HyperVAttention: Efficient Sparse Attention with Spatio-Temporal Clustering for Video Diffusion](https://arxiv.org/abs/2607.03012v1)**  
  Authors: Dongyeun Lee, Amir Zandieh, Vahab Mirrokni, Junmo Kim, Insu Han  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.03012v1.pdf)  
  Keywords: dit, diffusion transformer, denoising, video generation, efficient, text-to-video, video diffusion  
- **[Track the Noise, Move the World:3D-Grounded Motion-Consistent Noise for Controllable Video Generation](https://arxiv.org/abs/2607.02798v1)**  
  Authors: Long Vu, Tan Ngo, Animesh Karnewar, Amir Habibian, Binh-Son Hua, Hung Bui, Minh Hoai Nguyen, Phong Nguyen-Ha  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.02798v1.pdf)  
  Keywords: motion control, temporal consistency, dit, latent video, denoising, diffusion model, video generation, text-to-video, benchmark, video diffusion, controllable  

### World Models & Simulation

*Showing the latest 50 out of 129 papers*

- **[Unlocking Temporal Generalization in Hamiltonian Video Dynamics Models](https://arxiv.org/abs/2607.07763v1)**  
  Authors: Eli Laird, Corey Clark  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.07763v1.pdf)  
  Keywords: dynamics, video generation, physical, world model  
- **[Validate the Dream Before You Trust Its Verdict: Admissibility for World-Model Simulators](https://arxiv.org/abs/2607.07196v1)**  
  Authors: Christian Oefinger, Finn Rasmus Schäfer, Korbinian Moller, Mattia Piccinini, Johannes Betz  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.07196v1.pdf)  
  Keywords: dit, world model, simulation, robotics, autonomous driving  
- **[Point as Skeleton: Accumulated Point Cloud Enhanced Autoregressive Generation for Closed-Loop Autonomous Driving Simulation](https://arxiv.org/abs/2607.06516v1)**  
  Authors: Songbur Wong, Xiaosong Jia, Junqi You, Bo Zhang, Pei Xu, Renqiu Xia, Yuping Qiu, Shaofeng Zhang, Zelin Zhao, Xuechao Yan, Yuchen Zhou, Yurui Chen, Wen Guo, Hang Xu, Junchi Yan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.06516v1.pdf) | [![GitHub](https://img.shields.io/github/stars/krauwu/point-as-skeleton?style=social)](https://github.com/krauwu/point-as-skeleton)  
  Keywords: dit, video generation, simulation, autoregressive, autonomous driving  
- **[A Definition and Roadmap for World Models](https://arxiv.org/abs/2607.06401v1)**  
  Authors: Xinyuan Chen, Haoyu Guo, Shi Guo, Bingqi Jiang, Chunhua Shen, Xing Shen, Tianfan Xue, Yufei Xue, Mulin Yu, Weinan Zhang, Bin Zhao, Bowen Zhou, Ming Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.06401v1.pdf)  
  Keywords: dynamics, world model, video generation, robotics, concept, physical  
- **[Benchmarking the Robustness of Autonomous Driving to Environmental Illusions: A Lane Perception Perspective](https://arxiv.org/abs/2607.05783v1)**  
  Authors: Tianyuan Zhang, Xianglong Liu, Aishan Liu, Lu Wang, Yitong Zhang, Peng Yue, Mingchuan Zhang, Siyuan Liang, Dacheng Tao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.05783v1.pdf)  
  Keywords: dit, evaluation, simulation, autonomous driving, benchmark, controllable  
- **[FORGE: Towards Functional Tool-Use Generalization via Keypoint Trajectory Reasoning](https://arxiv.org/abs/2607.05780v1)**  
  Authors: Chuhao Zhou, Liquan Wang, Shuxin Cao, Xiangyu Chen, Yuxuan Hu, Boyu Ma, Animesh Garg, Jianfei Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.05780v1.pdf)  
  Keywords: benchmark, simulation, trajectory  
- **[DSWAM: A Dual-System World Action Foundation Model for Fine-Grained Robot Manipulation](https://arxiv.org/abs/2607.04927v1)**  
  Authors: Jian Zhu, Jianjun Zhang, Taiyi Su, Tianbin Liu, Zhangyuan Wang, Kai Xie, Zitai Huang, Chong Ma, Youzhang He, Tianjian Wang, Hanyang Wang, Weihao Ding, Yi Xu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.04927v1.pdf)  
  Keywords: evaluation, acceleration, world model, video generation, physical  
- **[Mask2Real-WM: Segmentation Masks as a Sim-to-Real Bridge for Controllable Dexterous World Models](https://arxiv.org/abs/2607.04546v1)**  
  Authors: Riccardo O. Feingold, Davide Liconti, Chenyu Yang, Robert K. Katzschmann  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.04546v1.pdf)  
  Keywords: dit, evaluation, action-conditioned, physical, dynamics, world model, simulation, benchmark, video diffusion, controllable  
- **[Worldscape-MoE: A Unified Mixture-of-Experts World Model for Scalable Heterogeneous Action Control](https://arxiv.org/abs/2607.03964v1)**  
  Authors: Jianjie Fang, Yongyan Xu, Ziyou Wang, Chen Gao, Yuchao Huang, Zhaolu Wang, Rongze Tang, Mingyuan Jia, Baining Zhao, Weichen Zhang, Xin Zhang, Haisheng Su, Yu Shang, Wei Wu, Xinlei Chen, Yong Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.03964v1.pdf)  
  Keywords: dit, diffusion transformer, dynamics, world model, controllable, video generation, physical, interactive  
- **[G$^2$TAM: Geometry Grounded Track Anything Model](https://arxiv.org/abs/2607.03789v1)**  
  Authors: Chenming Zhu, Peizhou Cao, Jingli Lin, Wenbo Hu, Yunlong Ran, Jiangmiao Pang, Tai Wang, Xihui Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.03789v1.pdf)  
  Keywords: interactive, benchmark, evaluation, identity  



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
