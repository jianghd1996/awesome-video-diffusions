# Awesome Video Diffusions [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of latest research papers, projects and resources related to Video Diffusion Models and Video Generation. Content is automatically updated daily.

> Last Update: 2026-09-14 03:26:44

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

- [3D-aware Video Generation](#3d-aware-video-generation) (16 papers) - Video generation with 3D awareness, multi-view consistency, and 4D content creation
- [Applications](#applications) (42 papers) - Domain-specific applications of video diffusion models
- [Architecture & Efficiency](#architecture-&-efficiency) (346 papers) - Architectural innovations (DiT, UNet), flow matching, and training/inference efficiency
- [Audio & Multi-modal](#audio-&-multi-modal) (21 papers) - Audio-driven and multi-modal conditioned video generation
- [Controllable Generation](#controllable-generation) (124 papers) - Controllable video generation with motion, camera, pose, or layout guidance
- [Human & Character Animation](#human-&-character-animation) (23 papers) - Human-centric video generation including talking heads, dance, and character animation
- [Image-to-Video Generation](#image-to-video-generation) (43 papers) - Methods for animating still images into videos
- [Long Video Generation](#long-video-generation) (127 papers) - Generating temporally consistent long-form videos beyond short clips
- [Personalization & Customization](#personalization-&-customization) (83 papers) - Personalized video generation with custom subjects, identities, or styles
- [Physical Understanding](#physical-understanding) (139 papers) - Physics-aware video generation and dynamics modeling
- [Surveys & Benchmarks](#surveys-&-benchmarks) (230 papers) - Survey papers, benchmarks, and evaluation metrics for video generation
- [Text-to-Video Generation](#text-to-video-generation) (70 papers) - Foundation models and methods for generating videos from text prompts
- [Video Editing](#video-editing) (18 papers) - Diffusion-based video editing, style transfer, and manipulation
- [Video Inpainting & Completion](#video-inpainting-&-completion) (10 papers) - Video inpainting, completion, outpainting, and temporal prediction
- [Video Super-Resolution & Enhancement](#video-super-resolution-&-enhancement) (81 papers) - Video quality improvement, upscaling, restoration, and frame interpolation
- [World Models & Simulation](#world-models-&-simulation) (109 papers) - Video generation as world simulators and interactive environment generation



## Table of Contents

- [Categorized Papers](#categorized-papers)
- [Classic Papers](#classic-papers)
- [Open Source Projects](#open-source-projects)
- [Applications](#applications)
- [Tutorials & Blogs](#tutorials--blogs)





## Categorized Papers

### 3D-aware Video Generation

- **[Rethinking 3D Noise: Learning 3D-Aware Video Priors via Optimization-Free Morphological Perturbations](https://arxiv.org/abs/2609.03657v1)**  
  Authors: Onat Şahin, Mohammad Altillawi, George Eskandar, Carlos Carbone, Ziyuan Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.03657v1.pdf)  
  Keywords: robotics, 3d-aware, video diffusion  
- **[Stabilizing Camera-Controlled Novel View Synthesis at Inference Time](https://arxiv.org/abs/2609.03639v1)**  
  Authors: Prajwal Singh, Arjun Badola, Seema Kumari, Hajime Nagahara, Shanmuganathan Raman  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.03639v1.pdf)  
  Keywords: efficient, video diffusion, novel view, diffusion model, autoregressive  
- **[Building Pretraining Data for World Models: An Unreal Engine-Based Pipeline for Action-Conditioned Video Generation](https://arxiv.org/abs/2609.03557v1)**  
  Authors: Haoyu Wang, Songchun Zhang, Haoran Li, Haoyang Huang, Zeyue Xue, Nan Duan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.03557v1.pdf)  
  Keywords: world model, video generation, physics, dit, architecture, multi-view video, trajectory, action-conditioned  
- **[RoGe: Novel View Synthesis via End-to-End Implicit Reconstruction and Generation](https://arxiv.org/abs/2609.02847v2)**  
  Authors: Xiaolei Lang, Ze Kang, Zehao Huang, Naiyan Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.02847v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://jerry-locker.github.io/roge)  
  Keywords: temporal consistency, dit, video diffusion, novel view, trajectory, diffusion model  
- **[Spatially Aware World Action Model via Geometric Latent Diffusion](https://arxiv.org/abs/2609.02531v1)**  
  Authors: Javier Alejandro Lopetegui Gonzalez, Paul Pacaud, Cordelia Schmid  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.02531v1.pdf)  
  Keywords: evaluation, world model, benchmark, 3d-aware, video diffusion, diffusion model, physical  
- **[Streaming4D: Accelerate 4D World Models via Block-wise Video Generation and Incremental Reconstruction](https://arxiv.org/abs/2609.00610v2)**  
  Authors: Xiaoyan Liu, Jiaxin Liu, Kangrui Li, Sifan Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.00610v2.pdf)  
  Keywords: 4d generation, streaming, world model, video generation, style, dit, interactive, autoregressive  
- **[GaussVid: Sparse-View Gaussian Splatting with 3D-Aware Video Diffusion Priors](https://arxiv.org/abs/2608.21849v1)**  
  Authors: Xinhui Liu, Can Wang, Wei Jiang, Wei Wang, Dong Xu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.21849v1.pdf)  
  Keywords: video generation, 3d-aware, video restoration, video diffusion, dit, novel view, diffusion model  
- **[Grounded-Exo2Ego: Structured Semantic Grounding for Robust Exocentric-to-Egocentric Video Generation](https://arxiv.org/abs/2608.20534v1)**  
  Authors: Shengze Wang, Michael Stengel, Tianye Li, Seonwook Park, Amrita Mazumdar, Koki Nagano, Alex Trevithick, Shalini De Mello  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.20534v1.pdf)  
  Keywords: evaluation, video generation, dit, video diffusion, novel view, diffusion model, physical  
- **[Beyond Pixels: From Video Priors to 4D Worlds](https://arxiv.org/abs/2608.10744v1)**  
  Authors: Zihao Liu, Xiaolong Shen, Zhenglin Zhou, Ruijie Quan, Yi Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.10744v1.pdf)  
  Keywords: 4d generation, diffusion transformer, video diffusion, dit  
- **[UniWorld-View: Large-Baseline View Synthesis via Video Diffusion Models](https://arxiv.org/abs/2608.04701v1)**  
  Authors: Haiyang Zhou, Wangbo Yu, Chaoran Feng, Xunyu Zhou, Yonghong Tian, Li Yuan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.04701v1.pdf)  
  Keywords: controllable, benchmark, camera control, video diffusion, multi-view video, novel view, diffusion model  

### Applications

- **[CamPilot: A Multi-Agent Cinematic Assistant for Camera-Controlled Movie Generation](https://arxiv.org/abs/2609.10943v1)**  
  Authors: Yang Wu, Stefano Petrangeli, Ishita Dasgupta, Yu Shen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.10943v1.pdf)  
  Keywords: controllable, text-to-video, benchmark, film, video generation  
- **[Geodesic-informed Generative Diffusion Model For Topology-preserved Image Video Generation](https://arxiv.org/abs/2609.08153v1)**  
  Authors: Nian Wu, Nivetha Jayakumar, Jiarui Xing, Miaomiao Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.08153v1.pdf) | [![GitHub](https://img.shields.io/github/stars/nellie689/IGG?style=social)](https://github.com/nellie689/IGG)  
  Keywords: robotics, video generation, dynamics, diffusion model, physical  
- **[VI-Bench: Benchmarking Prompt Inversion from AIGC Videos](https://arxiv.org/abs/2609.08079v1)**  
  Authors: Wulin Xie, Rui Zhao, Kecen Li, Xiujin Liu, Bokang Zhang, Zheng Liu, Xinwen Hou, Chen Gong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.08079v1.pdf)  
  Keywords: benchmark, video generation, style, dit, creative  
- **[Better Call CineCrew: Consistent Ultra-Long Narrative-to-Film Generation](https://arxiv.org/abs/2609.07720v1)**  
  Authors: Jiaben Chen, Sixun Dong, Qinhong Zhou, Raine Ma, Zhiyang Dou, Wojciech Matusik, Chuang Gan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.07720v1.pdf)  
  Keywords: film, video generation, style, identity, long-form  
- **[PAI-Actor: Cinematic Multi-Character Replacement in Dynamic Scenes](https://arxiv.org/abs/2609.05918v1)**  
  Authors: Bangxun Tang, Heyuan Gao, Yiren Song, Guian Fang, Zijian He, Jie Yang, Mike Zheng Shou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.05918v1.pdf)  
  Keywords: efficient, video generation, film, video-to-video, dynamics, distillation, diffusion transformer, autoregressive, long-form  
- **[Rethinking 3D Noise: Learning 3D-Aware Video Priors via Optimization-Free Morphological Perturbations](https://arxiv.org/abs/2609.03657v1)**  
  Authors: Onat Şahin, Mohammad Altillawi, George Eskandar, Carlos Carbone, Ziyuan Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.03657v1.pdf)  
  Keywords: robotics, 3d-aware, video diffusion  
- **[AgenticGen: Reward-Guided Agentic Video Generation for Advertising](https://arxiv.org/abs/2609.09187v1)**  
  Authors: Xingyuan Bu, Chengru Song, Hao Zhou, Tao Zhou, Dong Li, Wei Li, Shilong Li, Hao Shi, Yongxin Guo, Donghao Zhou, Qiangpeng Yang, Shilei Wen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.09187v1.pdf)  
  Keywords: video synthesis, video generation, dit, advertising  
- **[Matrix-Game 3.5: Enhancing Real-Time Streaming Interactive World Models with Patch Memory](https://arxiv.org/abs/2608.29910v1)**  
  Authors: Runjia Qian, Zile Wang, Jihai Zhang, Kai Zou, Wei Yu, Jiaxing Li, Zexiang Liu, Yaokun Li, Fei Kang, Kaichen Huang, Mengyin An, Haobo Zhang, Biao Jiang, Jiahua Wang, Haofeng Sun, Yang Liu, Yangguang Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.29910v1.pdf)  
  Keywords: robotics, streaming, world model, flow matching, video generation, camera control, dit, distillation, diffusion model, simulation, interactive, identity, autoregressive  
- **[FRAMEWORKERS: A Dynamic Multi-Agent Framework for AI-Generated Video Production](https://arxiv.org/abs/2608.29814v1)**  
  Authors: Zhendong Li, Lei Sun, Letian Shi, Deheng Zhang, Ruibo Ming, Mengshun Hu, Dannong Xu, Jian Wang, Danda Paudel, Luc Van Gool, Jinjin Gu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.29814v1.pdf)  
  Keywords: dit, creative  
- **[AcrossVAM1.0: Particle World Modeling for Text-Assisted Robot Video Prediction](https://arxiv.org/abs/2608.28491v1)**  
  Authors: Yafei Zhang, Nan Wu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.28491v1.pdf)  
  Keywords: world model, benchmark, film, dynamics, trajectory, video prediction  

### Architecture & Efficiency

*Showing the latest 50 out of 346 papers*

- **[MindTopo: Can Foundation Models Reason in Topological Space?](https://arxiv.org/abs/2609.11900v1)**  
  Authors: Yunfei Ge, Anbang Liu, Qineng Wang, Johnalbert Garnica, Jianwen Lyu, Zihan Wang, Reuben Tan, Jianfeng Gao, Ruohan Zhang, Yining Hong, Jiajun Wu, Manling Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.11900v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://mind-topo.github.io)  
  Keywords: evaluation, controllable, benchmark, video generation, dit, dynamics  
- **[Caption-once, Frames-on-Demand: Visual-Need Routing for Budget-Aware Agentic Long Video Understanding](https://arxiv.org/abs/2609.11899v1)**  
  Authors: Weitong Cai, Hang Zhang, Yukai Huang, Yiqiao Xie, Shan Gao, Jiankang Deng, Songcen Xu, Jifei Song, Zhensong Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.11899v1.pdf)  
  Keywords: dit, long video, benchmark  
- **[Vidu S2: Real-Time Interactive, Editable, and Spatial Video Generation](https://arxiv.org/abs/2609.11638v1)**  
  Authors: Jintao Zhang, Kai Jiang, Jintao Chen, Xu Wang, Deyuan Liu, Jungang Li, Dechuang Chen, Ming Lin, Jingjiang Zhou, Haopeng Jin, Qi Jia, Xiaohang Wang, Yaole Wang, Zhanqiang Zhang, Ran Li, Zhengkun Huang, Shuyue Xiong, Yuji Wang, Zikun Dai, Hui He, Yang Luo, Mang Ning, Weiqi Feng, Chengyang Ye, Xinyue Lin, Min Zhao, Hongzhou Zhu, Hengkai Tan, Zeyuan Wang, Chendong Xiang, Kaiwen Zheng, Zhijie Deng, Fan Bao, Jianfei Chen, Jun Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.11638v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://vidu.com/vidu-stream)  
  Keywords: video editing, video generation, avatar, style, dit, interactive  
- **[Harnessing Intrinsic Subject-Aware Attention for Controllable Multi-Subject Video Generation](https://arxiv.org/abs/2609.11507v1)**  
  Authors: Niange Yu, Ye Tian, Biaolong Chen, Miao Lu, Aixi Zhang, Hao Jiang, Yunhai Tong, Pipei Huang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.11507v1.pdf)  
  Keywords: controllable, benchmark, video generation, dit, diffusion transformer, identity  
- **[Uncertainty DMD: Restoring Diversity in Few-Step Autoregressive Video Distillation](https://arxiv.org/abs/2609.11265v1)**  
  Authors: Zixuan Duan, Xunzhi Xiang, Yabo Chen, Xin Zhang, Changhan Liu, Haibin Huang, Chi Zhang, Qi Fan, Xuelong Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.11265v1.pdf)  
  Keywords: video generation, dit, dynamics, distillation, autoregressive  
- **[OmniHallu: Unified Hallucination Detection for Cross-Modal Comprehension and Generation in Multimodal Large Language Models](https://arxiv.org/abs/2609.11244v1)**  
  Authors: Jianjiang Yang, Peihang Li, Shanqing Xu, Mengchen Qian, Lu Zhang, Meng Luo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.11244v1.pdf)  
  Keywords: architecture, t2v, text-to-video, benchmark  
- **[Decoupled Self-Forcing Distillation for Streaming Talking Head Generation](https://arxiv.org/abs/2609.10317v1)**  
  Authors: Yanru An, Ruiyan Wang, Wenwu Wei, Rui Bu, Qi Wang, Hongwei Hu, Zhengxue Cheng, Rong Xie, Li Song, Wenjun Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.10317v1.pdf)  
  Keywords: streaming, dit, video diffusion, distillation, diffusion model, identity, autoregressive, talking head  
- **[Mask Forcing: Improving Autoregressive Video Diffusion Distillation via Dual-Noise Masking Rollout](https://arxiv.org/abs/2609.09123v1)**  
  Authors: Zhuoran Zhao, Shengju Qian, Tongtong Liang, Xianghao Kong, Songchun Zhang, Junchao Huang, Guian Fang, Xin Wang, Pan Hui, Anyi Rao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.09123v1.pdf)  
  Keywords: efficient, video generation, denoising, dit, video diffusion, distillation, diffusion model, autoregressive  
- **[DSE-VTG: Dual-Side Enhancement for Training-Free Video Temporal Grounding](https://arxiv.org/abs/2609.08850v1)**  
  Authors: Zhuo Cao, Bingqing Zhang, Sen Wang, Xue Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.08850v1.pdf)  
  Keywords: dit, dynamics, benchmark  
- **[SignRefine: Adapting Foundational Video Models for Sign Language Generation](https://arxiv.org/abs/2609.08496v1)**  
  Authors: Anton Pelykh, Edward Fish, Ozge Mercanoglu Sincan, Richard Bowden  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.08496v1.pdf)  
  Keywords: video generation, dit, video diffusion, diffusion model, diffusion transformer  

### Audio & Multi-modal

- **[AV-SafetyBench: A Safety Benchmark for Text-to-Audio-Video Generation](https://arxiv.org/abs/2609.06991v1)**  
  Authors: Suah Choi, Tae-Young Lee, Gyeong-Moon Park  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.06991v1.pdf)  
  Keywords: evaluation, video generation, sound, benchmark  
- **[MVWeaver: A Hierarchical Music Video Generation Agent with a Learned Song-to-Visual Bridge](https://arxiv.org/abs/2609.06478v1)**  
  Authors: Sifei Li, Minyan Luo, Xu Li, Guodong Qi, Xincan Wang, Hanwen Wang, Chen Zhang, Pengfei Wan, Oliver Deussen, Weiming Dong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.06478v1.pdf)  
  Keywords: video generation, dit, architecture, music video, concept, long-form  
- **[PRISM-Bench: An Audio-Centric Diagnostic Benchmark for Text-to-Audio-Video Generation](https://arxiv.org/abs/2609.04867v2)**  
  Authors: Yuchen Sun, Qian Yang, Jun Wang, Detai Xin, Guoqiao Yu, Guanglu Wan, Qi Jia  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.04867v2.pdf)  
  Keywords: evaluation, video generation, sound, benchmark  
- **[The Attention Triangle in Audio-Video Models](https://arxiv.org/abs/2609.03586v1)**  
  Authors: Sagi Polaczek, Noa Kraicer, Gal Metzer, Zhuo Ning, Ali Mahdavi-Amiri, Daniel Cohen-Or, Raja Giryes  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.03586v1.pdf)  
  Keywords: video generation, sound, dit, video diffusion, dynamics, diffusion model  
- **[Encore: Infinite Audio-Video Generation with Adaptive Signal Routing](https://arxiv.org/abs/2609.04249v1)**  
  Authors: Shaohua Pan, Junbao Chen, Shengyi He, Jingfeng Xue, Wen Tao, Haocheng Feng, Siming Fan, Dongwei Pan, Yi Yang, Wei He, Hang Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.04249v1.pdf) | [![GitHub](https://img.shields.io/github/stars/shaohua-pan/Encore?style=social)](https://github.com/shaohua-pan/Encore)  
  Keywords: evaluation, video generation, denoising, dit, audio-to-video, long-form  
- **[Surgical Video Generation From Diffusion to World Models: A Survey](https://arxiv.org/abs/2608.26214v1)**  
  Authors: Fuxiang Huang, Chenxu Zhang, Liang Han, Lei Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.26214v1.pdf)  
  Keywords: world model, video generation, multi-modal, dit, dynamics, simulation, concept, physical, survey  
- **[WeMM-Embedding: WeChat Multi-Modal Embedding Technical Report](https://arxiv.org/abs/2608.24053v1)**  
  Authors: Junjie Zhou, Ke Mei, Lei Li, Tianyi Wang, Fengyun Rao, Jing Lyu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.24053v1.pdf) | [![GitHub](https://img.shields.io/github/stars/Tencent/WeMM-Embedding?style=social)](https://github.com/Tencent/WeMM-Embedding)  
  Keywords: evaluation, multi-modal, benchmark  
- **[SingDance: Compositional Zero-Shot Singing-and-Dancing Video Generation with Role-Aware Audio Conditioning](https://arxiv.org/abs/2608.16220v1)**  
  Authors: Tao Feng, Xu Li, Xiangyang Luo, Ming Wen, Huadai Liu, Chen Zhang, Wei Xue  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.16220v1.pdf)  
  Keywords: controllable, body motion, video generation, speech-driven, dit, video diffusion  
- **[AnyTalk: Speech Animation for Arbitrary Characters Leveraging a Video Generation Model](https://arxiv.org/abs/2608.16143v1)**  
  Authors: Kwan Yun, Serin Yoon, Sunjin Jung, Jung Eun Yoo, Inyup Lee, Junyong Noh  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.16143v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://serin-yoon.github.io/projects/anytalk)  
  Keywords: video generation, video diffusion, audio-driven, diffusion model  
- **[Adding Voice Cloning to Text-to-Audio-Video Models with a Single Zero-Initialised Layer](https://arxiv.org/abs/2608.15690v1)**  
  Authors: Ivan Mikheev, Viacheslav Vasilev, Anna Dmitrienko, Alexey Letunovskiy, Ivan Kirillov, Kirill Chernyshev, Denis Dimitrov  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.15690v1.pdf)  
  Keywords: benchmark, sound, dit, architecture, video diffusion  

### Controllable Generation

*Showing the latest 50 out of 124 papers*

- **[MindTopo: Can Foundation Models Reason in Topological Space?](https://arxiv.org/abs/2609.11900v1)**  
  Authors: Yunfei Ge, Anbang Liu, Qineng Wang, Johnalbert Garnica, Jianwen Lyu, Zihan Wang, Reuben Tan, Jianfeng Gao, Ruohan Zhang, Yining Hong, Jiajun Wu, Manling Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.11900v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://mind-topo.github.io)  
  Keywords: evaluation, controllable, benchmark, video generation, dit, dynamics  
- **[Harnessing Intrinsic Subject-Aware Attention for Controllable Multi-Subject Video Generation](https://arxiv.org/abs/2609.11507v1)**  
  Authors: Niange Yu, Ye Tian, Biaolong Chen, Miao Lu, Aixi Zhang, Hao Jiang, Yunhai Tong, Pipei Huang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.11507v1.pdf)  
  Keywords: controllable, benchmark, video generation, dit, diffusion transformer, identity  
- **[CamPilot: A Multi-Agent Cinematic Assistant for Camera-Controlled Movie Generation](https://arxiv.org/abs/2609.10943v1)**  
  Authors: Yang Wu, Stefano Petrangeli, Ishita Dasgupta, Yu Shen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.10943v1.pdf)  
  Keywords: controllable, text-to-video, benchmark, film, video generation  
- **[VANTAGE-Bench: Evaluating the Infrastructure AI Gap in Vision-Language Models](https://arxiv.org/abs/2609.09396v1)**  
  Authors: Zaid Pervaiz Bhat, Nimra Nayyar, Arihant Jain, Lap Fung Chan, John Suchanek, Yu Wang, Varun Praveen, Tomasz Kornuta, Vidya Nariyambut Murali  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.09396v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://vantage-bench.org)  
  Keywords: evaluation, physical, trajectory, benchmark  
- **[Temporal State Transport in Video Generation: Diagnosing and Correcting Spectral Imbalance](https://arxiv.org/abs/2609.08505v1)**  
  Authors: Luyao Tang, Bingjun Luo, Dong Yi, Jialin Guo, Haoning Xi, Cheng Chen, Yizhou Yu, Chaoqi Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.08505v1.pdf) | [![GitHub](https://img.shields.io/github/stars/lytang63/temporal-state-transport?style=social)](https://github.com/lytang63/temporal-state-transport)  
  Keywords: temporal consistency, video generation, layout, identity  
- **[PhysFlow: Physics-Aware Optical Flow for Motion Controllable Video Generation](https://arxiv.org/abs/2609.08215v1)**  
  Authors: Cong Wang, Hanxin Zhu, Yonglin Tian, Jiayi Luo, Ruiqi Song, Boyi Sun, Long Chen, Zhibo Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.08215v1.pdf)  
  Keywords: controllable, video generation, physics, motion control, dit, dynamics, physics-aware, physical  
- **[The Price of Consistency: Exploiting Visual Anchors for Multimodal Jailbreaking in Video Generation](https://arxiv.org/abs/2609.07216v1)**  
  Authors: Peng Li, Qianqian Xu, Yangbangyan Jiang, Zhipeng Yu, Qingming Huang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.07216v1.pdf)  
  Keywords: controllable, temporal consistency, benchmark, video generation, i2v, dit  
- **[PRG-Fusion: Orchestrating Generative Priors with Reconstruction Evidence for Driving View Synthesis](https://arxiv.org/abs/2609.06948v1)**  
  Authors: Sipeng He, Jialei Chen, Zhen Fang, Dongchun Ren, Feng Zhao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.06948v1.pdf)  
  Keywords: video synthesis, simulation, trajectory  
- **[Multi-Grid Post-Training for Long-Form Multi-Shot Video Generation](https://arxiv.org/abs/2609.06373v1)**  
  Authors: Jiawei Mao, Haoqin Tu, Hardy Chen, Yuhan Wang, Keyang Xu, Jieru Mei, Hongliang Fei, Ruogu Fang, Wei Shao, Cihang Xie, Yuyin Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.06373v1.pdf)  
  Keywords: benchmark, video generation, layout, denoising, long video, long-form  
- **[TourPhysics: Bringing Physics to World Models for Exploration and Manipulation from a Single Image](https://arxiv.org/abs/2609.04911v2)**  
  Authors: Xin Zhang, Yabo Chen, Zixuan Duan, Haibin Huang, Chi Zhang, Feng Xu, Xuelong Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.04911v2.pdf)  
  Keywords: world model, video synthesis, video generation, physical, physics, dit, trajectory, simulation, interactive  

### Human & Character Animation

- **[Vidu S2: Real-Time Interactive, Editable, and Spatial Video Generation](https://arxiv.org/abs/2609.11638v1)**  
  Authors: Jintao Zhang, Kai Jiang, Jintao Chen, Xu Wang, Deyuan Liu, Jungang Li, Dechuang Chen, Ming Lin, Jingjiang Zhou, Haopeng Jin, Qi Jia, Xiaohang Wang, Yaole Wang, Zhanqiang Zhang, Ran Li, Zhengkun Huang, Shuyue Xiong, Yuji Wang, Zikun Dai, Hui He, Yang Luo, Mang Ning, Weiqi Feng, Chengyang Ye, Xinyue Lin, Min Zhao, Hongzhou Zhu, Hengkai Tan, Zeyuan Wang, Chendong Xiang, Kaiwen Zheng, Zhijie Deng, Fan Bao, Jianfei Chen, Jun Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.11638v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://vidu.com/vidu-stream)  
  Keywords: video editing, video generation, avatar, style, dit, interactive  
- **[Decoupled Self-Forcing Distillation for Streaming Talking Head Generation](https://arxiv.org/abs/2609.10317v1)**  
  Authors: Yanru An, Ruiyan Wang, Wenwu Wei, Rui Bu, Qi Wang, Hongwei Hu, Zhengxue Cheng, Rong Xie, Li Song, Wenjun Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.10317v1.pdf)  
  Keywords: streaming, dit, video diffusion, distillation, diffusion model, identity, autoregressive, talking head  
- **[BooM-VVT: Boosting Mask-Free Video Virtual Try-On with Image-Level Pseudo Data](https://arxiv.org/abs/2609.04120v1)**  
  Authors: Wei Zhang, Xin Li, Peishu Shi, Jialin Gao, Xuekang Peng, Zhichao Lian, Yeying Jin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.04120v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://boomvvt.github.io/boomvvt)  
  Keywords: virtual try-on, video generation, temporal consistency  
- **[AvatarDynamizer: From Static to Dynamic Human Avatars via Generative Dynamic Textures](https://arxiv.org/abs/2608.19900v1)**  
  Authors: Guoxing Sun, Heming Zhu, Linjie Lyu, Pascal Fua, Christian Theobalt, Marc Habermann  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.19900v1.pdf)  
  Keywords: controllable, avatar, dit, video diffusion, dynamics, diffusion model  
- **[CL4D: Contrastive Language-4D Pretraining for Vision-Language Reasoning in Dynamic Scenes](https://arxiv.org/abs/2608.18734v2)**  
  Authors: Kumal Hewagamage, Isuranga Senavirathne, Sasika Amarasinghe, Hasitha Gallella, Dulanga Weerakoon, Vigneshwaran Subbaraju, Ranga Rodrigo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.18734v2.pdf)  
  Keywords: benchmark, dit, dynamics, human motion, physical  
- **[SingDance: Compositional Zero-Shot Singing-and-Dancing Video Generation with Role-Aware Audio Conditioning](https://arxiv.org/abs/2608.16220v1)**  
  Authors: Tao Feng, Xu Li, Xiangyang Luo, Ming Wen, Huadai Liu, Chen Zhang, Wei Xue  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.16220v1.pdf)  
  Keywords: controllable, body motion, video generation, speech-driven, dit, video diffusion  
- **[FlowDance: Music-Driven Dance Video Generation with Parallel Pose and RGB Streams](https://arxiv.org/abs/2608.15818v1)**  
  Authors: Genying Li, Boda Lin, Jiachen Li, Zijian Jia, Haojie Zheng, Yiming Wang, Shuchen Weng, Si Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.15818v1.pdf)  
  Keywords: video synthesis, body motion, video generation, denoising, long video, identity, human animation  
- **[Avatar-Forever: Decoupled Parallel Training for High-Quality Real-Time Infinite Avatars](https://arxiv.org/abs/2608.12107v1)**  
  Authors: Ruibin Li, Tao Yang, Zhiyuan Ma, Fangzhou Ai, Shilei Wen, Lei Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.12107v1.pdf)  
  Keywords: streaming, efficient, video generation, avatar, audio-driven, dit, distillation, interactive, identity, autoregressive  
- **[LiveAnimate: Stable Long-Form Streaming Human Animation in Real-Time](https://arxiv.org/abs/2608.11745v2)**  
  Authors: Yuxuan Zhang, Haozhong Xiong, Yubo Huang, Jiayi Song, Jinpeng Yu, Haofan Wang, Jiaming Liu, Ruihua Huang, Liwei Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.11745v2.pdf)  
  Keywords: streaming, benchmark, avatar, dit, video diffusion, distillation, human animation, diffusion transformer, interactive, identity, autoregressive, long-form  
- **[Omni-LiveAvatar: Minute-Level Real-Time Streaming Joint Audio-Video Avatar Generation](https://arxiv.org/abs/2608.13602v2)**  
  Authors: Lunjie Zhu, Xingtong Ge, Fangyu Lin, Yi Zhang, Zhening Liu, Mengfei Li, Yumeng Zhang, Guanglu Song, Yu Liu, Jun Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.13602v2.pdf) | [![GitHub](https://img.shields.io/github/stars/Aoko955/Omni-LiveAvatar?style=social)](https://github.com/Aoko955/Omni-LiveAvatar)  
  Keywords: streaming, avatar, denoising, video diffusion, distillation, diffusion model, interactive, autoregressive  

### Image-to-Video Generation

- **[DF26: We Cannot Tell Fake From Real Anymore](https://arxiv.org/abs/2609.07369v1)**  
  Authors: Severyn Shykula, Andrii Yermakov, Ivan Samarskyi, Dmytro Mishkin, Jan Cech, Anastasiia Mishchuk  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.07369v1.pdf)  
  Keywords: evaluation, image-to-video, text-to-video, benchmark  
- **[The Price of Consistency: Exploiting Visual Anchors for Multimodal Jailbreaking in Video Generation](https://arxiv.org/abs/2609.07216v1)**  
  Authors: Peng Li, Qianqian Xu, Yangbangyan Jiang, Zhipeng Yu, Qingming Huang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.07216v1.pdf)  
  Keywords: controllable, temporal consistency, benchmark, video generation, i2v, dit  
- **[PhysWeep: Does a Video Generator Realize the Physics You Ask For?](https://arxiv.org/abs/2609.06207v1)**  
  Authors: Rasul Khanbayov, Hasan Kurban  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.06207v1.pdf)  
  Keywords: world model, benchmark, physics, image-to-video, dit, dynamics, physical  
- **[TempJail: Temporal Jailbreak Attacks against Image-to-Video Generation Models](https://arxiv.org/abs/2608.26971v2)**  
  Authors: Qi Lu, Zehui Guo, David Yuanda Gan, Zijing Li, Hengda Zhang, Weijun Xu, Qiankun Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.26971v2.pdf) | [![GitHub](https://img.shields.io/github/stars/luqi-glory/TempJail?style=social)](https://github.com/luqi-glory/TempJail)  
  Keywords: evaluation, video synthesis, video generation, image-to-video, i2v, dit  
- **[Direct, Parallel, or Sequential? A Comparative Study of Training-Free Multi-Subject Image-to-Video Generation](https://arxiv.org/abs/2608.22819v1)**  
  Authors: Yanliang Qi, Kexi Chen, Muchao Ye, Haomiao Ni  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.22819v1.pdf)  
  Keywords: controllable, temporal consistency, video generation, image-to-video, i2v, dit  
- **[CaliBench: Are the Stochastic Dynamics of Video World Models Physically Calibrated?](https://arxiv.org/abs/2608.16829v2)**  
  Authors: Jonathan Sadeghi, Jenny Seidenschwarz, Jesse Allardice, Sirish Srinivasan, Benjamin Graham, Jeffrey Hawke  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.16829v2.pdf)  
  Keywords: world model, benchmark, image-to-video, dynamics, physical  
- **[EditStream: A Unified Autoregressive Framework for Interactive Video Generation and Editing](https://arxiv.org/abs/2608.21424v1)**  
  Authors: Yuqian Zhou, Zhenghong Zhou, Zongze Wu, Cameron Smith, Richard Zhang, Jiebo Luo, Eli Shechtman, Zhe Lin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.21424v1.pdf)  
  Keywords: streaming, video editing, text-to-video, efficient, video generation, image-to-video, dit, distillation, creative, video-to-video, interactive, autoregressive  
- **[RigidBench: Evaluating Rigid-Body Physics in Video Generation Models](https://arxiv.org/abs/2608.15555v1)**  
  Authors: Swarnim Jain, Shangzhe Wu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.15555v1.pdf)  
  Keywords: benchmark, video generation, denoising, physics, i2v, trajectory, diffusion transformer, identity  
- **[HPSD: Hybrid-Policy Self-Distillation for Text-Image-to-Video Diffusion Models](https://arxiv.org/abs/2608.13205v1)**  
  Authors: Jiazi Bu, Pengyang Ling, Yujie Zhou, Yibin Wang, Yuhang Zang, Xuanlang Dai, Shengyuan Ding, Tianyi Wei, Xiaohang Zhan, Jiaqi Wang, Tong Wu, Dahua Lin, Xingang Pan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.13205v1.pdf)  
  Keywords: text-to-video, image-to-video, i2v, video diffusion, dit, trajectory, architecture, diffusion model, distillation, t2v  
- **[Beyond Trial-and-Error: Agentic Optimization for Image-to-Video Adherence](https://arxiv.org/abs/2608.12290v1)**  
  Authors: Aman Tyagi, Hemanth Boinpally, Jonathan Chen, Douglas Gebert, Steven Hickson  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.12290v1.pdf)  
  Keywords: evaluation, video synthesis, efficient, video generation, image-to-video, i2v  

### Long Video Generation

*Showing the latest 50 out of 127 papers*

- **[Caption-once, Frames-on-Demand: Visual-Need Routing for Budget-Aware Agentic Long Video Understanding](https://arxiv.org/abs/2609.11899v1)**  
  Authors: Weitong Cai, Hang Zhang, Yukai Huang, Yiqiao Xie, Shan Gao, Jiankang Deng, Songcen Xu, Jifei Song, Zhensong Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.11899v1.pdf)  
  Keywords: dit, long video, benchmark  
- **[Uncertainty DMD: Restoring Diversity in Few-Step Autoregressive Video Distillation](https://arxiv.org/abs/2609.11265v1)**  
  Authors: Zixuan Duan, Xunzhi Xiang, Yabo Chen, Xin Zhang, Changhan Liu, Haibin Huang, Chi Zhang, Qi Fan, Xuelong Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.11265v1.pdf)  
  Keywords: video generation, dit, dynamics, distillation, autoregressive  
- **[Decoupled Self-Forcing Distillation for Streaming Talking Head Generation](https://arxiv.org/abs/2609.10317v1)**  
  Authors: Yanru An, Ruiyan Wang, Wenwu Wei, Rui Bu, Qi Wang, Hongwei Hu, Zhengxue Cheng, Rong Xie, Li Song, Wenjun Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.10317v1.pdf)  
  Keywords: streaming, dit, video diffusion, distillation, diffusion model, identity, autoregressive, talking head  
- **[Mask Forcing: Improving Autoregressive Video Diffusion Distillation via Dual-Noise Masking Rollout](https://arxiv.org/abs/2609.09123v1)**  
  Authors: Zhuoran Zhao, Shengju Qian, Tongtong Liang, Xianghao Kong, Songchun Zhang, Junchao Huang, Guian Fang, Xin Wang, Pan Hui, Anyi Rao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.09123v1.pdf)  
  Keywords: efficient, video generation, denoising, dit, video diffusion, distillation, diffusion model, autoregressive  
- **[Temporal State Transport in Video Generation: Diagnosing and Correcting Spectral Imbalance](https://arxiv.org/abs/2609.08505v1)**  
  Authors: Luyao Tang, Bingjun Luo, Dong Yi, Jialin Guo, Haoning Xi, Cheng Chen, Yizhou Yu, Chaoqi Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.08505v1.pdf) | [![GitHub](https://img.shields.io/github/stars/lytang63/temporal-state-transport?style=social)](https://github.com/lytang63/temporal-state-transport)  
  Keywords: temporal consistency, video generation, layout, identity  
- **[Better Call CineCrew: Consistent Ultra-Long Narrative-to-Film Generation](https://arxiv.org/abs/2609.07720v1)**  
  Authors: Jiaben Chen, Sixun Dong, Qinhong Zhou, Raine Ma, Zhiyang Dou, Wojciech Matusik, Chuang Gan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.07720v1.pdf)  
  Keywords: film, video generation, style, identity, long-form  
- **[The Price of Consistency: Exploiting Visual Anchors for Multimodal Jailbreaking in Video Generation](https://arxiv.org/abs/2609.07216v1)**  
  Authors: Peng Li, Qianqian Xu, Yangbangyan Jiang, Zhipeng Yu, Qingming Huang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.07216v1.pdf)  
  Keywords: controllable, temporal consistency, benchmark, video generation, i2v, dit  
- **[MVWeaver: A Hierarchical Music Video Generation Agent with a Learned Song-to-Visual Bridge](https://arxiv.org/abs/2609.06478v1)**  
  Authors: Sifei Li, Minyan Luo, Xu Li, Guodong Qi, Xincan Wang, Hanwen Wang, Chen Zhang, Pengfei Wan, Oliver Deussen, Weiming Dong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.06478v1.pdf)  
  Keywords: video generation, dit, architecture, music video, concept, long-form  
- **[Multi-Grid Post-Training for Long-Form Multi-Shot Video Generation](https://arxiv.org/abs/2609.06373v1)**  
  Authors: Jiawei Mao, Haoqin Tu, Hardy Chen, Yuhan Wang, Keyang Xu, Jieru Mei, Hongliang Fei, Ruogu Fang, Wei Shao, Cihang Xie, Yuyin Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.06373v1.pdf)  
  Keywords: benchmark, video generation, layout, denoising, long video, long-form  
- **[Object-Aware Background-Controlled Editing via Weighted Velocity Guidance](https://arxiv.org/abs/2609.06288v1)**  
  Authors: Wuji Wang, Yue Wu, Chenhao Yi, Shuhui Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.06288v1.pdf)  
  Keywords: temporal consistency, benchmark, denoising, dit, dynamics  

### Personalization & Customization

*Showing the latest 50 out of 83 papers*

- **[Vidu S2: Real-Time Interactive, Editable, and Spatial Video Generation](https://arxiv.org/abs/2609.11638v1)**  
  Authors: Jintao Zhang, Kai Jiang, Jintao Chen, Xu Wang, Deyuan Liu, Jungang Li, Dechuang Chen, Ming Lin, Jingjiang Zhou, Haopeng Jin, Qi Jia, Xiaohang Wang, Yaole Wang, Zhanqiang Zhang, Ran Li, Zhengkun Huang, Shuyue Xiong, Yuji Wang, Zikun Dai, Hui He, Yang Luo, Mang Ning, Weiqi Feng, Chengyang Ye, Xinyue Lin, Min Zhao, Hongzhou Zhu, Hengkai Tan, Zeyuan Wang, Chendong Xiang, Kaiwen Zheng, Zhijie Deng, Fan Bao, Jianfei Chen, Jun Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.11638v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://vidu.com/vidu-stream)  
  Keywords: video editing, video generation, avatar, style, dit, interactive  
- **[Harnessing Intrinsic Subject-Aware Attention for Controllable Multi-Subject Video Generation](https://arxiv.org/abs/2609.11507v1)**  
  Authors: Niange Yu, Ye Tian, Biaolong Chen, Miao Lu, Aixi Zhang, Hao Jiang, Yunhai Tong, Pipei Huang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.11507v1.pdf)  
  Keywords: controllable, benchmark, video generation, dit, diffusion transformer, identity  
- **[Decoupled Self-Forcing Distillation for Streaming Talking Head Generation](https://arxiv.org/abs/2609.10317v1)**  
  Authors: Yanru An, Ruiyan Wang, Wenwu Wei, Rui Bu, Qi Wang, Hongwei Hu, Zhengxue Cheng, Rong Xie, Li Song, Wenjun Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.10317v1.pdf)  
  Keywords: streaming, dit, video diffusion, distillation, diffusion model, identity, autoregressive, talking head  
- **[Temporal State Transport in Video Generation: Diagnosing and Correcting Spectral Imbalance](https://arxiv.org/abs/2609.08505v1)**  
  Authors: Luyao Tang, Bingjun Luo, Dong Yi, Jialin Guo, Haoning Xi, Cheng Chen, Yizhou Yu, Chaoqi Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.08505v1.pdf) | [![GitHub](https://img.shields.io/github/stars/lytang63/temporal-state-transport?style=social)](https://github.com/lytang63/temporal-state-transport)  
  Keywords: temporal consistency, video generation, layout, identity  
- **[VI-Bench: Benchmarking Prompt Inversion from AIGC Videos](https://arxiv.org/abs/2609.08079v1)**  
  Authors: Wulin Xie, Rui Zhao, Kecen Li, Xiujin Liu, Bokang Zhang, Zheng Liu, Xinwen Hou, Chen Gong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.08079v1.pdf)  
  Keywords: benchmark, video generation, style, dit, creative  
- **[Better Call CineCrew: Consistent Ultra-Long Narrative-to-Film Generation](https://arxiv.org/abs/2609.07720v1)**  
  Authors: Jiaben Chen, Sixun Dong, Qinhong Zhou, Raine Ma, Zhiyang Dou, Wojciech Matusik, Chuang Gan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.07720v1.pdf)  
  Keywords: film, video generation, style, identity, long-form  
- **[MVWeaver: A Hierarchical Music Video Generation Agent with a Learned Song-to-Visual Bridge](https://arxiv.org/abs/2609.06478v1)**  
  Authors: Sifei Li, Minyan Luo, Xu Li, Guodong Qi, Xincan Wang, Hanwen Wang, Chen Zhang, Pengfei Wan, Oliver Deussen, Weiming Dong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.06478v1.pdf)  
  Keywords: video generation, dit, architecture, music video, concept, long-form  
- **[EraseSAE: Surgical Concept Erasure in Text-to-Video Diffusion Models via Sparse Autoencoders](https://arxiv.org/abs/2609.03629v2)**  
  Authors: Xinghao Wang, Dong Li, Wei Yu, Yingwei Pan, Tao Gong, Qi Chu, Nenghai Yu, Ting Yao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.03629v2.pdf) | [![GitHub](https://img.shields.io/github/stars/HiDream-ai/EraseSAE?style=social)](https://github.com/HiDream-ai/EraseSAE)  
  Keywords: text-to-video, dit, video diffusion, diffusion model, concept, t2v  
- **[SolarWM: Open Data and Scalable Training for Long-Horizon Video World Models](https://arxiv.org/abs/2609.02886v1)**  
  Authors: Junchao Huang, Guian Fang, Shengju Qian, Xianghao Kong, Zhuoran Zhao, Wei Huang, Yihua Du, Zixin Zhang, Justin Cui, Yuchao Gu, Yukang Chen, Xinting Hu, Tianyu He, Shaoshuai Shi, Zhuotao Tian, Xin Wang, Mike Zheng Shou, Li Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.02886v1.pdf)  
  Keywords: world model, style, dit, architecture, distillation, interactive, autoregressive  
- **[Thinking in Pictures: A Systematic Benchmark for Reasoning-driven Image Generation](https://arxiv.org/abs/2609.02864v1)**  
  Authors: Yutong Liu, Nan Huang, Xu Cao, James M. Rehg  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.02864v1.pdf)  
  Keywords: evaluation, benchmark, video generation, concept, world simulator  

### Physical Understanding

*Showing the latest 50 out of 139 papers*

- **[MindTopo: Can Foundation Models Reason in Topological Space?](https://arxiv.org/abs/2609.11900v1)**  
  Authors: Yunfei Ge, Anbang Liu, Qineng Wang, Johnalbert Garnica, Jianwen Lyu, Zihan Wang, Reuben Tan, Jianfeng Gao, Ruohan Zhang, Yining Hong, Jiajun Wu, Manling Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.11900v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://mind-topo.github.io)  
  Keywords: evaluation, controllable, benchmark, video generation, dit, dynamics  
- **[Uncertainty DMD: Restoring Diversity in Few-Step Autoregressive Video Distillation](https://arxiv.org/abs/2609.11265v1)**  
  Authors: Zixuan Duan, Xunzhi Xiang, Yabo Chen, Xin Zhang, Changhan Liu, Haibin Huang, Chi Zhang, Qi Fan, Xuelong Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.11265v1.pdf)  
  Keywords: video generation, dit, dynamics, distillation, autoregressive  
- **[From Evaluation to Enhancement: Benchmarking and Improving Think-with-Video Reasoning for Video Generative Models](https://arxiv.org/abs/2609.11242v1)**  
  Authors: Meng Luo, Yicheng Liu, Jiahao Wang, Yuanxing Zhang, Xin Tao, Pengfei Wan, Kun Gai, Hao Fei  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.11242v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://huggingface.co/datasets/KlingTeam/VWG-Bench.) | [![Dataset](https://img.shields.io/badge/-Dataset-orange)](https://huggingface.co/datasets/KlingTeam/VWG-Bench)  
  Keywords: evaluation, video generation, physical, benchmark  
- **[VANTAGE-Bench: Evaluating the Infrastructure AI Gap in Vision-Language Models](https://arxiv.org/abs/2609.09396v1)**  
  Authors: Zaid Pervaiz Bhat, Nimra Nayyar, Arihant Jain, Lap Fung Chan, John Suchanek, Yu Wang, Varun Praveen, Tomasz Kornuta, Vidya Nariyambut Murali  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.09396v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://vantage-bench.org)  
  Keywords: evaluation, physical, trajectory, benchmark  
- **[DSE-VTG: Dual-Side Enhancement for Training-Free Video Temporal Grounding](https://arxiv.org/abs/2609.08850v1)**  
  Authors: Zhuo Cao, Bingqing Zhang, Sen Wang, Xue Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.08850v1.pdf)  
  Keywords: dit, dynamics, benchmark  
- **[Kairos: A Dataset for Fine-Grained Video-Language Modeling over Space, Time, and Dynamics](https://arxiv.org/abs/2609.08755v1)**  
  Authors: Ruibo Ming, Lei Sun, Deheng Zhang, He Zhang, Jialu Li, Jian Wang, Zhendong Li, Mengshun Hu, Danda Pani Paudel, Luc Van Gool, Jinjin Gu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.08755v1.pdf)  
  Keywords: evaluation, video generation, dynamics  
- **[Beyond Coherence: Benchmarking Professional Editing-Technique Execution in Multi-Shot Audio-Video Generation](https://arxiv.org/abs/2609.08275v1)**  
  Authors: Tianyi Zeng, Junchao Liao, Yujie Wei, Ziying Zhang, Litao Li, Tianyi Wang, Zhichao Wei, Shuyao Xu, Wenwen Qiang, Siyu Zhu, Zhenghao Zhang, Long Qin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.08275v1.pdf) | [![GitHub](https://img.shields.io/github/stars/AlibabaResearch/cut-craft-bench?style=social)](https://github.com/AlibabaResearch/cut-craft-bench)  
  Keywords: evaluation, benchmark, video generation, dit, physical  
- **[PhysFlow: Physics-Aware Optical Flow for Motion Controllable Video Generation](https://arxiv.org/abs/2609.08215v1)**  
  Authors: Cong Wang, Hanxin Zhu, Yonglin Tian, Jiayi Luo, Ruiqi Song, Boyi Sun, Long Chen, Zhibo Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.08215v1.pdf)  
  Keywords: controllable, video generation, physics, motion control, dit, dynamics, physics-aware, physical  
- **[Geodesic-informed Generative Diffusion Model For Topology-preserved Image Video Generation](https://arxiv.org/abs/2609.08153v1)**  
  Authors: Nian Wu, Nivetha Jayakumar, Jiarui Xing, Miaomiao Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.08153v1.pdf) | [![GitHub](https://img.shields.io/github/stars/nellie689/IGG?style=social)](https://github.com/nellie689/IGG)  
  Keywords: robotics, video generation, dynamics, diffusion model, physical  
- **[Identifying Habit, Physics, and Nuisance in Robot World Models](https://arxiv.org/abs/2609.09210v1)**  
  Authors: Jinting Hang, Zhenhui Cai  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.09210v1.pdf)  
  Keywords: world model, benchmark, video generation, physics, dynamics  

### Surveys & Benchmarks

*Showing the latest 50 out of 230 papers*

- **[MindTopo: Can Foundation Models Reason in Topological Space?](https://arxiv.org/abs/2609.11900v1)**  
  Authors: Yunfei Ge, Anbang Liu, Qineng Wang, Johnalbert Garnica, Jianwen Lyu, Zihan Wang, Reuben Tan, Jianfeng Gao, Ruohan Zhang, Yining Hong, Jiajun Wu, Manling Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.11900v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://mind-topo.github.io)  
  Keywords: evaluation, controllable, benchmark, video generation, dit, dynamics  
- **[Caption-once, Frames-on-Demand: Visual-Need Routing for Budget-Aware Agentic Long Video Understanding](https://arxiv.org/abs/2609.11899v1)**  
  Authors: Weitong Cai, Hang Zhang, Yukai Huang, Yiqiao Xie, Shan Gao, Jiankang Deng, Songcen Xu, Jifei Song, Zhensong Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.11899v1.pdf)  
  Keywords: dit, long video, benchmark  
- **[Harnessing Intrinsic Subject-Aware Attention for Controllable Multi-Subject Video Generation](https://arxiv.org/abs/2609.11507v1)**  
  Authors: Niange Yu, Ye Tian, Biaolong Chen, Miao Lu, Aixi Zhang, Hao Jiang, Yunhai Tong, Pipei Huang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.11507v1.pdf)  
  Keywords: controllable, benchmark, video generation, dit, diffusion transformer, identity  
- **[OmniHallu: Unified Hallucination Detection for Cross-Modal Comprehension and Generation in Multimodal Large Language Models](https://arxiv.org/abs/2609.11244v1)**  
  Authors: Jianjiang Yang, Peihang Li, Shanqing Xu, Mengchen Qian, Lu Zhang, Meng Luo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.11244v1.pdf)  
  Keywords: architecture, t2v, text-to-video, benchmark  
- **[From Evaluation to Enhancement: Benchmarking and Improving Think-with-Video Reasoning for Video Generative Models](https://arxiv.org/abs/2609.11242v1)**  
  Authors: Meng Luo, Yicheng Liu, Jiahao Wang, Yuanxing Zhang, Xin Tao, Pengfei Wan, Kun Gai, Hao Fei  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.11242v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://huggingface.co/datasets/KlingTeam/VWG-Bench.) | [![Dataset](https://img.shields.io/badge/-Dataset-orange)](https://huggingface.co/datasets/KlingTeam/VWG-Bench)  
  Keywords: evaluation, video generation, physical, benchmark  
- **[CamPilot: A Multi-Agent Cinematic Assistant for Camera-Controlled Movie Generation](https://arxiv.org/abs/2609.10943v1)**  
  Authors: Yang Wu, Stefano Petrangeli, Ishita Dasgupta, Yu Shen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.10943v1.pdf)  
  Keywords: controllable, text-to-video, benchmark, film, video generation  
- **[VANTAGE-Bench: Evaluating the Infrastructure AI Gap in Vision-Language Models](https://arxiv.org/abs/2609.09396v1)**  
  Authors: Zaid Pervaiz Bhat, Nimra Nayyar, Arihant Jain, Lap Fung Chan, John Suchanek, Yu Wang, Varun Praveen, Tomasz Kornuta, Vidya Nariyambut Murali  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.09396v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://vantage-bench.org)  
  Keywords: evaluation, physical, trajectory, benchmark  
- **[DSE-VTG: Dual-Side Enhancement for Training-Free Video Temporal Grounding](https://arxiv.org/abs/2609.08850v1)**  
  Authors: Zhuo Cao, Bingqing Zhang, Sen Wang, Xue Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.08850v1.pdf)  
  Keywords: dit, dynamics, benchmark  
- **[Kairos: A Dataset for Fine-Grained Video-Language Modeling over Space, Time, and Dynamics](https://arxiv.org/abs/2609.08755v1)**  
  Authors: Ruibo Ming, Lei Sun, Deheng Zhang, He Zhang, Jialu Li, Jian Wang, Zhendong Li, Mengshun Hu, Danda Pani Paudel, Luc Van Gool, Jinjin Gu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.08755v1.pdf)  
  Keywords: evaluation, video generation, dynamics  
- **[Beyond Coherence: Benchmarking Professional Editing-Technique Execution in Multi-Shot Audio-Video Generation](https://arxiv.org/abs/2609.08275v1)**  
  Authors: Tianyi Zeng, Junchao Liao, Yujie Wei, Ziying Zhang, Litao Li, Tianyi Wang, Zhichao Wei, Shuyao Xu, Wenwen Qiang, Siyu Zhu, Zhenghao Zhang, Long Qin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.08275v1.pdf) | [![GitHub](https://img.shields.io/github/stars/AlibabaResearch/cut-craft-bench?style=social)](https://github.com/AlibabaResearch/cut-craft-bench)  
  Keywords: evaluation, benchmark, video generation, dit, physical  

### Text-to-Video Generation

*Showing the latest 50 out of 70 papers*

- **[OmniHallu: Unified Hallucination Detection for Cross-Modal Comprehension and Generation in Multimodal Large Language Models](https://arxiv.org/abs/2609.11244v1)**  
  Authors: Jianjiang Yang, Peihang Li, Shanqing Xu, Mengchen Qian, Lu Zhang, Meng Luo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.11244v1.pdf)  
  Keywords: architecture, t2v, text-to-video, benchmark  
- **[CamPilot: A Multi-Agent Cinematic Assistant for Camera-Controlled Movie Generation](https://arxiv.org/abs/2609.10943v1)**  
  Authors: Yang Wu, Stefano Petrangeli, Ishita Dasgupta, Yu Shen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.10943v1.pdf)  
  Keywords: controllable, text-to-video, benchmark, film, video generation  
- **[DF26: We Cannot Tell Fake From Real Anymore](https://arxiv.org/abs/2609.07369v1)**  
  Authors: Severyn Shykula, Andrii Yermakov, Ivan Samarskyi, Dmytro Mishkin, Jan Cech, Anastasiia Mishchuk  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.07369v1.pdf)  
  Keywords: evaluation, image-to-video, text-to-video, benchmark  
- **[Adapting Vision Foundation Models to Acoustics for Pose-Free 3D Sonar Reconstruction](https://arxiv.org/abs/2609.06261v1)**  
  Authors: Kevin Zhang, Jingxi Chen, Mohamad Qadri, Russell Shomberg, Michael Kaess, Jia-Bin Huang, Adithya Pediredla, Christopher Metzler  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.06261v1.pdf)  
  Keywords: text-to-video, efficient, video generation, physics, dit  
- **[ReaDiT Guidance: Control for Image and Video Generation using Diffusion Transformer Features](https://arxiv.org/abs/2609.04649v1)**  
  Authors: Jay Mahajan, Chang Liu, Rauf Makharov, Viraj Shah, Alexander Schwing, Svetlana Lazebnik  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.04649v1.pdf)  
  Keywords: text-to-video, video generation, motion control, dit, diffusion transformer  
- **[DSAQuant: Denoising-Stage-Aligned Quantization-Aware Training for Video Generation](https://arxiv.org/abs/2609.04031v1)**  
  Authors: Shuaiting Li, Zelin Gao, Haibin Shen, Yujun Shen, Haotong Qin, Yinghao Xu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.04031v1.pdf)  
  Keywords: text-to-video, video generation, layout, denoising, video diffusion, distillation, diffusion model  
- **[EraseSAE: Surgical Concept Erasure in Text-to-Video Diffusion Models via Sparse Autoencoders](https://arxiv.org/abs/2609.03629v2)**  
  Authors: Xinghao Wang, Dong Li, Wei Yu, Yingwei Pan, Tao Gong, Qi Chu, Nenghai Yu, Ting Yao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.03629v2.pdf) | [![GitHub](https://img.shields.io/github/stars/HiDream-ai/EraseSAE?style=social)](https://github.com/HiDream-ai/EraseSAE)  
  Keywords: text-to-video, dit, video diffusion, diffusion model, concept, t2v  
- **[Step Back to Move Forward: Reflection-Aware Preference Optimization for Visual Generation](https://arxiv.org/abs/2609.04282v1)**  
  Authors: Junlong Wu, Jiuzhou Lin, Jia Sun, Boheng Zhang, Huaiqing Wang, Dewen Fan, Houde Liu, Qianqian Gan, Fan Yang, Tingting Gao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.04282v1.pdf)  
  Keywords: text-to-video, efficient, architecture, diffusion model, t2v  
- **[NoisEasier: Test-Time Noise Optimization for Text-to-Video Generation](https://arxiv.org/abs/2608.30194v1)**  
  Authors: Yujiang Pu, Yu Kong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.30194v1.pdf)  
  Keywords: controllable, text-to-video, efficient, video generation, dit, trajectory, diffusion model, t2v  
- **[Off-Manifold Refinement: Guiding Video Generators with a Frozen World Model](https://arxiv.org/abs/2608.29904v1)**  
  Authors: Hai Nguyen-Truong, Tuan-Anh Vu, Dang Huynh  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.29904v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://itruonghai.github.io/omr)  
  Keywords: world model, physical, denoising, dit, dynamics, trajectory, t2v  

### Video Editing

- **[Vidu S2: Real-Time Interactive, Editable, and Spatial Video Generation](https://arxiv.org/abs/2609.11638v1)**  
  Authors: Jintao Zhang, Kai Jiang, Jintao Chen, Xu Wang, Deyuan Liu, Jungang Li, Dechuang Chen, Ming Lin, Jingjiang Zhou, Haopeng Jin, Qi Jia, Xiaohang Wang, Yaole Wang, Zhanqiang Zhang, Ran Li, Zhengkun Huang, Shuyue Xiong, Yuji Wang, Zikun Dai, Hui He, Yang Luo, Mang Ning, Weiqi Feng, Chengyang Ye, Xinyue Lin, Min Zhao, Hongzhou Zhu, Hengkai Tan, Zeyuan Wang, Chendong Xiang, Kaiwen Zheng, Zhijie Deng, Fan Bao, Jianfei Chen, Jun Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.11638v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://vidu.com/vidu-stream)  
  Keywords: video editing, video generation, avatar, style, dit, interactive  
- **[PAI-Actor: Cinematic Multi-Character Replacement in Dynamic Scenes](https://arxiv.org/abs/2609.05918v1)**  
  Authors: Bangxun Tang, Heyuan Gao, Yiren Song, Guian Fang, Zijian He, Jie Yang, Mike Zheng Shou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.05918v1.pdf)  
  Keywords: efficient, video generation, film, video-to-video, dynamics, distillation, diffusion transformer, autoregressive, long-form  
- **[FixAnything: 3D-Consistent Rendering Refinement via Video Generative Priors](https://arxiv.org/abs/2608.23549v1)**  
  Authors: Khiem Vuong, Deva Ramanan, Srinivasa Narasimhan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.23549v1.pdf)  
  Keywords: video-to-video, architecture, video translation  
- **[InfinityEdit: Infinite Video Editing with a Lightweight Edit-Ignition Adapter](https://arxiv.org/abs/2608.20910v1)**  
  Authors: Yunze Tong, Mushui Liu, Canyu Zhao, Shiyi Zhang, Didi Zhu, Peng Zhang, Wanggui He, Jinlong Liu, Ying Chen, Hao Jiang, Pipei Huang, Bo Zheng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.20910v1.pdf)  
  Keywords: dit, streaming, denoising, video editing  
- **[Identity-Preserving Text-to-Video Generation via Agentic Enhancement and Semantic Repair](https://arxiv.org/abs/2608.20749v1)**  
  Authors: Jiayi Gao, Changcheng Hua, Jiaqi Tang, Yuxin Peng, Yang Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.20749v1.pdf) | [![GitHub](https://img.shields.io/github/stars/oceanflowlab/AESR?style=social)](https://github.com/oceanflowlab/AESR)  
  Keywords: evaluation, video editing, text-to-video, video generation, dit, identity  
- **[EditStream: A Unified Autoregressive Framework for Interactive Video Generation and Editing](https://arxiv.org/abs/2608.21424v1)**  
  Authors: Yuqian Zhou, Zhenghong Zhou, Zongze Wu, Cameron Smith, Richard Zhang, Jiebo Luo, Eli Shechtman, Zhe Lin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.21424v1.pdf)  
  Keywords: streaming, video editing, text-to-video, efficient, video generation, image-to-video, dit, distillation, creative, video-to-video, interactive, autoregressive  
- **[Instruction-Based Video Editing by Repurposing an Image Editing Model](https://arxiv.org/abs/2608.14790v3)**  
  Authors: Yunpeng Bai, Yossi Gandelsman, Michaël Gharbi, Qixing Huang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.14790v3.pdf) | [![GitHub](https://img.shields.io/github/stars/yunpeng1998/Qwen-Video-Edit?style=social)](https://github.com/yunpeng1998/Qwen-Video-Edit) | [![Project](https://img.shields.io/badge/-Project-blue)](https://yunpeng1998.github.io/Qwen-Video-Edit-Page) | [![HuggingFace](https://img.shields.io/badge/-HuggingFace-yellow)](https://huggingface.co/yunpeng1998/Qwen-Video-Edit)  
  Keywords: video editing, denoising, dit, video diffusion, diffusion transformer  
- **[EgoPlay: Event-Triggered Video Editing for Egocentric Streams](https://arxiv.org/abs/2607.24560v1)**  
  Authors: Jinjie Mai, Gordon Guocheng Qian, Willi Menapace, Arpit Sahni, Chaoyang Wang, Ashkan Mirzaei, Runjia Li, Sergey Tulyakov, Bernard Ghanem, Peter Wonka, Rameen Abdal  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.24560v1.pdf)  
  Keywords: evaluation, video editing, benchmark, video-to-video, dit, video diffusion, diffusion transformer  
- **[ID-V2V: Identity-Preserving Video Restylization](https://arxiv.org/abs/2607.22830v2)**  
  Authors: Yuancheng Xu, Mingming He, Pablo Salamanca, Li Ma, Yash Kant, Emmett Steven, Paul Debevec, Ning Yu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.22830v2.pdf) | [![GitHub](https://img.shields.io/github/stars/Eyeline-Labs/ID-V2V?style=social)](https://github.com/Eyeline-Labs/ID-V2V)  
  Keywords: video synthesis, style, dit, creative, video-to-video, identity  
- **[OSVE: One Step Video Editing with One Step Diffusion Models](https://arxiv.org/abs/2607.19895v1)**  
  Authors: Habin Lim, Gyeong-Moon Park  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.19895v1.pdf) | [![GitHub](https://img.shields.io/github/stars/KU-VGI/OSVE?style=social)](https://github.com/KU-VGI/OSVE)  
  Keywords: temporal consistency, video editing, dit, diffusion model, long video  

### Video Inpainting & Completion

- **[AcrossVAM1.0: Particle World Modeling for Text-Assisted Robot Video Prediction](https://arxiv.org/abs/2608.28491v1)**  
  Authors: Yafei Zhang, Nan Wu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.28491v1.pdf)  
  Keywords: world model, benchmark, film, dynamics, trajectory, video prediction  
- **[V-RAE: Rethinking Video Latent Spaces for Generation](https://arxiv.org/abs/2608.13556v1)**  
  Authors: Minghui Guo, Shengqiong Wu, Hao Fei  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.13556v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://v-rae.github.io)  
  Keywords: video generation, latent video, dit, architecture, video prediction  
- **[GeoRoute: Geometry-Aware Hybrid Inference for Traffic Future-Frame Prediction](https://arxiv.org/abs/2608.09493v1)**  
  Authors: Khang Minh Le, Hieu Dinh Trung Pham, Luu Thanh Danh, Nam-Tien Le, Hieu Anh Ngo, Phuong Huu Vu Tran, Son Nguyen Minh Le, Nguyen Trong Nghia, Tu Tran Thi Cam, Huy Minh Nhat Nguyen, Cuong Tuan Nguyen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.09493v1.pdf)  
  Keywords: benchmark, latent video, autonomous driving, dit, video diffusion, architecture, diffusion model, video prediction  
- **[SimWAM: A Simple World Action Model for End-to-End Autonomous Driving](https://arxiv.org/abs/2608.07468v4)**  
  Authors: Zongchuang Zhao, Xin Zhou, Tianyang Xu, Zhengyang Sun, Kaixuan Zhou, Yu Wu, Honglin Li, Dingkang Liang, Xiang Bai  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.07468v4.pdf) | [![GitHub](https://img.shields.io/github/stars/H-EmbodVis/SimWAM?style=social)](https://github.com/H-EmbodVis/SimWAM)  
  Keywords: flow matching, efficient, video generation, autonomous driving, dynamics, trajectory, video prediction  
- **[MirrorWorld: Taming Video Diffusion Models for Mirror Reflection Generation](https://arxiv.org/abs/2608.07463v1)**  
  Authors: Youjun Zhao, Alex Warren, Gary K. L. Tam, Rynson W. H. Lau  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.07463v1.pdf)  
  Keywords: benchmark, video synthesis, video diffusion, distillation, diffusion model, video inpainting  
- **[UniVVT: A Unified End-to-End Framework for High-Fidelity Video Virtual Try-on](https://arxiv.org/abs/2608.05745v2)**  
  Authors: Yushe Cao, Shikun Feng, Fei Shen, Haikuo Peng, Jianqiang Xia, Yiheng Zhu, Dianxi Shi, Chun Yu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.05745v2.pdf)  
  Keywords: benchmark, virtual try-on, video generation, dit, dynamics, video inpainting, identity  
- **[CrossScope: A Role-Asymmetric World Model for Joint Dual-Scope Surgical Video Prediction](https://arxiv.org/abs/2608.03211v1)**  
  Authors: Wanhao Liu, Jinsong Lin, Rulin Zhou, Chi Kit Ng, Wenbin Pan, Zhiqing Tang, Dongyue Li, Liwei Luo, Yanshen Wu, Panshuo Li, Zhiyong Xiong, Huxin Gao, Tamas Haidegger, Hongliang Ren  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.03211v1.pdf)  
  Keywords: evaluation, world model, benchmark, video generation, dynamics, video prediction  
- **[Schrödinger's Cat: Probabilistic Representation and Prediction of Potential Scene Kinematics](https://arxiv.org/abs/2607.25984v1)**  
  Authors: Timy Phan, Jannik Wiese, Björn Ommer  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.25984v1.pdf)  
  Keywords: efficient, video generation, dit, trajectory, interactive, video prediction  
- **[The Seriality Gap in Video Diffusion Models](https://arxiv.org/abs/2607.13031v1)**  
  Authors: Jorge Diaz Chao, Konpat Preechakul, Yuxi Liu, Yutong Bai  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.13031v1.pdf)  
  Keywords: denoising, video diffusion, dynamics, diffusion model, simulation, autoregressive, video prediction  
- **[Video Generation Models Are Inherent Lighting Estimators](https://arxiv.org/abs/2607.04674v1)**  
  Authors: Ziqi Cai, Shuchen Weng, Kaiqi Liu, Zifeng Wang, Zhiquan Zhang, Minggui Teng, Han Jiang, Boxin Shi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2607.04674v1.pdf)  
  Keywords: efficient, video generation, video diffusion, diffusion model, video inpainting, physical  

### Video Super-Resolution & Enhancement

*Showing the latest 50 out of 81 papers*

- **[Mask Forcing: Improving Autoregressive Video Diffusion Distillation via Dual-Noise Masking Rollout](https://arxiv.org/abs/2609.09123v1)**  
  Authors: Zhuoran Zhao, Shengju Qian, Tongtong Liang, Xianghao Kong, Songchun Zhang, Junchao Huang, Guian Fang, Xin Wang, Pan Hui, Anyi Rao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.09123v1.pdf)  
  Keywords: efficient, video generation, denoising, dit, video diffusion, distillation, diffusion model, autoregressive  
- **[Multi-Grid Post-Training for Long-Form Multi-Shot Video Generation](https://arxiv.org/abs/2609.06373v1)**  
  Authors: Jiawei Mao, Haoqin Tu, Hardy Chen, Yuhan Wang, Keyang Xu, Jieru Mei, Hongliang Fei, Ruogu Fang, Wei Shao, Cihang Xie, Yuyin Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.06373v1.pdf)  
  Keywords: benchmark, video generation, layout, denoising, long video, long-form  
- **[Object-Aware Background-Controlled Editing via Weighted Velocity Guidance](https://arxiv.org/abs/2609.06288v1)**  
  Authors: Wuji Wang, Yue Wu, Chenhao Yi, Shuhui Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.06288v1.pdf)  
  Keywords: temporal consistency, benchmark, denoising, dit, dynamics  
- **[DSAQuant: Denoising-Stage-Aligned Quantization-Aware Training for Video Generation](https://arxiv.org/abs/2609.04031v1)**  
  Authors: Shuaiting Li, Zelin Gao, Haibin Shen, Yujun Shen, Haotong Qin, Yinghao Xu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.04031v1.pdf)  
  Keywords: text-to-video, video generation, layout, denoising, video diffusion, distillation, diffusion model  
- **[Physically Plausible Video Generation via Visual-Semantic Chain-of-Events Conditioning](https://arxiv.org/abs/2609.00656v1)**  
  Authors: Zixuan Wang, Yixin Hu, Wen Li, Feng Chen, Yan Liu, Duo Peng, Yinjie Lei  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.00656v1.pdf)  
  Keywords: video generation, denoising, physics, dit, dynamics, physical  
- **[DreamX-Creator: Democratizing Native Audio-Video Generation at 2K Resolution](https://arxiv.org/abs/2608.31106v1)**  
  Authors: Jiashu Zhu, Yanhao Zheng, Ruitian Tian, Rujing Dang, Shen Zhang, Bingze Song, Jiachen Lei, Ruimin Lin, Jiahong Wu, Xiangxiang Chu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.31106v1.pdf)  
  Keywords: evaluation, video generation, denoising, dit, dynamics, autoregressive  
- **[Off-Manifold Refinement: Guiding Video Generators with a Frozen World Model](https://arxiv.org/abs/2608.29904v1)**  
  Authors: Hai Nguyen-Truong, Tuan-Anh Vu, Dang Huynh  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.29904v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://itruonghai.github.io/omr)  
  Keywords: world model, physical, denoising, dit, dynamics, trajectory, t2v  
- **[On the Resilience of Text-to-Video Diffusion Models to Hardware Faults](https://arxiv.org/abs/2608.29598v1)**  
  Authors: Zachary Coalson, A M Aahad, Stella Doehring, Zane Ma, Sanghyun Hong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.29598v1.pdf) | [![GitHub](https://img.shields.io/github/stars/ztcoalson/T2V-Resilience?style=social)](https://github.com/ztcoalson/T2V-Resilience)  
  Keywords: text-to-video, benchmark, video generation, denoising, video diffusion, diffusion model, t2v  
- **[Test-Time Scaling for Video Diffusion Models via Diagnosis-Guided Candidate Recycling](https://arxiv.org/abs/2608.29322v1)**  
  Authors: Hangzhou He, Lunhao Duan, Shanshan Zhao, Kaiwen Li, Qing-Guo Chen, Weihua Luo, Yanye Lu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.29322v1.pdf)  
  Keywords: evaluation, layout, denoising, dit, video diffusion, diffusion model  
- **[ClearText-Video: A Large-Scale Text-Centric Video Dataset Bridging Video Restoration and Scene-Text Enhancement](https://arxiv.org/abs/2608.28784v1)**  
  Authors: Jinlong Li, Jiaming Ding, Dingfu Lu, Malcolm Hsiu, Chuang Ke, Kangning Yang, Bochen Guan, Lan Fu, Jie Cai, Huiming Sun, Zibo Meng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.28784v1.pdf)  
  Keywords: video restoration, dit, benchmark  

### World Models & Simulation

*Showing the latest 50 out of 109 papers*

- **[Vidu S2: Real-Time Interactive, Editable, and Spatial Video Generation](https://arxiv.org/abs/2609.11638v1)**  
  Authors: Jintao Zhang, Kai Jiang, Jintao Chen, Xu Wang, Deyuan Liu, Jungang Li, Dechuang Chen, Ming Lin, Jingjiang Zhou, Haopeng Jin, Qi Jia, Xiaohang Wang, Yaole Wang, Zhanqiang Zhang, Ran Li, Zhengkun Huang, Shuyue Xiong, Yuji Wang, Zikun Dai, Hui He, Yang Luo, Mang Ning, Weiqi Feng, Chengyang Ye, Xinyue Lin, Min Zhao, Hongzhou Zhu, Hengkai Tan, Zeyuan Wang, Chendong Xiang, Kaiwen Zheng, Zhijie Deng, Fan Bao, Jianfei Chen, Jun Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.11638v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://vidu.com/vidu-stream)  
  Keywords: video editing, video generation, avatar, style, dit, interactive  
- **[PRG-Fusion: Orchestrating Generative Priors with Reconstruction Evidence for Driving View Synthesis](https://arxiv.org/abs/2609.06948v1)**  
  Authors: Sipeng He, Jialei Chen, Zhen Fang, Dongchun Ren, Feng Zhao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.06948v1.pdf)  
  Keywords: video synthesis, simulation, trajectory  
- **[Identifying Habit, Physics, and Nuisance in Robot World Models](https://arxiv.org/abs/2609.09210v1)**  
  Authors: Jinting Hang, Zhenhui Cai  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.09210v1.pdf)  
  Keywords: world model, benchmark, video generation, physics, dynamics  
- **[PhysWeep: Does a Video Generator Realize the Physics You Ask For?](https://arxiv.org/abs/2609.06207v1)**  
  Authors: Rasul Khanbayov, Hasan Kurban  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.06207v1.pdf)  
  Keywords: world model, benchmark, physics, image-to-video, dit, dynamics, physical  
- **[TourPhysics: Bringing Physics to World Models for Exploration and Manipulation from a Single Image](https://arxiv.org/abs/2609.04911v2)**  
  Authors: Xin Zhang, Yabo Chen, Zixuan Duan, Haibin Huang, Chi Zhang, Feng Xu, Xuelong Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.04911v2.pdf)  
  Keywords: world model, video synthesis, video generation, physical, physics, dit, trajectory, simulation, interactive  
- **[Building Pretraining Data for World Models: An Unreal Engine-Based Pipeline for Action-Conditioned Video Generation](https://arxiv.org/abs/2609.03557v1)**  
  Authors: Haoyu Wang, Songchun Zhang, Haoran Li, Haoyang Huang, Zeyue Xue, Nan Duan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.03557v1.pdf)  
  Keywords: world model, video generation, physics, dit, architecture, multi-view video, trajectory, action-conditioned  
- **[SolarWM: Open Data and Scalable Training for Long-Horizon Video World Models](https://arxiv.org/abs/2609.02886v1)**  
  Authors: Junchao Huang, Guian Fang, Shengju Qian, Xianghao Kong, Zhuoran Zhao, Wei Huang, Yihua Du, Zixin Zhang, Justin Cui, Yuchao Gu, Yukang Chen, Xinting Hu, Tianyu He, Shaoshuai Shi, Zhuotao Tian, Xin Wang, Mike Zheng Shou, Li Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.02886v1.pdf)  
  Keywords: world model, style, dit, architecture, distillation, interactive, autoregressive  
- **[Thinking in Pictures: A Systematic Benchmark for Reasoning-driven Image Generation](https://arxiv.org/abs/2609.02864v1)**  
  Authors: Yutong Liu, Nan Huang, Xu Cao, James M. Rehg  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.02864v1.pdf)  
  Keywords: evaluation, benchmark, video generation, concept, world simulator  
- **[Spatially Aware World Action Model via Geometric Latent Diffusion](https://arxiv.org/abs/2609.02531v1)**  
  Authors: Javier Alejandro Lopetegui Gonzalez, Paul Pacaud, Cordelia Schmid  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.02531v1.pdf)  
  Keywords: evaluation, world model, benchmark, 3d-aware, video diffusion, diffusion model, physical  
- **[H3-World: Turning Language Understanding into World Control](https://arxiv.org/abs/2609.01560v1)**  
  Authors: Danze Chen, Zeqing Wang, Ziyue Lin, Xingyi Yang, Yeying Jin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.01560v1.pdf)  
  Keywords: efficient, camera control, interactive, world model  



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
