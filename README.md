# Awesome Video Diffusions [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of latest research papers, projects and resources related to Video Diffusion Models and Video Generation. Content is automatically updated daily.

> Last Update: 2026-10-23 03:26:11

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

- [3D-aware Video Generation](#3d-aware-video-generation) (12 papers) - Video generation with 3D awareness, multi-view consistency, and 4D content creation
- [Applications](#applications) (34 papers) - Domain-specific applications of video diffusion models
- [Architecture & Efficiency](#architecture-&-efficiency) (370 papers) - Architectural innovations (DiT, UNet), flow matching, and training/inference efficiency
- [Audio & Multi-modal](#audio-&-multi-modal) (17 papers) - Audio-driven and multi-modal conditioned video generation
- [Controllable Generation](#controllable-generation) (125 papers) - Controllable video generation with motion, camera, pose, or layout guidance
- [Human & Character Animation](#human-&-character-animation) (16 papers) - Human-centric video generation including talking heads, dance, and character animation
- [Image-to-Video Generation](#image-to-video-generation) (43 papers) - Methods for animating still images into videos
- [Long Video Generation](#long-video-generation) (104 papers) - Generating temporally consistent long-form videos beyond short clips
- [Personalization & Customization](#personalization-&-customization) (62 papers) - Personalized video generation with custom subjects, identities, or styles
- [Physical Understanding](#physical-understanding) (134 papers) - Physics-aware video generation and dynamics modeling
- [Surveys & Benchmarks](#surveys-&-benchmarks) (245 papers) - Survey papers, benchmarks, and evaluation metrics for video generation
- [Text-to-Video Generation](#text-to-video-generation) (64 papers) - Foundation models and methods for generating videos from text prompts
- [Video Editing](#video-editing) (25 papers) - Diffusion-based video editing, style transfer, and manipulation
- [Video Inpainting & Completion](#video-inpainting-&-completion) (8 papers) - Video inpainting, completion, outpainting, and temporal prediction
- [Video Super-Resolution & Enhancement](#video-super-resolution-&-enhancement) (86 papers) - Video quality improvement, upscaling, restoration, and frame interpolation
- [World Models & Simulation](#world-models-&-simulation) (126 papers) - Video generation as world simulators and interactive environment generation



## Table of Contents

- [Categorized Papers](#categorized-papers)
- [Classic Papers](#classic-papers)
- [Open Source Projects](#open-source-projects)
- [Applications](#applications)
- [Tutorials & Blogs](#tutorials--blogs)





## Categorized Papers

### 3D-aware Video Generation

- **[Learning the 4D World through Point Trajectory Forecasting](https://arxiv.org/abs/2610.28594v1)**  
  Authors: Byungwoo Jeon, Sunghwan Hong, Dohyeon Kim, Jonghoon Lee, Jungwoo Park, Inhee Lee, Doosan Baek, Jinil Kim, Taehyun Lim, Hanbyul Joo, Marc Pollefeys, Saining Xie, Jinwoo Shin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.28594v1.pdf)  
  Keywords: benchmark, 4d generation, dit, evaluation, physical, simulation, video generation, 3d-aware, trajectory, multi-view video, world model  
- **[Mise-en-Video: Fine-Grained 3D Control for Multi-Shot Video Generation](https://arxiv.org/abs/2610.26801v1)**  
  Authors: Yingshuang Zou, Xiaoyu Shi, Yawen Luo, Ziang Li, Qinghe Wang, Mengfei Li, Chengfeng Zhao, Xintao Wang, Pengfei Wan, Kun Gai, Yuan Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.26801v1.pdf)  
  Keywords: layout, evaluation, text-to-video, video generation, 3d-aware, controllable  
- **[HORIA: 4D Human and Object Reconstruction from a Monocular Video with Interaction-Aware Re-Rendering](https://arxiv.org/abs/2610.25960v2)**  
  Authors: Hyeongjin Nam, Taeryung Lee, Daniel Sungho Jung, Kyoung Mu Lee  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.25960v2.pdf)  
  Keywords: video diffusion, text-to-video, dit, novel view  
- **[GeoV2V: Geometry-Grounded Video Diffusion Model for Driving Scene Generation](https://arxiv.org/abs/2610.25245v1)**  
  Authors: Yuchen Xi, Yuhan Guo, Chenwei Hou, Zixu Liu, Jin Fang, Jason Liu, Ruigang Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.25245v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://xiyuche.github.io/GeoV2V)  
  Keywords: video diffusion, dit, simulation, dynamics, trajectory, autonomous driving, video-to-video, novel view, diffusion model  
- **[GeoFix: Geometry Fixing for 4D Consistent Generation](https://arxiv.org/abs/2610.14293v1)**  
  Authors: Yeobin Hong, Hyojun Go, Dohun Lee, Jeongjae Lee, Sunghwan Hong, Federico Tombari, Zhaochong An, Jong Chul Ye, Konrad Schindler, Dominik Narnhofer  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.14293v1.pdf)  
  Keywords: video diffusion, 4d generation, diffusion model  
- **[LEGO: A Lifting-Free Approach for Exocentric-to-Egocentric Video Generation](https://arxiv.org/abs/2610.12442v1)**  
  Authors: Suhwan Cho, Yonwoo Choi, Soongjin Kim, Jicheol Park, Taegyu Lim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.12442v1.pdf)  
  Keywords: video diffusion, dit, denoising, layout, video generation, style, novel view, diffusion model  
- **[SepGen: Multi-Stem Audio-Video Separation and Generation in a Single Model](https://arxiv.org/abs/2610.11361v1)**  
  Authors: Aviad Dahan, Rajaei Khatib, Yonatan Bitton, Idan Szpektor, Lior Wolf, Raja Giryes  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.11361v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://sepgen.github.io)  
  Keywords: sound, trajectory, dit, novel view  
- **[GeoVerse: World-Consistent Novel View Synthesis in Geometric Latent Space](https://arxiv.org/abs/2609.35734v2)**  
  Authors: Kerui Ren, Tao Lu, Linning Xu, Changjian Jiang, Mu Huang, Chunhua Shen, Mulin Yu, Bo Dai  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.35734v2.pdf)  
  Keywords: style, novel view, diffusion model  
- **[GenNVS: Geometry-enhanced Novel View Synthesis via Disentangled 3D Prior](https://arxiv.org/abs/2609.34579v2)**  
  Authors: Yajiao Xiong, Youyu Luan, Xiaoyu Zhou, Yongtao Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.34579v2.pdf)  
  Keywords: video diffusion, dit, novel view, diffusion model  
- **[VGGT-Diff: Visual Geometry Meets Diffusion for Sparse-View Novel View Synthesis](https://arxiv.org/abs/2609.33253v2)**  
  Authors: Kangjie Chen, Xiangyu Li, Dongbin Zhang, Chaoda Zheng, Shijia Chen, Jinhao Deng, Hongbin Lin, Choo Sin Wai, Minqi Wang, Minghao Yang, Dake Zhong, Guorui Song, Yu Zhang, Xianming Liu, Boyang Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.33253v2.pdf) | [![GitHub](https://img.shields.io/github/stars/chenkangjie1123/VGGT-Diff?style=social)](https://github.com/chenkangjie1123/VGGT-Diff)  
  Keywords: video diffusion, dit, denoising, novel view, diffusion model  

### Applications

- **[CineEvolve: An Agentic Self-Evolution Framework for Cinematic Multi-Shot Video Generation](https://arxiv.org/abs/2610.29590v1)**  
  Authors: Jingzhe Zhang, Peixuan Zhang, Genying Li, Bing Ma, Shuchen Weng, Si Li, Boxin Shi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.29590v1.pdf) | [![GitHub](https://img.shields.io/github/stars/JingZhe-8/CineEvolve?style=social)](https://github.com/JingZhe-8/CineEvolve)  
  Keywords: film, trajectory, dit, video generation  
- **[HorizonComposer: Spatiotemporally Consistent Driving Video Editing with Enriched Traffic Semantics](https://arxiv.org/abs/2610.28829v1)**  
  Authors: Mauricio Soroco, Yuqiu Liu, Zaid Tasneem, Francesco Pittaluga, Abhishek Aich, Wuyang Chen, Manmohan Chandraker, Ziyu Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.28829v1.pdf)  
  Keywords: dit, temporal consistency, dynamics, autonomous driving, video editing  
- **[Code2Video-Compass: A Comprehensive Benchmark for General-Purpose Code-Based Video Generation across T2V, I2V, and V2V](https://arxiv.org/abs/2610.28416v1)**  
  Authors: Zhenghan Chen, Zekai Shao, Xin Lin, Leting Cheng, Siming Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.28416v1.pdf)  
  Keywords: benchmark, dit, creative, evaluation, text-to-video, video generation, t2v, i2v, image-to-video, controllable, video-to-video  
- **[Wan-Alpha++: Animating a Single RGBA Asset into Controllable Transparent Video Effects](https://arxiv.org/abs/2610.26189v1)**  
  Authors: Haotian Dong, Xin Wang, Wenjing Wang, Chen Li, Jing Lyu, Yan Tina Luximon, Ping Li, Wanchao Su, Ke Xu, Di Lin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.26189v1.pdf)  
  Keywords: video diffusion, dit, video generation, image-to-video, controllable, film  
- **[MAPS: A Multi-Agent Personalized Script-Driven Video Advertising System Enhanced by Reinforcement Learning](https://arxiv.org/abs/2610.25748v1)**  
  Authors: Zhongyu Wang, Chen Zuo, Qingxuan Sun, Jiayang Qiao, Qiuhao Qian, Songyan Cui, Guocheng Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.25748v1.pdf)  
  Keywords: personalization, advertising, video synthesis, creative  
- **[Painting Change Map as guidance for generating painting processes](https://arxiv.org/abs/2610.25369v2)**  
  Authors: Markus Pobitzer, Chang Liu, Niccolò Biondi, Nicu Sebe  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.25369v2.pdf) | [![GitHub](https://img.shields.io/github/stars/Markus-Pobitzer/painting-change-map?style=social)](https://github.com/Markus-Pobitzer/painting-change-map)  
  Keywords: benchmark, creative, dit, video generation  
- **[GeoV2V: Geometry-Grounded Video Diffusion Model for Driving Scene Generation](https://arxiv.org/abs/2610.25245v1)**  
  Authors: Yuchen Xi, Yuhan Guo, Chenwei Hou, Zixu Liu, Jin Fang, Jason Liu, Ruigang Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.25245v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://xiyuche.github.io/GeoV2V)  
  Keywords: video diffusion, dit, simulation, dynamics, trajectory, autonomous driving, video-to-video, novel view, diffusion model  
- **[BodyBridge: Grounded Body Layers for Sim-to-Real Translation of Vulnerable Road Users](https://arxiv.org/abs/2610.24436v1)**  
  Authors: Mark Azer, Fabian B. Flohr  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.24436v1.pdf)  
  Keywords: video diffusion, dit, evaluation, simulation, identity, autonomous driving, diffusion model  
- **[OmniXRef: A Unified Framework for Multimodal Multi-Reference Video Editing](https://arxiv.org/abs/2610.22744v1)**  
  Authors: Xiaoyan Cong, Tianyu Wang, Hyeonho Jeong, Zhifei Zhang, Yuqian Zhou, Yijun Li, Shaoteng Liu, Zhe Lin, Srinath Sridhar, Soo Ye Kim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.22744v1.pdf)  
  Keywords: diffusion transformer, benchmark, dit, creative, evaluation, video editing, style  
- **[Any Time, Any Space: A World-State-Centric Framework for Agentic Video Generation](https://arxiv.org/abs/2610.20571v1)**  
  Authors: Weijie Wang, Haomin Zhang, Ye Li, Akide Liu, Zeyu Zhang, Haoyu Zhao, Yefei He, Donny Y. Chen, Feng Chen, Bohan Zhuang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.20571v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://lhmd.top/atas)  
  Keywords: benchmark, film, long-form, video generation  

### Architecture & Efficiency

*Showing the latest 50 out of 370 papers*

- **[WorldForge V2: Eliciting Camera-Trajectory Alignment in Video Diffusion Models](https://arxiv.org/abs/2610.31640v1)**  
  Authors: Chenxi Song, Yanming Yang, Tong Zhao, Ruibo Li, Joey Tianyi Zhou, Chi Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.31640v1.pdf)  
  Keywords: video diffusion, dit, denoising, evaluation, camera control, dynamics, video generation, trajectory, motion control, diffusion model  
- **[AnyGameRenderer: Entity-Consistent Generative Rendering Across Games and an Entity-Level Benchmark](https://arxiv.org/abs/2610.31466v1)**  
  Authors: Ruicong Liu, Liangyang Ouyang, Fengbo Lan, Zhixiang Wang, Kaipeng Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.31466v1.pdf)  
  Keywords: benchmark, dit, layout, video generation, video-to-video  
- **[PhysTrace: Interpretable Temporal Evaluation of Physical Consistency in Video Generative Models](https://arxiv.org/abs/2610.31429v1)**  
  Authors: Taekoan Yoo, Wonkyung Jung, Kyunghun Kim, Kyeongbo Kong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.31429v1.pdf)  
  Keywords: physical, dit, dynamics, evaluation  
- **[Making MLLM Latents Matter: Factor-Aware Predictive Learning for Cinematic Video Generation](https://arxiv.org/abs/2610.30926v1)**  
  Authors: Songlin Yang, Zhe Wang, Xiaotong Zhao, Xi Wang, Ran Zhang, Shuai Li, Taiyi Wu, Songlian Li, Eric Liu, Alan Zhao, Anyi Rao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.30926v1.pdf)  
  Keywords: video diffusion, dit, video generation, diffusion transformer  
- **[DeXplicit: Making Physical State Explicit in Dexterous Manipulation World Models](https://arxiv.org/abs/2610.30781v1)**  
  Authors: Adam Lee, Mutian Xu, Yukang Cao, Shulin Tian, Ziwei Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.30781v1.pdf)  
  Keywords: dit, denoising, physical, dynamics, video generation, trajectory, video synthesis, efficient, world model, action-conditioned  
- **[Learning from Next-Frame Prediction: Towards Unified and Scalable Visual Representation Learning](https://arxiv.org/abs/2610.30724v1)**  
  Authors: Yifeng Yao, Jinghan Li, Zhihao Zhang, Yajiao Xiong, Yang Jin, Kun Xu, Huishuai Zhang, Dongyan Zhao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.30724v1.pdf)  
  Keywords: benchmark, world model, autoregressive, dit  
- **[Latent Space Jam: Layout Guided Video Synthesis](https://arxiv.org/abs/2610.30390v1)**  
  Authors: Asaf Joseph, Moshe Mandel, Ohad Fried  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.30390v1.pdf)  
  Keywords: video diffusion, dit, layout, temporal consistency, video generation, trajectory, video synthesis, diffusion model  
- **[Self-Distilling Future Video Representations for World Action Models](https://arxiv.org/abs/2610.30320v1)**  
  Authors: Huiwon Jang, Suhyeok Jang, Hyeonmo Kang, Seungku Kim, Jinwoo Shin, Sihyun Yu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.30320v1.pdf)  
  Keywords: video diffusion, dit, denoising, video generation, distillation, diffusion model  
- **[Looking Ahead: Modeling Future Evolution in Autoregressive Video Generation](https://arxiv.org/abs/2610.29989v1)**  
  Authors: Ruopeng Gao, Yukun Huang, Jiarui Hu, Shuai Wang, Wenbo Hu, Ying Shan, Limin Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.29989v1.pdf)  
  Keywords: video diffusion, autoregressive, denoising, dit, physical, video generation, world model, diffusion model  
- **[CineEvolve: An Agentic Self-Evolution Framework for Cinematic Multi-Shot Video Generation](https://arxiv.org/abs/2610.29590v1)**  
  Authors: Jingzhe Zhang, Peixuan Zhang, Genying Li, Bing Ma, Shuchen Weng, Si Li, Boxin Shi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.29590v1.pdf) | [![GitHub](https://img.shields.io/github/stars/JingZhe-8/CineEvolve?style=social)](https://github.com/JingZhe-8/CineEvolve)  
  Keywords: film, trajectory, dit, video generation  

### Audio & Multi-modal

- **[SonoWorld: Towards Interactive Pose-Controllable Ultrasound World Models](https://arxiv.org/abs/2610.19327v2)**  
  Authors: Zefan Yang, Zheyuan Zhang, Boris Maihe, Yikang Liu, Hang Yu, Ankush Mukherjee, Xiao Chen, Pingkun Yan, Terrence Chen, Shanhui Sun  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.19327v2.pdf)  
  Keywords: video diffusion, autoregressive, dit, evaluation, action-conditioned, simulation, interactive, dynamics, controllable, distillation, sound, world model, diffusion model  
- **[Kandinsky S2V 1.0: Audio-Driven Avatar Video Generation](https://arxiv.org/abs/2610.19290v1)**  
  Authors: Nikolay Semenov, Artem Riabinin, Sergey Bassenko, Anna Averchenkova, Julia Agafonova, Anastasia Aliaskina, Kirill Kozlov, Lev Novitskiy, Nikita Samsonov, Nikolai Gerasimenko, Denis Dimitrov  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.19290v1.pdf)  
  Keywords: benchmark, dit, architecture, layout, evaluation, video generation, audio-driven, long-form, gesture, controllable, human animation, avatar  
- **[Structured Stateful Relational Scripts with a High-Quality Dataset for Multi-Shot Audio-Visual Video Generation](https://arxiv.org/abs/2610.15512v1)**  
  Authors: Chen Zhao, Lehan Shen, Qilong Huang, Hongyu Li, Zhuoliang Kang, Xiaoming Wei, Jian Yang, Ying Tai  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.15512v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://huggingface.co/datasets/shenlehan/MSAV-Script-100K}{MSAV-Script-100K}.) | [![Dataset](https://img.shields.io/badge/-Dataset-orange)](https://huggingface.co/datasets/shenlehan/MSAV-Script-100K)  
  Keywords: sound, identity, dit, video generation  
- **[CatPortrait: Taming Video Generative Models for Portrait Animation via In-context Conditioning](https://arxiv.org/abs/2610.14957v1)**  
  Authors: Ziqi Ni, Zhou Fang, Shijian Wang, Rui Li, Yi Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.14957v1.pdf)  
  Keywords: dit, video generation, audio-driven, image-to-video, controllable  
- **[PAGE: Parts-Aware Guidance for Co-Speech Gesture Portrait Video Generation](https://arxiv.org/abs/2610.13301v1)**  
  Authors: Yabiao Wang, Jiafu Wu, Yicheng Xu, Teng Hu, Shengzhe Zhou, Yanxiao Sun, Jiangning Zhang, Ying Tai, Yong Liu, Ming-Hsuan Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.13301v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://aigc-explorer.github.io/PAGE)  
  Keywords: benchmark, dit, denoising, evaluation, video generation, audio-driven, trajectory, gesture, body motion, efficient  
- **[SepGen: Multi-Stem Audio-Video Separation and Generation in a Single Model](https://arxiv.org/abs/2610.11361v1)**  
  Authors: Aviad Dahan, Rajaei Khatib, Yonatan Bitton, Idan Szpektor, Lior Wolf, Raja Giryes  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.11361v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://sepgen.github.io)  
  Keywords: sound, trajectory, dit, novel view  
- **[PVSync: A Unified Lip-Sync Expert for Timing and Articulation](https://arxiv.org/abs/2610.09223v1)**  
  Authors: Kevin Stephen, Varun Menon, Timo Mertens, Nikita Drobyshev  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.09223v1.pdf)  
  Keywords: benchmark, sound, video generation  
- **[AiSearch: Interactive Multi-Modal Search with VLMs](https://arxiv.org/abs/2610.01389v1)**  
  Authors: Ali Koksal, Mei Chee Leong, Vicky Sintunata, Ching Ling Chin, Wee Teck Fong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.01389v1.pdf)  
  Keywords: benchmark, interactive, multi-modal  
- **[Watch Your Speech: Text-aware Video-to-Speech Synthesis with Textual Conditioning](https://arxiv.org/abs/2610.01012v1)**  
  Authors: Gunwoo Lee, Yoori Oh, Yoseob Han  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.01012v1.pdf) | [![GitHub](https://img.shields.io/github/stars/gunwoo5034/Watch-your-Speech?style=social)](https://github.com/gunwoo5034/Watch-your-Speech)  
  Keywords: dit, evaluation, dynamics, flow matching, sound  
- **[Soundwich: Video Generation with Layered and Controllable Audio](https://arxiv.org/abs/2610.00691v2)**  
  Authors: Zhuo Ning, AmirHossein Naghi Razlighi, Sagi Polaczek, Daniel Cohen-Or, Ali Mahdavi-Amiri  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.00691v2.pdf) | [![GitHub](https://img.shields.io/github/stars/CodyNing/Soundwich?style=social)](https://github.com/CodyNing/Soundwich)  
  Keywords: dit, evaluation, video generation, controllable, sound  

### Controllable Generation

*Showing the latest 50 out of 125 papers*

- **[WorldForge V2: Eliciting Camera-Trajectory Alignment in Video Diffusion Models](https://arxiv.org/abs/2610.31640v1)**  
  Authors: Chenxi Song, Yanming Yang, Tong Zhao, Ruibo Li, Joey Tianyi Zhou, Chi Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.31640v1.pdf)  
  Keywords: video diffusion, dit, denoising, evaluation, camera control, dynamics, video generation, trajectory, motion control, diffusion model  
- **[AnyGameRenderer: Entity-Consistent Generative Rendering Across Games and an Entity-Level Benchmark](https://arxiv.org/abs/2610.31466v1)**  
  Authors: Ruicong Liu, Liangyang Ouyang, Fengbo Lan, Zhixiang Wang, Kaipeng Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.31466v1.pdf)  
  Keywords: benchmark, dit, layout, video generation, video-to-video  
- **[DeXplicit: Making Physical State Explicit in Dexterous Manipulation World Models](https://arxiv.org/abs/2610.30781v1)**  
  Authors: Adam Lee, Mutian Xu, Yukang Cao, Shulin Tian, Ziwei Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.30781v1.pdf)  
  Keywords: dit, denoising, physical, dynamics, video generation, trajectory, video synthesis, efficient, world model, action-conditioned  
- **[Latent Space Jam: Layout Guided Video Synthesis](https://arxiv.org/abs/2610.30390v1)**  
  Authors: Asaf Joseph, Moshe Mandel, Ohad Fried  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.30390v1.pdf)  
  Keywords: video diffusion, dit, layout, temporal consistency, video generation, trajectory, video synthesis, diffusion model  
- **[RealMe: Immersive Volumetric Video from Minimal Captures](https://arxiv.org/abs/2610.30023v1)**  
  Authors: Chenxu Zhou, Zhiyuan Yu, Yudong Jin, Yinji Shentu, Yu Zhang, Jiaming Sun, Xiaowei Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.30023v1.pdf)  
  Keywords: video diffusion, benchmark, layout, dynamics, diffusion model  
- **[CineEvolve: An Agentic Self-Evolution Framework for Cinematic Multi-Shot Video Generation](https://arxiv.org/abs/2610.29590v1)**  
  Authors: Jingzhe Zhang, Peixuan Zhang, Genying Li, Bing Ma, Shuchen Weng, Si Li, Boxin Shi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.29590v1.pdf) | [![GitHub](https://img.shields.io/github/stars/JingZhe-8/CineEvolve?style=social)](https://github.com/JingZhe-8/CineEvolve)  
  Keywords: film, trajectory, dit, video generation  
- **[Sparsity Should Be ALLOTted by Output: Training-Free Allocation of Block-Sparse Attention for Video Diffusion Transformers](https://arxiv.org/abs/2610.29441v1)**  
  Authors: Tianze Xia, Xiaoling Zhou, Ruya Lan, Yiqiao Liao, Chengru Song, Shiming Xiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.29441v1.pdf)  
  Keywords: video diffusion, diffusion transformer, dit, denoising, trajectory  
- **[Pair-Free Coarse-to-Real Video Generation via Real-to-Coarse Image Supervision](https://arxiv.org/abs/2610.28954v1)**  
  Authors: Gonzalo Gómez-Nogales, Daohan Lu, Peiye Zhuang, Tinghui Zhou, Yi Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.28954v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://gonzalognogales.github.io/coarse2real-sharp)  
  Keywords: dit, layout, simulation, dynamics, video generation  
- **[Learning the 4D World through Point Trajectory Forecasting](https://arxiv.org/abs/2610.28594v1)**  
  Authors: Byungwoo Jeon, Sunghwan Hong, Dohyeon Kim, Jonghoon Lee, Jungwoo Park, Inhee Lee, Doosan Baek, Jinil Kim, Taehyun Lim, Hanbyul Joo, Marc Pollefeys, Saining Xie, Jinwoo Shin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.28594v1.pdf)  
  Keywords: benchmark, 4d generation, dit, evaluation, physical, simulation, video generation, 3d-aware, trajectory, multi-view video, world model  
- **[Code2Video-Compass: A Comprehensive Benchmark for General-Purpose Code-Based Video Generation across T2V, I2V, and V2V](https://arxiv.org/abs/2610.28416v1)**  
  Authors: Zhenghan Chen, Zekai Shao, Xin Lin, Leting Cheng, Siming Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.28416v1.pdf)  
  Keywords: benchmark, dit, creative, evaluation, text-to-video, video generation, t2v, i2v, image-to-video, controllable, video-to-video  

### Human & Character Animation

- **[StreamEval: Evaluating Interactive Streaming Video Generation Models](https://arxiv.org/abs/2610.28402v1)**  
  Authors: StreamEval Team  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.28402v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://streameval.ai)  
  Keywords: benchmark, dit, evaluation, streaming, interactive, video generation, identity, avatar  
- **[Video Diffusion Avatars: Taming Video Diffusion Models into Controllable 3D Avatars](https://arxiv.org/abs/2610.23772v1)**  
  Authors: Simon Giebenhain, Tobias Kirschstein, Liam Schoneveld, Davide Davoli, Zhe Chen, Matthias Nießner  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.23772v1.pdf)  
  Keywords: video diffusion, benchmark, physical, dynamics, physics, controllable, efficient, avatar, diffusion model  
- **[DreamHMR: From Video Generation to Human Motion Modeling via Structural Focusing](https://arxiv.org/abs/2610.20124v1)**  
  Authors: Zhengjie Xu, Ruihao Gong, Xianglong Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.20124v1.pdf)  
  Keywords: body motion, human motion, video generation, evaluation  
- **[Kandinsky S2V 1.0: Audio-Driven Avatar Video Generation](https://arxiv.org/abs/2610.19290v1)**  
  Authors: Nikolay Semenov, Artem Riabinin, Sergey Bassenko, Anna Averchenkova, Julia Agafonova, Anastasia Aliaskina, Kirill Kozlov, Lev Novitskiy, Nikita Samsonov, Nikolai Gerasimenko, Denis Dimitrov  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.19290v1.pdf)  
  Keywords: benchmark, dit, architecture, layout, evaluation, video generation, audio-driven, long-form, gesture, controllable, human animation, avatar  
- **[JtT: Rethinking Point Trajectory Diffusion for Diverse and Rigid Motion from an Image](https://arxiv.org/abs/2610.16591v1)**  
  Authors: Gabrijel Boduljak, Yushi Lan, Christian Rupprecht, Andrea Vedaldi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.16591v1.pdf)  
  Keywords: diffusion transformer, dit, architecture, evaluation, physical, trajectory, body motion  
- **[PAGE: Parts-Aware Guidance for Co-Speech Gesture Portrait Video Generation](https://arxiv.org/abs/2610.13301v1)**  
  Authors: Yabiao Wang, Jiafu Wu, Yicheng Xu, Teng Hu, Shengzhe Zhou, Yanxiao Sun, Jiangning Zhang, Ying Tai, Yong Liu, Ming-Hsuan Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.13301v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://aigc-explorer.github.io/PAGE)  
  Keywords: benchmark, dit, denoising, evaluation, video generation, audio-driven, trajectory, gesture, body motion, efficient  
- **[Golden Anchor for Video Generation](https://arxiv.org/abs/2610.13217v2)**  
  Authors: Jinyuan Xu, Shitong Shao, Lichen Bai, Zikai Zhou, Guoxi Huang, Nantheera Anantrasirichai, Zeke Xie  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.13217v2.pdf)  
  Keywords: interactive, video generation, i2v, image-to-video, identity, film, avatar, style, world model  
- **[PixReenact: Pixel-Conditioned Causal Video Diffusion for Streaming Head-Avatar Reenactment](https://arxiv.org/abs/2610.05233v1)**  
  Authors: Gavriel Habib, Dvir Samuel, Or Shimshi, Rami Ben-Ari  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.05233v1.pdf)  
  Keywords: video diffusion, benchmark, autoregressive, denoising, dit, streaming, identity, distillation, avatar  
- **[Parasitic Co-Denoising: Unlocking 3D Human Motion Generation in a Frozen Video Diffusion Model](https://arxiv.org/abs/2610.03047v1)**  
  Authors: Yunjiao Zhou, Junlang Qian, Lihua Xie, Jianfei Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03047v1.pdf)  
  Keywords: video diffusion, denoising, text-to-video, human motion, efficient, diffusion model  
- **[GLARE: Generating Listening Heads with Appropriate Reactions](https://arxiv.org/abs/2609.40317v1)**  
  Authors: Zikai Liao, Yumin Suh, Yi Ouyang, Yi-Lun Lee, Yi-Hsuan Tsai, Zhaozheng Yin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.40317v1.pdf)  
  Keywords: talking head, dit, evaluation, audio-driven, video generation  

### Image-to-Video Generation

- **[Latent Bridge: From Video Latents to 3D Geometry via Feature Alignment](https://arxiv.org/abs/2610.28521v1)**  
  Authors: Shuai Zhang, Zhanpeng Ouyang, Zhengqing Chen, Ruohong Mei, Shaoyu Chen, Weiqiang Ren, Hui Sun, Qian Zhang, Wenyu Liu, Xinggang Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.28521v1.pdf) | [![GitHub](https://img.shields.io/github/stars/hustvl/Latent-Bridge?style=social)](https://github.com/hustvl/Latent-Bridge)  
  Keywords: text-to-video, video generation, image-to-video, distillation, efficient  
- **[Code2Video-Compass: A Comprehensive Benchmark for General-Purpose Code-Based Video Generation across T2V, I2V, and V2V](https://arxiv.org/abs/2610.28416v1)**  
  Authors: Zhenghan Chen, Zekai Shao, Xin Lin, Leting Cheng, Siming Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.28416v1.pdf)  
  Keywords: benchmark, dit, creative, evaluation, text-to-video, video generation, t2v, i2v, image-to-video, controllable, video-to-video  
- **[PVBench: Quantifying Physical Plausibility in Video Generation with Object-Level Physical Measurements](https://arxiv.org/abs/2610.26711v1)**  
  Authors: Kaiwei Chen, Moran Li, Zhenye Gan, Yabiao Wang, Chengjie Wang, Kexin Zhang, Yong Liu, Jiangning Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.26711v1.pdf)  
  Keywords: benchmark, evaluation, physical, text-to-video, dynamics, video generation, image-to-video, world model  
- **[Wan-Alpha++: Animating a Single RGBA Asset into Controllable Transparent Video Effects](https://arxiv.org/abs/2610.26189v1)**  
  Authors: Haotian Dong, Xin Wang, Wenjing Wang, Chen Li, Jing Lyu, Yan Tina Luximon, Ping Li, Wanchao Su, Ke Xu, Di Lin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.26189v1.pdf)  
  Keywords: video diffusion, dit, video generation, image-to-video, controllable, film  
- **[ViMoLa: Discrete Motion Tokens for Language-Guided Video Generation](https://arxiv.org/abs/2610.25595v1)**  
  Authors: Bishoy Galoaa, Sarah Ostadabbas  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.25595v1.pdf)  
  Keywords: image-to-video, dit, video generation  
- **[MotionShift: Environment-Compatible Motion Transfer via Planner-Evaluator Synergistic Adaptation](https://arxiv.org/abs/2610.25290v1)**  
  Authors: Yanchen Liu, Junyao Gao, Yanan Sun, Wensheng Chen, Guangming Lu, Wenjie Pei  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.25290v1.pdf)  
  Keywords: dit, physical, i2v, image-to-video, trajectory  
- **[Meta Inverse Prompting for Video Generative Models](https://arxiv.org/abs/2610.24965v1)**  
  Authors: Yerin Jung, Jongheon Jeong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.24965v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://ueriniuno.github.io/mvip-page)  
  Keywords: dit, text-to-video, dynamics, image-to-video, controllable, efficient  
- **[CorrFlow: Self-Correcting Flow Matching](https://arxiv.org/abs/2610.24750v1)**  
  Authors: Hangwei Zhang, Nathan Rouillé, Chuanxia Zheng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.24750v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://fogradio.github.io/corrflow-project) | [![Demo](https://img.shields.io/badge/-Demo-brightgreen)](https://fogradio.github.io/corrflow-project)  
  Keywords: dit, evaluation, physical, text-to-video, video generation, identity, image-to-video, flow matching  
- **[Learning to Correct Geometry in Generated Videos](https://arxiv.org/abs/2610.23856v1)**  
  Authors: Weijie Lyu, Tiancheng Shen, Jason Li, Yujing Wang, Xiaoyuan Wang, Haobo Yuan, Yizhou Zhao, Ming-Hsuan Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.23856v1.pdf)  
  Keywords: benchmark, dit, image-to-video, trajectory, video-to-video, video inpainting  
- **[I2V-DETACH: Source Grounding Detachment for Unauthorized Image-to-Video Generation](https://arxiv.org/abs/2610.23287v1)**  
  Authors: Chanhui Lee, Yeonghwan Song, Yewon Kang, Jeany Son  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.23287v1.pdf)  
  Keywords: dit, denoising, architecture, dynamics, video generation, i2v, image-to-video, diffusion model  

### Long Video Generation

*Showing the latest 50 out of 104 papers*

- **[Direct Forcing: A Single-Stage Training Recipe for Few-Step Autoregressive Text-to-Video Generation](https://arxiv.org/abs/2610.30861v1)**  
  Authors: Haojun Xu, Jie Huang, Xin Lu, Mingchen Zhong, Zihao Fan, Linjiang Huang, Si Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.30861v1.pdf)  
  Keywords: text-to-video, streaming, autoregressive, video generation  
- **[Learning from Next-Frame Prediction: Towards Unified and Scalable Visual Representation Learning](https://arxiv.org/abs/2610.30724v1)**  
  Authors: Yifeng Yao, Jinghan Li, Zhihao Zhang, Yajiao Xiong, Yang Jin, Kun Xu, Huishuai Zhang, Dongyan Zhao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.30724v1.pdf)  
  Keywords: benchmark, world model, autoregressive, dit  
- **[Latent Space Jam: Layout Guided Video Synthesis](https://arxiv.org/abs/2610.30390v1)**  
  Authors: Asaf Joseph, Moshe Mandel, Ohad Fried  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.30390v1.pdf)  
  Keywords: video diffusion, dit, layout, temporal consistency, video generation, trajectory, video synthesis, diffusion model  
- **[Attn-Forcing: Learning Full-Context Attention Proxies for Streaming Video Generation](https://arxiv.org/abs/2610.30036v1)**  
  Authors: Junyao Gao, Sibo Liu, Jiaxing Li, Yanan Sun, Hanxin Zhu, Weidong Zhang, Jun Zhang, Cairong Zhao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.30036v1.pdf)  
  Keywords: streaming, video generation  
- **[Looking Ahead: Modeling Future Evolution in Autoregressive Video Generation](https://arxiv.org/abs/2610.29989v1)**  
  Authors: Ruopeng Gao, Yukun Huang, Jiarui Hu, Shuai Wang, Wenbo Hu, Ying Shan, Limin Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.29989v1.pdf)  
  Keywords: video diffusion, autoregressive, denoising, dit, physical, video generation, world model, diffusion model  
- **[HorizonComposer: Spatiotemporally Consistent Driving Video Editing with Enriched Traffic Semantics](https://arxiv.org/abs/2610.28829v1)**  
  Authors: Mauricio Soroco, Yuqiu Liu, Zaid Tasneem, Francesco Pittaluga, Abhishek Aich, Wuyang Chen, Manmohan Chandraker, Ziyu Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.28829v1.pdf)  
  Keywords: dit, temporal consistency, dynamics, autonomous driving, video editing  
- **[StreamEval: Evaluating Interactive Streaming Video Generation Models](https://arxiv.org/abs/2610.28402v1)**  
  Authors: StreamEval Team  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.28402v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://streameval.ai)  
  Keywords: benchmark, dit, evaluation, streaming, interactive, video generation, identity, avatar  
- **[Offline Makes Online Better: Calibrated Cache Compression for Video Generation](https://arxiv.org/abs/2610.28192v1)**  
  Authors: Zhen Wang, Ning Lai, Qingtao Yu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.28192v1.pdf)  
  Keywords: efficient, autoregressive, video generation  
- **[MoDDiT: Simple Token Routing in Diffusion Transformers](https://arxiv.org/abs/2610.28086v1)**  
  Authors: Jarek Liesen, Matthew T. Jackson, Benjamin Ellis, Shimon Whiteson, Jakob N. Foerster  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.28086v1.pdf)  
  Keywords: diffusion transformer, autoregressive, denoising, dit, architecture, interactive, video generation, world model  
- **[Recast the Past: Stable Long Video Generation with Full Context Memory](https://arxiv.org/abs/2610.27986v1)**  
  Authors: Yukuo Ma, Cong Liu, Junke Wang, Junqi Liu, Haibin Huang, Zuxuan Wu, Xuelong Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.27986v1.pdf)  
  Keywords: diffusion transformer, autoregressive, denoising, dit, long video, video generation  

### Personalization & Customization

*Showing the latest 50 out of 62 papers*

- **[HumanCentric-Scenes-AI: A Human-Curated Multimodal Dataset of AI-Generated Human-Centric Scenes Across Surveillance, Occupational Portraits, AI-Edited Images, and Short-Form Video](https://arxiv.org/abs/2610.29045v1)**  
  Authors: Nima Kamali, Sana Nasiri, Negar Kamali  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.29045v1.pdf)  
  Keywords: dit, style  
- **[Copyright Leakage Detection in AI Generated Videos](https://arxiv.org/abs/2610.28524v1)**  
  Authors: Shaif Chowdhury, Moshiur Rahman Tonmoy  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.28524v1.pdf) | [![GitHub](https://img.shields.io/github/stars/Shaif95/video-cp-Leakage?style=social)](https://github.com/Shaif95/video-cp-Leakage) | [![Project](https://img.shields.io/badge/-Project-blue)](https://zenodo.org/records/21386117)  
  Keywords: benchmark, video generation, concept  
- **[StreamEval: Evaluating Interactive Streaming Video Generation Models](https://arxiv.org/abs/2610.28402v1)**  
  Authors: StreamEval Team  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.28402v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://streameval.ai)  
  Keywords: benchmark, dit, evaluation, streaming, interactive, video generation, identity, avatar  
- **[LaLa-World: Scaling Latent World Models with Natural Language Actions](https://arxiv.org/abs/2610.27851v2)**  
  Authors: Junha Song, Geonmo Gu, Jeongeun Park, Heejeong Nam, Lucas Maes, Byeongho Heo, Dongyoon Han, Sangdoo Yun  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.27851v2.pdf)  
  Keywords: dit, simulation, video generation, efficient, world model, style  
- **[Manga2Animate: An Agentic Framework for Faithful Manga Animation with Script and Storyboard Planning](https://arxiv.org/abs/2610.26851v1)**  
  Authors: Sheng-Wei Zhang, Hsi-An Chen, Yan-Ting Liou, Chih-Hsuan Chen, Shih-Chen Tseng, Yu-Lun Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.26851v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://annchenn.github.io/Manga2Animate)  
  Keywords: style, video generation  
- **[TamedFlow: Trajectory-Aware Distillation for Teacher-Assisted Diffusion Sampling](https://arxiv.org/abs/2610.26025v2)**  
  Authors: Shuaiqi Cheng, Jiahao Zhang, Boyuan Gu, Yuxi Chen, Haiying Xu, Zexin Lu, Huiyu Zhou, Xuming Hu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.26025v2.pdf)  
  Keywords: diffusion transformer, dit, architecture, evaluation, video generation, identity, trajectory, distillation, acceleration  
- **[MAPS: A Multi-Agent Personalized Script-Driven Video Advertising System Enhanced by Reinforcement Learning](https://arxiv.org/abs/2610.25748v1)**  
  Authors: Zhongyu Wang, Chen Zuo, Qingxuan Sun, Jiayang Qiao, Qiuhao Qian, Songyan Cui, Guocheng Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.25748v1.pdf)  
  Keywords: personalization, advertising, video synthesis, creative  
- **[Clean Forcing: Drift-Resistant Autoregressive Video Diffusion with a Frozen Base](https://arxiv.org/abs/2610.25634v1)**  
  Authors: Wenqing Wang, Joonghyuk Shin, Jonathan Tremblay, Chan Hee Song, Yun Fu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.25634v1.pdf)  
  Keywords: video diffusion, autoregressive, dit, text-to-video, streaming, video generation, style, diffusion model  
- **[CorrFlow: Self-Correcting Flow Matching](https://arxiv.org/abs/2610.24750v1)**  
  Authors: Hangwei Zhang, Nathan Rouillé, Chuanxia Zheng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.24750v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://fogradio.github.io/corrflow-project) | [![Demo](https://img.shields.io/badge/-Demo-brightgreen)](https://fogradio.github.io/corrflow-project)  
  Keywords: dit, evaluation, physical, text-to-video, video generation, identity, image-to-video, flow matching  
- **[BodyBridge: Grounded Body Layers for Sim-to-Real Translation of Vulnerable Road Users](https://arxiv.org/abs/2610.24436v1)**  
  Authors: Mark Azer, Fabian B. Flohr  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.24436v1.pdf)  
  Keywords: video diffusion, dit, evaluation, simulation, identity, autonomous driving, diffusion model  

### Physical Understanding

*Showing the latest 50 out of 134 papers*

- **[WorldForge V2: Eliciting Camera-Trajectory Alignment in Video Diffusion Models](https://arxiv.org/abs/2610.31640v1)**  
  Authors: Chenxi Song, Yanming Yang, Tong Zhao, Ruibo Li, Joey Tianyi Zhou, Chi Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.31640v1.pdf)  
  Keywords: video diffusion, dit, denoising, evaluation, camera control, dynamics, video generation, trajectory, motion control, diffusion model  
- **[PhysTrace: Interpretable Temporal Evaluation of Physical Consistency in Video Generative Models](https://arxiv.org/abs/2610.31429v1)**  
  Authors: Taekoan Yoo, Wonkyung Jung, Kyunghun Kim, Kyeongbo Kong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.31429v1.pdf)  
  Keywords: physical, dit, dynamics, evaluation  
- **[DeXplicit: Making Physical State Explicit in Dexterous Manipulation World Models](https://arxiv.org/abs/2610.30781v1)**  
  Authors: Adam Lee, Mutian Xu, Yukang Cao, Shulin Tian, Ziwei Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.30781v1.pdf)  
  Keywords: dit, denoising, physical, dynamics, video generation, trajectory, video synthesis, efficient, world model, action-conditioned  
- **[PhyEvolve: Multi-Agent State-Evolution Planning for Physics-Aware Video Generation](https://arxiv.org/abs/2610.30717v1)**  
  Authors: Yang-Hao Zhou, Lixing Tan, Zhiqi Li, Guang Yang, Xiao Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.30717v1.pdf)  
  Keywords: benchmark, physical, text-to-video, video generation, physics, physics-aware  
- **[RealMe: Immersive Volumetric Video from Minimal Captures](https://arxiv.org/abs/2610.30023v1)**  
  Authors: Chenxu Zhou, Zhiyuan Yu, Yudong Jin, Yinji Shentu, Yu Zhang, Jiaming Sun, Xiaowei Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.30023v1.pdf)  
  Keywords: video diffusion, benchmark, layout, dynamics, diffusion model  
- **[Looking Ahead: Modeling Future Evolution in Autoregressive Video Generation](https://arxiv.org/abs/2610.29989v1)**  
  Authors: Ruopeng Gao, Yukun Huang, Jiarui Hu, Shuai Wang, Wenbo Hu, Ying Shan, Limin Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.29989v1.pdf)  
  Keywords: video diffusion, autoregressive, denoising, dit, physical, video generation, world model, diffusion model  
- **[CausalAlign: Causal Alignment of Video Generation Models for Consistent Ego-Motion](https://arxiv.org/abs/2610.29915v1)**  
  Authors: Kai Zhu, Yintianrun Zhang, Shuwei Jiang, Ruolin Zuo, Yixin Chen, Duomin Wang, Miao Liu, Yin Li, Daquan Zhou, Yiwu Zhong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.29915v1.pdf)  
  Keywords: benchmark, dynamics, denoising, video generation  
- **[Pair-Free Coarse-to-Real Video Generation via Real-to-Coarse Image Supervision](https://arxiv.org/abs/2610.28954v1)**  
  Authors: Gonzalo Gómez-Nogales, Daohan Lu, Peiye Zhuang, Tinghui Zhou, Yi Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.28954v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://gonzalognogales.github.io/coarse2real-sharp)  
  Keywords: dit, layout, simulation, dynamics, video generation  
- **[HorizonComposer: Spatiotemporally Consistent Driving Video Editing with Enriched Traffic Semantics](https://arxiv.org/abs/2610.28829v1)**  
  Authors: Mauricio Soroco, Yuqiu Liu, Zaid Tasneem, Francesco Pittaluga, Abhishek Aich, Wuyang Chen, Manmohan Chandraker, Ziyu Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.28829v1.pdf)  
  Keywords: dit, temporal consistency, dynamics, autonomous driving, video editing  
- **[AEON: Unifying Video and 3D World Models](https://arxiv.org/abs/2610.28631v1)**  
  Authors: Weiqi Zhang, Wenyuan Zhang, Yu-Shen Liu, Junsheng Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.28631v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://weiqi-zhang.github.io/AEON)  
  Keywords: benchmark, dit, simulation, dynamics, distillation, world model  

### Surveys & Benchmarks

*Showing the latest 50 out of 245 papers*

- **[WorldForge V2: Eliciting Camera-Trajectory Alignment in Video Diffusion Models](https://arxiv.org/abs/2610.31640v1)**  
  Authors: Chenxi Song, Yanming Yang, Tong Zhao, Ruibo Li, Joey Tianyi Zhou, Chi Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.31640v1.pdf)  
  Keywords: video diffusion, dit, denoising, evaluation, camera control, dynamics, video generation, trajectory, motion control, diffusion model  
- **[AnyGameRenderer: Entity-Consistent Generative Rendering Across Games and an Entity-Level Benchmark](https://arxiv.org/abs/2610.31466v1)**  
  Authors: Ruicong Liu, Liangyang Ouyang, Fengbo Lan, Zhixiang Wang, Kaipeng Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.31466v1.pdf)  
  Keywords: benchmark, dit, layout, video generation, video-to-video  
- **[PhysTrace: Interpretable Temporal Evaluation of Physical Consistency in Video Generative Models](https://arxiv.org/abs/2610.31429v1)**  
  Authors: Taekoan Yoo, Wonkyung Jung, Kyunghun Kim, Kyeongbo Kong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.31429v1.pdf)  
  Keywords: physical, dit, dynamics, evaluation  
- **[Verus-Insight: Towards Explainable Artifact Detection in AI-Generated Videos](https://arxiv.org/abs/2610.30866v1)**  
  Authors: Zhuoran Zhang, Yang Shi, Qixun Wang, Tengfei Liu, Yuqi Tang, Xuanyu Zhu, Yizhuo Jia, Jingyun Hua, Shixuan Liu, Xianghua Ying, Haotian Wang, Yuanxing Zhang, Pengfei Wan, Wenjing Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.30866v1.pdf)  
  Keywords: benchmark, video generation  
- **[Learning from Next-Frame Prediction: Towards Unified and Scalable Visual Representation Learning](https://arxiv.org/abs/2610.30724v1)**  
  Authors: Yifeng Yao, Jinghan Li, Zhihao Zhang, Yajiao Xiong, Yang Jin, Kun Xu, Huishuai Zhang, Dongyan Zhao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.30724v1.pdf)  
  Keywords: benchmark, world model, autoregressive, dit  
- **[PhyEvolve: Multi-Agent State-Evolution Planning for Physics-Aware Video Generation](https://arxiv.org/abs/2610.30717v1)**  
  Authors: Yang-Hao Zhou, Lixing Tan, Zhiqi Li, Guang Yang, Xiao Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.30717v1.pdf)  
  Keywords: benchmark, physical, text-to-video, video generation, physics, physics-aware  
- **[RealMe: Immersive Volumetric Video from Minimal Captures](https://arxiv.org/abs/2610.30023v1)**  
  Authors: Chenxu Zhou, Zhiyuan Yu, Yudong Jin, Yinji Shentu, Yu Zhang, Jiaming Sun, Xiaowei Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.30023v1.pdf)  
  Keywords: video diffusion, benchmark, layout, dynamics, diffusion model  
- **[CausalAlign: Causal Alignment of Video Generation Models for Consistent Ego-Motion](https://arxiv.org/abs/2610.29915v1)**  
  Authors: Kai Zhu, Yintianrun Zhang, Shuwei Jiang, Ruolin Zuo, Yixin Chen, Duomin Wang, Miao Liu, Yin Li, Daquan Zhou, Yiwu Zhong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.29915v1.pdf)  
  Keywords: benchmark, dynamics, denoising, video generation  
- **[MOSAIC: An Omni-Modal Benchmark for Long-Term Memory and Cross-Modal Reasoning in Conversational Agents](https://arxiv.org/abs/2610.29249v1)**  
  Authors: Hong Ting Tsang, Boyi Zhang, Haoyu Huang, Jiaxin Bai, Yufei Li, Yisen Gao, Zhongwei Xie, Hongyu Luo, Jeff Z. Pan, Yangqiu Song  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.29249v1.pdf)  
  Keywords: benchmark, evaluation  
- **[NeuralSRender: G-Buffer Guided Video Diffusion for Sim-to-Real Rendering](https://arxiv.org/abs/2610.29200v1)**  
  Authors: Yipeng Lu, Youqi Liao, Zhenyu Wang, Yuning Peng, Zhen Dong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.29200v1.pdf) | [![GitHub](https://img.shields.io/github/stars/WHU-USI3DV/NeuralSRender?style=social)](https://github.com/WHU-USI3DV/NeuralSRender)  
  Keywords: video diffusion, diffusion transformer, dit, evaluation, efficient, video translation  

### Text-to-Video Generation

*Showing the latest 50 out of 64 papers*

- **[Direct Forcing: A Single-Stage Training Recipe for Few-Step Autoregressive Text-to-Video Generation](https://arxiv.org/abs/2610.30861v1)**  
  Authors: Haojun Xu, Jie Huang, Xin Lu, Mingchen Zhong, Zihao Fan, Linjiang Huang, Si Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.30861v1.pdf)  
  Keywords: text-to-video, streaming, autoregressive, video generation  
- **[PhyEvolve: Multi-Agent State-Evolution Planning for Physics-Aware Video Generation](https://arxiv.org/abs/2610.30717v1)**  
  Authors: Yang-Hao Zhou, Lixing Tan, Zhiqi Li, Guang Yang, Xiao Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.30717v1.pdf)  
  Keywords: benchmark, physical, text-to-video, video generation, physics, physics-aware  
- **[Rethinking Video Autoencoders for Interactive World Models](https://arxiv.org/abs/2610.30129v1)**  
  Authors: Adrien Ramanana Rahary, Yutong Bai, Nicolas Dufour, Patrick Pérez, David Picard  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.30129v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://kyutai.org/blog/2026-10-21-cadre)  
  Keywords: world model, text-to-video, interactive  
- **[Latent Bridge: From Video Latents to 3D Geometry via Feature Alignment](https://arxiv.org/abs/2610.28521v1)**  
  Authors: Shuai Zhang, Zhanpeng Ouyang, Zhengqing Chen, Ruohong Mei, Shaoyu Chen, Weiqiang Ren, Hui Sun, Qian Zhang, Wenyu Liu, Xinggang Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.28521v1.pdf) | [![GitHub](https://img.shields.io/github/stars/hustvl/Latent-Bridge?style=social)](https://github.com/hustvl/Latent-Bridge)  
  Keywords: text-to-video, video generation, image-to-video, distillation, efficient  
- **[Code2Video-Compass: A Comprehensive Benchmark for General-Purpose Code-Based Video Generation across T2V, I2V, and V2V](https://arxiv.org/abs/2610.28416v1)**  
  Authors: Zhenghan Chen, Zekai Shao, Xin Lin, Leting Cheng, Siming Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.28416v1.pdf)  
  Keywords: benchmark, dit, creative, evaluation, text-to-video, video generation, t2v, i2v, image-to-video, controllable, video-to-video  
- **[Mise-en-Video: Fine-Grained 3D Control for Multi-Shot Video Generation](https://arxiv.org/abs/2610.26801v1)**  
  Authors: Yingshuang Zou, Xiaoyu Shi, Yawen Luo, Ziang Li, Qinghe Wang, Mengfei Li, Chengfeng Zhao, Xintao Wang, Pengfei Wan, Kun Gai, Yuan Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.26801v1.pdf)  
  Keywords: layout, evaluation, text-to-video, video generation, 3d-aware, controllable  
- **[PVBench: Quantifying Physical Plausibility in Video Generation with Object-Level Physical Measurements](https://arxiv.org/abs/2610.26711v1)**  
  Authors: Kaiwei Chen, Moran Li, Zhenye Gan, Yabiao Wang, Chengjie Wang, Kexin Zhang, Yong Liu, Jiangning Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.26711v1.pdf)  
  Keywords: benchmark, evaluation, physical, text-to-video, dynamics, video generation, image-to-video, world model  
- **[HORIA: 4D Human and Object Reconstruction from a Monocular Video with Interaction-Aware Re-Rendering](https://arxiv.org/abs/2610.25960v2)**  
  Authors: Hyeongjin Nam, Taeryung Lee, Daniel Sungho Jung, Kyoung Mu Lee  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.25960v2.pdf)  
  Keywords: video diffusion, text-to-video, dit, novel view  
- **[Clean Forcing: Drift-Resistant Autoregressive Video Diffusion with a Frozen Base](https://arxiv.org/abs/2610.25634v1)**  
  Authors: Wenqing Wang, Joonghyuk Shin, Jonathan Tremblay, Chan Hee Song, Yun Fu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.25634v1.pdf)  
  Keywords: video diffusion, autoregressive, dit, text-to-video, streaming, video generation, style, diffusion model  
- **[Meta Inverse Prompting for Video Generative Models](https://arxiv.org/abs/2610.24965v1)**  
  Authors: Yerin Jung, Jongheon Jeong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.24965v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://ueriniuno.github.io/mvip-page)  
  Keywords: dit, text-to-video, dynamics, image-to-video, controllable, efficient  

### Video Editing

- **[AnyGameRenderer: Entity-Consistent Generative Rendering Across Games and an Entity-Level Benchmark](https://arxiv.org/abs/2610.31466v1)**  
  Authors: Ruicong Liu, Liangyang Ouyang, Fengbo Lan, Zhixiang Wang, Kaipeng Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.31466v1.pdf)  
  Keywords: benchmark, dit, layout, video generation, video-to-video  
- **[NeuralSRender: G-Buffer Guided Video Diffusion for Sim-to-Real Rendering](https://arxiv.org/abs/2610.29200v1)**  
  Authors: Yipeng Lu, Youqi Liao, Zhenyu Wang, Yuning Peng, Zhen Dong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.29200v1.pdf) | [![GitHub](https://img.shields.io/github/stars/WHU-USI3DV/NeuralSRender?style=social)](https://github.com/WHU-USI3DV/NeuralSRender)  
  Keywords: video diffusion, diffusion transformer, dit, evaluation, efficient, video translation  
- **[HorizonComposer: Spatiotemporally Consistent Driving Video Editing with Enriched Traffic Semantics](https://arxiv.org/abs/2610.28829v1)**  
  Authors: Mauricio Soroco, Yuqiu Liu, Zaid Tasneem, Francesco Pittaluga, Abhishek Aich, Wuyang Chen, Manmohan Chandraker, Ziyu Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.28829v1.pdf)  
  Keywords: dit, temporal consistency, dynamics, autonomous driving, video editing  
- **[Code2Video-Compass: A Comprehensive Benchmark for General-Purpose Code-Based Video Generation across T2V, I2V, and V2V](https://arxiv.org/abs/2610.28416v1)**  
  Authors: Zhenghan Chen, Zekai Shao, Xin Lin, Leting Cheng, Siming Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.28416v1.pdf)  
  Keywords: benchmark, dit, creative, evaluation, text-to-video, video generation, t2v, i2v, image-to-video, controllable, video-to-video  
- **[VitronEdit: Universal Visual Editing across Images, Videos, and 3D Scenes](https://arxiv.org/abs/2610.27049v1)**  
  Authors: Jing Wang, Yanlin Li, Mong-Li Lee, Wynne Hsu, Shengqiong Wu, Hao Fei  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.27049v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://vitron-llm.github.io/VitronEdit)  
  Keywords: video editing, dit  
- **[GeoV2V: Geometry-Grounded Video Diffusion Model for Driving Scene Generation](https://arxiv.org/abs/2610.25245v1)**  
  Authors: Yuchen Xi, Yuhan Guo, Chenwei Hou, Zixu Liu, Jin Fang, Jason Liu, Ruigang Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.25245v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://xiyuche.github.io/GeoV2V)  
  Keywords: video diffusion, dit, simulation, dynamics, trajectory, autonomous driving, video-to-video, novel view, diffusion model  
- **[Learning to Correct Geometry in Generated Videos](https://arxiv.org/abs/2610.23856v1)**  
  Authors: Weijie Lyu, Tiancheng Shen, Jason Li, Yujing Wang, Xiaoyuan Wang, Haobo Yuan, Yizhou Zhao, Ming-Hsuan Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.23856v1.pdf)  
  Keywords: benchmark, dit, image-to-video, trajectory, video-to-video, video inpainting  
- **[OmniXRef: A Unified Framework for Multimodal Multi-Reference Video Editing](https://arxiv.org/abs/2610.22744v1)**  
  Authors: Xiaoyan Cong, Tianyu Wang, Hyeonho Jeong, Zhifei Zhang, Yuqian Zhou, Yijun Li, Shaoteng Liu, Zhe Lin, Srinath Sridhar, Soo Ye Kim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.22744v1.pdf)  
  Keywords: diffusion transformer, benchmark, dit, creative, evaluation, video editing, style  
- **[Where, How, and When: Query-Guided Grounding for Video Understanding](https://arxiv.org/abs/2610.21422v1)**  
  Authors: Yogesh Kumar  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.21422v1.pdf)  
  Keywords: text-to-video, temporal consistency, dit, video-to-video  
- **[QK-Edit: Revisiting Attention-based Injection in MM-DiT for Image and Video Editing](https://arxiv.org/abs/2610.17829v2)**  
  Authors: Tiancheng Shen, Zilong Huang, Xiangtai Li, Zhijie Lin, Jiyang Liu, Yitong Wang, Jiashi Feng, Ming-Hsuan Yang, Jun Hao Liew  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.17829v2.pdf)  
  Keywords: diffusion transformer, dit, architecture, dynamics, video editing, style  

### Video Inpainting & Completion

- **[Learning to Correct Geometry in Generated Videos](https://arxiv.org/abs/2610.23856v1)**  
  Authors: Weijie Lyu, Tiancheng Shen, Jason Li, Yujing Wang, Xiaoyuan Wang, Haobo Yuan, Yizhou Zhao, Ming-Hsuan Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.23856v1.pdf)  
  Keywords: benchmark, dit, image-to-video, trajectory, video-to-video, video inpainting  
- **[Perceive, Predict, and Plan: a Unified World Action Model for Egocentric Dexterous Manipulation](https://arxiv.org/abs/2610.22363v2)**  
  Authors: Zirui Wu, Chen Guo, Tianjian Jiang, Zeren Jiang, Zeming Li, Lingchen Yang, Longteng Duan, Ying Xue, Handi Yin, Shenyuan Gao, Martin R. Oswald, Jun Zhang, Ping Tan, Jie Song  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.22363v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://p3-wam.pages.dev)  
  Keywords: video diffusion, diffusion transformer, dit, architecture, evaluation, video prediction, action-conditioned  
- **[RAP-WAM: Learning World-Action Models through Predictive Rehearsal and Action Perturbations](https://arxiv.org/abs/2610.16443v2)**  
  Authors: Yuanpeng He, Ceyao Zhang, Fangjing Li, Kefei Zhu, Lijian Li, Yueheng Li, Tianjia He, Wenpin Jiao, Zhi Jin, Yaodong Yang, Yuanpei Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.16443v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://rapwam.github.io)  
  Keywords: video prediction, dit, simulation, video generation  
- **[SurgCast: Action-Conditioned Future Skeletons for Controllable Surgical World Models](https://arxiv.org/abs/2610.15645v1)**  
  Authors: Wanhao Liu, Rulin Zhou, Liangjing Shao, Zhaocheng Lin, Dongyue Li, Jinsong Lin, Guoheng Ma, Hangheng Yang, Zhiqing Tang, Jing Chen, Panshuo Li, Hongliang Ren  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.15645v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://surgcast.netlify.app/.) | [![Demo](https://img.shields.io/badge/-Demo-brightgreen)](https://surgcast.netlify.app)  
  Keywords: dit, video generation, video prediction, controllable, world model, action-conditioned  
- **[WorldWeave: Growing Persistent Geometric Worlds for Video Generation](https://arxiv.org/abs/2609.34221v2)**  
  Authors: Yifan Huang, Lifan Jiang, Qingyue Hao, Cheng Chen, Boxi Wu, Xiaoxue Ren, Xiaofei He, Dehai Zhao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.34221v2.pdf)  
  Keywords: dit, video generation, video synthesis, world model, outpainting  
- **[MT-WAM: Reorienting the One-Pass Predictive Representation Toward Action Generation](https://arxiv.org/abs/2609.21474v1)**  
  Authors: Yiguang Yang, Jiankun Peng, Xiaoming Wang, Yiran Zhang, Zhibo Fang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.21474v1.pdf)  
  Keywords: video diffusion, diffusion transformer, dit, dynamics, video prediction  
- **[StrucPhysVideo: Learning Physical Dynamics from Structured Captions and Robot Actions](https://arxiv.org/abs/2609.18430v1)**  
  Authors: Awomo-WM Team, :, Enhui Ma, Kaiwen Guo, Tingrui Zhang, Wei Song, Yingshui Tan, Jianhua Xu, Tong Zhang, Kaicheng Yu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.18430v1.pdf)  
  Keywords: autoregressive, denoising, dit, physical, dynamics, interactive, physics, i2v, image-to-video, video prediction, distillation, world model, action-conditioned  
- **[GeoLAM: Learning Geometry-Grounded Latent Actions from Unlabeled Human Videos](https://arxiv.org/abs/2609.17099v1)**  
  Authors: Yifan Xie, Hekun Tian, Jinkun Liu, YuAn Wang, Qiao Sun, Wenbo Ding  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.17099v1.pdf)  
  Keywords: benchmark, evaluation, video generation, video prediction, trajectory  

### Video Super-Resolution & Enhancement

*Showing the latest 50 out of 86 papers*

- **[WorldForge V2: Eliciting Camera-Trajectory Alignment in Video Diffusion Models](https://arxiv.org/abs/2610.31640v1)**  
  Authors: Chenxi Song, Yanming Yang, Tong Zhao, Ruibo Li, Joey Tianyi Zhou, Chi Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.31640v1.pdf)  
  Keywords: video diffusion, dit, denoising, evaluation, camera control, dynamics, video generation, trajectory, motion control, diffusion model  
- **[DeXplicit: Making Physical State Explicit in Dexterous Manipulation World Models](https://arxiv.org/abs/2610.30781v1)**  
  Authors: Adam Lee, Mutian Xu, Yukang Cao, Shulin Tian, Ziwei Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.30781v1.pdf)  
  Keywords: dit, denoising, physical, dynamics, video generation, trajectory, video synthesis, efficient, world model, action-conditioned  
- **[Self-Distilling Future Video Representations for World Action Models](https://arxiv.org/abs/2610.30320v1)**  
  Authors: Huiwon Jang, Suhyeok Jang, Hyeonmo Kang, Seungku Kim, Jinwoo Shin, Sihyun Yu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.30320v1.pdf)  
  Keywords: video diffusion, dit, denoising, video generation, distillation, diffusion model  
- **[Looking Ahead: Modeling Future Evolution in Autoregressive Video Generation](https://arxiv.org/abs/2610.29989v1)**  
  Authors: Ruopeng Gao, Yukun Huang, Jiarui Hu, Shuai Wang, Wenbo Hu, Ying Shan, Limin Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.29989v1.pdf)  
  Keywords: video diffusion, autoregressive, denoising, dit, physical, video generation, world model, diffusion model  
- **[CausalAlign: Causal Alignment of Video Generation Models for Consistent Ego-Motion](https://arxiv.org/abs/2610.29915v1)**  
  Authors: Kai Zhu, Yintianrun Zhang, Shuwei Jiang, Ruolin Zuo, Yixin Chen, Duomin Wang, Miao Liu, Yin Li, Daquan Zhou, Yiwu Zhong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.29915v1.pdf)  
  Keywords: benchmark, dynamics, denoising, video generation  
- **[Sparsity Should Be ALLOTted by Output: Training-Free Allocation of Block-Sparse Attention for Video Diffusion Transformers](https://arxiv.org/abs/2610.29441v1)**  
  Authors: Tianze Xia, Xiaoling Zhou, Ruya Lan, Yiqiao Liao, Chengru Song, Shiming Xiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.29441v1.pdf)  
  Keywords: video diffusion, diffusion transformer, dit, denoising, trajectory  
- **[OccJEPA: Occlusion as Masking for Amodal Video Segmentation](https://arxiv.org/abs/2610.29061v1)**  
  Authors: Genpei Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.29061v1.pdf) | [![GitHub](https://img.shields.io/github/stars/zgp110/occjepa?style=social)](https://github.com/zgp110/occjepa)  
  Keywords: video diffusion, world model, denoising, diffusion model  
- **[MoDDiT: Simple Token Routing in Diffusion Transformers](https://arxiv.org/abs/2610.28086v1)**  
  Authors: Jarek Liesen, Matthew T. Jackson, Benjamin Ellis, Shimon Whiteson, Jakob N. Foerster  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.28086v1.pdf)  
  Keywords: diffusion transformer, autoregressive, denoising, dit, architecture, interactive, video generation, world model  
- **[Recast the Past: Stable Long Video Generation with Full Context Memory](https://arxiv.org/abs/2610.27986v1)**  
  Authors: Yukuo Ma, Cong Liu, Junke Wang, Junqi Liu, Haibin Huang, Zuxuan Wu, Xuelong Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.27986v1.pdf)  
  Keywords: diffusion transformer, autoregressive, denoising, dit, long video, video generation  
- **[Decoupling Action from Egocentric Observation for World Simulation](https://arxiv.org/abs/2610.27946v1)**  
  Authors: Yue Ma, Pengjie Song, Xinyu Wang, Yi He, Zeqian Long, Fangneng Zhan, Kaichen Zhou, Hongyu Liu, Hongfa Wang, Peihao Li, Haoyang Huang, Nan Duan, Qifeng Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.27946v1.pdf)  
  Keywords: video diffusion, benchmark, dit, denoising, layout, physical, simulation, dynamics, video generation, diffusion model  

### World Models & Simulation

*Showing the latest 50 out of 126 papers*

- **[DeXplicit: Making Physical State Explicit in Dexterous Manipulation World Models](https://arxiv.org/abs/2610.30781v1)**  
  Authors: Adam Lee, Mutian Xu, Yukang Cao, Shulin Tian, Ziwei Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.30781v1.pdf)  
  Keywords: dit, denoising, physical, dynamics, video generation, trajectory, video synthesis, efficient, world model, action-conditioned  
- **[Learning from Next-Frame Prediction: Towards Unified and Scalable Visual Representation Learning](https://arxiv.org/abs/2610.30724v1)**  
  Authors: Yifeng Yao, Jinghan Li, Zhihao Zhang, Yajiao Xiong, Yang Jin, Kun Xu, Huishuai Zhang, Dongyan Zhao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.30724v1.pdf)  
  Keywords: benchmark, world model, autoregressive, dit  
- **[Rethinking Video Autoencoders for Interactive World Models](https://arxiv.org/abs/2610.30129v1)**  
  Authors: Adrien Ramanana Rahary, Yutong Bai, Nicolas Dufour, Patrick Pérez, David Picard  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.30129v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://kyutai.org/blog/2026-10-21-cadre)  
  Keywords: world model, text-to-video, interactive  
- **[Looking Ahead: Modeling Future Evolution in Autoregressive Video Generation](https://arxiv.org/abs/2610.29989v1)**  
  Authors: Ruopeng Gao, Yukun Huang, Jiarui Hu, Shuai Wang, Wenbo Hu, Ying Shan, Limin Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.29989v1.pdf)  
  Keywords: video diffusion, autoregressive, denoising, dit, physical, video generation, world model, diffusion model  
- **[How Representational Priors Shape Generalization in World Action Models](https://arxiv.org/abs/2610.29168v1)**  
  Authors: Junha Chun, Youngjoon Jeong, Taesup Kim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.29168v1.pdf)  
  Keywords: world model, dit  
- **[OccJEPA: Occlusion as Masking for Amodal Video Segmentation](https://arxiv.org/abs/2610.29061v1)**  
  Authors: Genpei Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.29061v1.pdf) | [![GitHub](https://img.shields.io/github/stars/zgp110/occjepa?style=social)](https://github.com/zgp110/occjepa)  
  Keywords: video diffusion, world model, denoising, diffusion model  
- **[Pair-Free Coarse-to-Real Video Generation via Real-to-Coarse Image Supervision](https://arxiv.org/abs/2610.28954v1)**  
  Authors: Gonzalo Gómez-Nogales, Daohan Lu, Peiye Zhuang, Tinghui Zhou, Yi Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.28954v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://gonzalognogales.github.io/coarse2real-sharp)  
  Keywords: dit, layout, simulation, dynamics, video generation  
- **[AEON: Unifying Video and 3D World Models](https://arxiv.org/abs/2610.28631v1)**  
  Authors: Weiqi Zhang, Wenyuan Zhang, Yu-Shen Liu, Junsheng Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.28631v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://weiqi-zhang.github.io/AEON)  
  Keywords: benchmark, dit, simulation, dynamics, distillation, world model  
- **[Learning the 4D World through Point Trajectory Forecasting](https://arxiv.org/abs/2610.28594v1)**  
  Authors: Byungwoo Jeon, Sunghwan Hong, Dohyeon Kim, Jonghoon Lee, Jungwoo Park, Inhee Lee, Doosan Baek, Jinil Kim, Taehyun Lim, Hanbyul Joo, Marc Pollefeys, Saining Xie, Jinwoo Shin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.28594v1.pdf)  
  Keywords: benchmark, 4d generation, dit, evaluation, physical, simulation, video generation, 3d-aware, trajectory, multi-view video, world model  
- **[StreamEval: Evaluating Interactive Streaming Video Generation Models](https://arxiv.org/abs/2610.28402v1)**  
  Authors: StreamEval Team  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.28402v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://streameval.ai)  
  Keywords: benchmark, dit, evaluation, streaming, interactive, video generation, identity, avatar  



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
