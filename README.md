# Awesome Video Diffusions [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of latest research papers, projects and resources related to Video Diffusion Models and Video Generation. Content is automatically updated daily.

> Last Update: 2026-09-24 03:12:53

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

- [3D-aware Video Generation](#3d-aware-video-generation) (14 papers) - Video generation with 3D awareness, multi-view consistency, and 4D content creation
- [Applications](#applications) (40 papers) - Domain-specific applications of video diffusion models
- [Architecture & Efficiency](#architecture-&-efficiency) (343 papers) - Architectural innovations (DiT, UNet), flow matching, and training/inference efficiency
- [Audio & Multi-modal](#audio-&-multi-modal) (26 papers) - Audio-driven and multi-modal conditioned video generation
- [Controllable Generation](#controllable-generation) (115 papers) - Controllable video generation with motion, camera, pose, or layout guidance
- [Human & Character Animation](#human-&-character-animation) (21 papers) - Human-centric video generation including talking heads, dance, and character animation
- [Image-to-Video Generation](#image-to-video-generation) (42 papers) - Methods for animating still images into videos
- [Long Video Generation](#long-video-generation) (121 papers) - Generating temporally consistent long-form videos beyond short clips
- [Personalization & Customization](#personalization-&-customization) (82 papers) - Personalized video generation with custom subjects, identities, or styles
- [Physical Understanding](#physical-understanding) (138 papers) - Physics-aware video generation and dynamics modeling
- [Surveys & Benchmarks](#surveys-&-benchmarks) (230 papers) - Survey papers, benchmarks, and evaluation metrics for video generation
- [Text-to-Video Generation](#text-to-video-generation) (72 papers) - Foundation models and methods for generating videos from text prompts
- [Video Editing](#video-editing) (18 papers) - Diffusion-based video editing, style transfer, and manipulation
- [Video Inpainting & Completion](#video-inpainting-&-completion) (12 papers) - Video inpainting, completion, outpainting, and temporal prediction
- [Video Super-Resolution & Enhancement](#video-super-resolution-&-enhancement) (79 papers) - Video quality improvement, upscaling, restoration, and frame interpolation
- [World Models & Simulation](#world-models-&-simulation) (103 papers) - Video generation as world simulators and interactive environment generation



## Table of Contents

- [Categorized Papers](#categorized-papers)
- [Classic Papers](#classic-papers)
- [Open Source Projects](#open-source-projects)
- [Applications](#applications)
- [Tutorials & Blogs](#tutorials--blogs)





## Categorized Papers

### 3D-aware Video Generation

- **[WorldCrafter: Consistent Video World Model with Implicit 3D-aware Memory](https://arxiv.org/abs/2609.24984v1)**  
  Authors: Wangbo Yu, Kunhao Liu, Wenbo Hu, Shenghai Yuan, Chaoran Feng, Haiyang Zhou, Yukun Huang, Yiran Wang, Wang Zhao, Yingmin Luo, Ying Shan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.24984v1.pdf)  
  Keywords: streaming, interactive, 3d-aware, distillation, dit, denoising, world model  
- **[Printing the Underdetermined: Materializing Multi-solutionness in Figurative Paintings](https://arxiv.org/abs/2609.19782v1)**  
  Authors: Yutao Ming, Teng Xu, Youjia Wang, Yunyang Liu, Fengmin Yang, Fuqiang Zhao, Jingyi Yu, Hua Yang, Yanjun Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.19782v1.pdf)  
  Keywords: dit, multi-view video, physical  
- **[Rethinking 3D Noise: Learning 3D-Aware Video Priors via Optimization-Free Morphological Perturbations](https://arxiv.org/abs/2609.03657v1)**  
  Authors: Onat Şahin, Mohammad Altillawi, George Eskandar, Carlos Carbone, Ziyuan Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.03657v1.pdf)  
  Keywords: 3d-aware, robotics, video diffusion  
- **[Stabilizing Camera-Controlled Novel View Synthesis at Inference Time](https://arxiv.org/abs/2609.03639v1)**  
  Authors: Prajwal Singh, Arjun Badola, Seema Kumari, Hajime Nagahara, Shanmuganathan Raman  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.03639v1.pdf)  
  Keywords: autoregressive, diffusion model, video diffusion, efficient, novel view  
- **[Building Pretraining Data for World Models: An Unreal Engine-Based Pipeline for Action-Conditioned Video Generation](https://arxiv.org/abs/2609.03557v1)**  
  Authors: Haoyu Wang, Songchun Zhang, Haoran Li, Haoyang Huang, Zeyue Xue, Nan Duan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.03557v1.pdf)  
  Keywords: physics, trajectory, architecture, action-conditioned, multi-view video, dit, video generation, world model  
- **[RoGe: Novel View Synthesis via End-to-End Implicit Reconstruction and Generation](https://arxiv.org/abs/2609.02847v2)**  
  Authors: Xiaolei Lang, Ze Kang, Zehao Huang, Naiyan Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.02847v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://jerry-locker.github.io/roge)  
  Keywords: temporal consistency, trajectory, diffusion model, video diffusion, dit, novel view  
- **[Spatially Aware World Action Model via Geometric Latent Diffusion](https://arxiv.org/abs/2609.02531v1)**  
  Authors: Javier Alejandro Lopetegui Gonzalez, Paul Pacaud, Cordelia Schmid  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.02531v1.pdf)  
  Keywords: benchmark, physical, diffusion model, 3d-aware, video diffusion, world model, evaluation  
- **[Streaming4D: Accelerate 4D World Models via Block-wise Video Generation and Incremental Reconstruction](https://arxiv.org/abs/2609.00610v2)**  
  Authors: Xiaoyan Liu, Jiaxin Liu, Kangrui Li, Sifan Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.00610v2.pdf)  
  Keywords: streaming, interactive, autoregressive, style, dit, 4d generation, video generation, world model  
- **[GaussVid: Sparse-View Gaussian Splatting with 3D-Aware Video Diffusion Priors](https://arxiv.org/abs/2608.21849v1)**  
  Authors: Xinhui Liu, Can Wang, Wei Jiang, Wei Wang, Dong Xu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.21849v1.pdf)  
  Keywords: diffusion model, 3d-aware, video generation, video diffusion, dit, video restoration, novel view  
- **[Grounded-Exo2Ego: Structured Semantic Grounding for Robust Exocentric-to-Egocentric Video Generation](https://arxiv.org/abs/2608.20534v1)**  
  Authors: Shengze Wang, Michael Stengel, Tianye Li, Seonwook Park, Amrita Mazumdar, Koki Nagano, Alex Trevithick, Shalini De Mello  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.20534v1.pdf)  
  Keywords: physical, diffusion model, video generation, video diffusion, dit, evaluation, novel view  

### Applications

- **[UniK: Universal Knowledge Perception for Digital and Physical AI](https://arxiv.org/abs/2609.23971v1)**  
  Authors: Nirmit Desai, Kunal Sawarkar, Aditya Mahakali, Dongkon Lee, Kevin Park, Eric Song  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.23971v1.pdf)  
  Keywords: physical, world model, evaluation, efficient, medical  
- **[Astronex-World 1.0: Real-Time Interactive World Model Foundation](https://arxiv.org/abs/2609.20034v1)**  
  Authors: Xin Zhou, Cong Miao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.20034v1.pdf)  
  Keywords: text-to-video, controllable, image-to-video, interactive, autonomous driving, dynamics, i2v, world model  
- **[World-Action Models for Robot Learning and Control: A Survey](https://arxiv.org/abs/2609.16074v1)**  
  Authors: Zuxing Lu, Hongjia Zhai, Guanzhi Wang, Huajian Zeng, Jiaqi Yang, Jingyu Liu, Lei Cheng, Yuantai Zhang, Yuheng Qiu, Zezhou Cheng, Ivan Laptev, Danfei Xu, Benjamin Riviere, Giuseppe Loianno, Eric Xing, Xingxing Zuo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.16074v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://rcl-robotics.github.io/Awesome-World-Action-Models)  
  Keywords: benchmark, architecture, physical, action-conditioned, simulation, survey, dit, autonomous driving, video generation, world model, robotics, efficient  
- **[Dynamic Learning Solutions: A System for Personalized Educational Video Generation](https://arxiv.org/abs/2609.14408v1)**  
  Authors: Siddhanth Sridhar, Shreya Chaurasia, Baddela Sai Yaswantha Reddy, Deepak Parmar, Shylaja S S  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.14408v1.pdf)  
  Keywords: interactive, education, multi-modal, style, video generation  
- **[CamPilot: A Multi-Agent Cinematic Assistant for Camera-Controlled Movie Generation](https://arxiv.org/abs/2609.10943v1)**  
  Authors: Yang Wu, Stefano Petrangeli, Ishita Dasgupta, Yu Shen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.10943v1.pdf)  
  Keywords: text-to-video, benchmark, controllable, film, video generation  
- **[Geodesic-informed Generative Diffusion Model For Topology-preserved Image Video Generation](https://arxiv.org/abs/2609.08153v1)**  
  Authors: Nian Wu, Nivetha Jayakumar, Jiarui Xing, Miaomiao Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.08153v1.pdf) | [![GitHub](https://img.shields.io/github/stars/nellie689/IGG?style=social)](https://github.com/nellie689/IGG)  
  Keywords: physical, diffusion model, dynamics, video generation, robotics  
- **[VI-Bench: Benchmarking Prompt Inversion from AIGC Videos](https://arxiv.org/abs/2609.08079v1)**  
  Authors: Wulin Xie, Rui Zhao, Kecen Li, Xiujin Liu, Bokang Zhang, Zheng Liu, Xinwen Hou, Chen Gong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.08079v1.pdf)  
  Keywords: benchmark, style, video generation, creative, dit  
- **[Better Call CineCrew: Consistent Ultra-Long Narrative-to-Film Generation](https://arxiv.org/abs/2609.07720v1)**  
  Authors: Jiaben Chen, Sixun Dong, Qinhong Zhou, Raine Ma, Zhiyang Dou, Wojciech Matusik, Chuang Gan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.07720v1.pdf)  
  Keywords: identity, film, style, long-form, video generation  
- **[PAI-Actor: Cinematic Multi-Character Replacement in Dynamic Scenes](https://arxiv.org/abs/2609.05918v1)**  
  Authors: Bangxun Tang, Heyuan Gao, Yiren Song, Guian Fang, Zijian He, Jie Yang, Mike Zheng Shou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.05918v1.pdf)  
  Keywords: video-to-video, film, autoregressive, distillation, diffusion transformer, long-form, dynamics, video generation, efficient  
- **[Rethinking 3D Noise: Learning 3D-Aware Video Priors via Optimization-Free Morphological Perturbations](https://arxiv.org/abs/2609.03657v1)**  
  Authors: Onat Şahin, Mohammad Altillawi, George Eskandar, Carlos Carbone, Ziyuan Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.03657v1.pdf)  
  Keywords: 3d-aware, robotics, video diffusion  

### Architecture & Efficiency

*Showing the latest 50 out of 343 papers*

- **[The Past Frames the Future: Memory for Autoregressive Video Generation](https://arxiv.org/abs/2609.28466v1)**  
  Authors: Harold Haodong Chen, Rongjin Guo, Disen Lan, Wen-Jie Shu, Hongfei Zhang, Hanzhe Hu, Shengtao Yao, Zixin Zhang, Guibin Zhang, Zhefan Rao, Jinxiu Liu, Yexin Liu, Rui Peng, Yuhao Liu, Bin Ren, Shuai Yang, Yukang Chen, Salman Khan, Ying-Cong Chen, Ser-Nam Lim, Rynson W. H. Lau, Nicu Sebe, Yu Cheng, Ming-Hsuan Yang, Qifeng Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.28466v1.pdf)  
  Keywords: interactive, architecture, physical, autoregressive, dit, video generation, world model, evaluation  
- **[When Visual Quality Misleads: Intent Recognition under Rendered Avatar Distortions](https://arxiv.org/abs/2609.27560v1)**  
  Authors: Ning-Hsuan Chang, Kai-Siang Ma, Yu-Chih Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.27560v1.pdf)  
  Keywords: dit, avatar, streaming  
- **[Latent evolving World Action Model](https://arxiv.org/abs/2609.27455v1)**  
  Authors: Xueji Fang, Boqiang Duan, Hua Wu, Jingdong Wang, Guo-Jun Qi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.27455v1.pdf)  
  Keywords: architecture, diffusion model, dynamics, video generation, video diffusion, dit  
- **[HYDRO: Towards Non-Reversible Face De-Identification Using a High-Fidelity Hybrid Diffusion and Target-Oriented Approach](https://arxiv.org/abs/2609.27011v1)**  
  Authors: Felix Rosberg, Vitomir Štruc, Cristofer Englund, Eren Erdal Aksoy, Fernando Alonso-Fernandez  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.27011v1.pdf)  
  Keywords: identity, architecture  
- **[QuantWM: Temporally Consistent 2-Bit KV Cache Quantization for World Models and Video Generation](https://arxiv.org/abs/2609.26425v2)**  
  Authors: Jiaqi Zhao, Xiaobin Hu, Bo Yin, Junpeng Jiang, Miao Zhang, Shuicheng Yan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.26425v2.pdf)  
  Keywords: benchmark, temporal consistency, dit, video generation, world model, efficient  
- **[VideoX-Qwen: Data-Centric Instruction-Based Video Editing](https://arxiv.org/abs/2609.26015v1)**  
  Authors: JJiahang Li, Dingbao Shao, Xinyu Chen, Song Wu, Jiang Lin, Duo Li, Yuhang Liu, Jiaxin Hu, Shengrong Gu, Ying Tai, Zili Yi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.26015v1.pdf)  
  Keywords: dit, video editing, video generation  
- **[CogenPVG: Cognitive-Enhanced Reflective Multi-Agent Framework for Persuasive Video Generation](https://arxiv.org/abs/2609.25821v1)**  
  Authors: Yuntian Xiao, Shoulong Zhang, Wenfeng Song, Yan Wang, Yi Chen, Shuai Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.25821v1.pdf)  
  Keywords: dit, video generation  
- **[TRACE: Trajectory Representation and Consistency Estimation for AI-Generated Video Detection](https://arxiv.org/abs/2609.25775v1)**  
  Authors: Huangsen Cao, Hongkang chu, Siyao Yu, Xin Ding, Jianfeng Dong, Yongwei Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.25775v1.pdf)  
  Keywords: dit, trajectory, video generation, flow matching  
- **[mbariml: a curation pipeline for turning deep-sea imagery and video into object-detection training data](https://arxiv.org/abs/2609.25500v1)**  
  Authors: Lonny Lundsten, Kevin Barnard, Dave Caress  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.25500v1.pdf)  
  Keywords: dit, architecture  
- **[VideoGen-Agent: Reinforcing Video Generation Agents](https://arxiv.org/abs/2609.24997v1)**  
  Authors: Binxu Li, Haoyi Duan, Yuhui Zhang, Yaohui Zhang, Zihao Lin, Kaituo Feng, Suozhi Huang, Xiangyi Li, Yu Li, Chunyuan Li, Shilong Liu, Mengdi Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.24997v1.pdf)  
  Keywords: text-to-video, benchmark, identity, physical, video generation, dit  

### Audio & Multi-modal

- **[Dreaming the Sound of Contact: Leveraging Video and Audio Generation for Zero-Shot Force-Aware Manipulation and Data Generation](https://arxiv.org/abs/2609.19137v2)**  
  Authors: Guanhua Ji, Tianyu Li, Dayoon Suh, Yuqian Zhang, Boyan Zhang, Nadia Figueroa  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.19137v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://dreamingcontactsound.github.io)  
  Keywords: sound, video generation  
- **[LynnReal-Omni: Native multi-modal Video Generation for Agentic Visual Workflows](https://arxiv.org/abs/2609.15863v1)**  
  Authors: Xiaofeng Mao, Peijia Lin, Shaohao Rui, Yibo Zhang, Haibin Wan, Weijie Ma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.15863v1.pdf)  
  Keywords: text-to-video, efficient, controllable, streaming, diffusion model, multi-modal, diffusion transformer, acceleration, video generation, video diffusion, dit, evaluation, video restoration  
- **[Dynamic Learning Solutions: A System for Personalized Educational Video Generation](https://arxiv.org/abs/2609.14408v1)**  
  Authors: Siddhanth Sridhar, Shreya Chaurasia, Baddela Sai Yaswantha Reddy, Deepak Parmar, Shylaja S S  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.14408v1.pdf)  
  Keywords: interactive, education, multi-modal, style, video generation  
- **[AV-SafetyBench: A Safety Benchmark for Text-to-Audio-Video Generation](https://arxiv.org/abs/2609.06991v1)**  
  Authors: Suah Choi, Tae-Young Lee, Gyeong-Moon Park  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.06991v1.pdf)  
  Keywords: benchmark, sound, evaluation, video generation  
- **[MVWeaver: A Hierarchical Music Video Generation Agent with a Learned Song-to-Visual Bridge](https://arxiv.org/abs/2609.06478v1)**  
  Authors: Sifei Li, Minyan Luo, Xu Li, Guodong Qi, Xincan Wang, Hanwen Wang, Chen Zhang, Pengfei Wan, Oliver Deussen, Weiming Dong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.06478v1.pdf)  
  Keywords: architecture, concept, music video, long-form, video generation, dit  
- **[PRISM-Bench: An Audio-Centric Diagnostic Benchmark for Text-to-Audio-Video Generation](https://arxiv.org/abs/2609.04867v2)**  
  Authors: Yuchen Sun, Qian Yang, Jun Wang, Detai Xin, Guoqiao Yu, Guanglu Wan, Qi Jia  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.04867v2.pdf)  
  Keywords: benchmark, sound, evaluation, video generation  
- **[The Attention Triangle in Audio-Video Models](https://arxiv.org/abs/2609.03586v1)**  
  Authors: Sagi Polaczek, Noa Kraicer, Gal Metzer, Zhuo Ning, Ali Mahdavi-Amiri, Daniel Cohen-Or, Raja Giryes  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.03586v1.pdf)  
  Keywords: diffusion model, sound, dynamics, video generation, video diffusion, dit  
- **[Encore: Infinite Audio-Video Generation with Adaptive Signal Routing](https://arxiv.org/abs/2609.04249v1)**  
  Authors: Shaohua Pan, Junbao Chen, Shengyi He, Jingfeng Xue, Wen Tao, Haocheng Feng, Siming Fan, Dongwei Pan, Yi Yang, Wei He, Hang Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.04249v1.pdf) | [![GitHub](https://img.shields.io/github/stars/shaohua-pan/Encore?style=social)](https://github.com/shaohua-pan/Encore)  
  Keywords: denoising, long-form, audio-to-video, video generation, dit, evaluation  
- **[Surgical Video Generation From Diffusion to World Models: A Survey](https://arxiv.org/abs/2608.26214v1)**  
  Authors: Fuxiang Huang, Chenxu Zhang, Liang Han, Lei Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.26214v1.pdf)  
  Keywords: physical, concept, multi-modal, simulation, survey, dynamics, video generation, dit, world model  
- **[WeMM-Embedding: WeChat Multi-Modal Embedding Technical Report](https://arxiv.org/abs/2608.24053v1)**  
  Authors: Junjie Zhou, Ke Mei, Lei Li, Tianyi Wang, Fengyun Rao, Jing Lyu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.24053v1.pdf) | [![GitHub](https://img.shields.io/github/stars/Tencent/WeMM-Embedding?style=social)](https://github.com/Tencent/WeMM-Embedding)  
  Keywords: benchmark, evaluation, multi-modal  

### Controllable Generation

*Showing the latest 50 out of 115 papers*

- **[MotionSpec: Spectral Trajectory Supervision for Motion-Consistent Video Generation](https://arxiv.org/abs/2609.28095v1)**  
  Authors: Ziqi Ni, Rui Li, Shiqi Jiang, Wei Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.28095v1.pdf)  
  Keywords: text-to-video, trajectory, video generation  
- **[TRACE: Trajectory Representation and Consistency Estimation for AI-Generated Video Detection](https://arxiv.org/abs/2609.25775v1)**  
  Authors: Huangsen Cao, Hongkang chu, Siyao Yu, Xin Ding, Jianfeng Dong, Yongwei Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.25775v1.pdf)  
  Keywords: dit, trajectory, video generation, flow matching  
- **[Streaming Video Editing with Easy Adaptation](https://arxiv.org/abs/2609.24788v1)**  
  Authors: Yujia Hu, Jiajun Li, Zihao He, Songhua Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.24788v1.pdf) | [![GitHub](https://img.shields.io/github/stars/YujiaHu1109/SVEET?style=social)](https://github.com/YujiaHu1109/SVEET)  
  Keywords: controllable, video-to-video, streaming, architecture, diffusion model, acceleration, video generation, video diffusion, dit, video editing  
- **[CoaG: Cylinders on a Grid: Coarse 3D Layout Control for Video Generation](https://arxiv.org/abs/2609.24208v1)**  
  Authors: Zhangsihao Yang, Mengyi Shan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.24208v1.pdf)  
  Keywords: text-to-video, layout, video generation  
- **[Why Do Video Diffusion Models Violate Physics? Unveiling the Flaws in Attention Mechanisms](https://arxiv.org/abs/2609.23658v1)**  
  Authors: Yueyan Li, Haibo Wang, Caixia Yuan, Xiaojie Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.23658v1.pdf)  
  Keywords: text-to-video, physics, trajectory, physical, diffusion model, denoising, video diffusion  
- **[SparkDiffusion: Mitigating the High-Sparsity Trap --- A Unified Framework for up to $265\times$ Single-GPU Acceleration of Visual Generation](https://arxiv.org/abs/2609.23153v1)**  
  Authors: Yuxi Liu, Haoyu Li, Zekun Zhang, Tengxu Sun, Yixiang Cai, Jiayong Li, Yifei Xia, Tianle Liu, Baole Ai, Ang Wang, Jiamang Wang, Lin Qu, Kai Zhang, Kun Yuan, Bin Cui  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.23153v1.pdf)  
  Keywords: trajectory, architecture, distillation, diffusion transformer, t2v, acceleration, i2v, video diffusion  
- **[Edit-VAR: Taming Visual Autoregressive Model for Precise Video Editing](https://arxiv.org/abs/2609.21268v1)**  
  Authors: Chongbo Zhao, Jiangming Wang, Xilai Wang, Xinyu Wang, Jingyi Tang, Chunjie Hao, Pengjie Song, Yue Ma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.21268v1.pdf)  
  Keywords: autoregressive, dit, video editing, trajectory  
- **[DART: Distillation-Aware Reparameterization for Training-Free LoRA Reuse in Few-Step Video Diffusion Models](https://arxiv.org/abs/2609.20051v1)**  
  Authors: Shihong Li, Juntao Xu, JinCao, Maowen Tang, Jun Huang, Jintao Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.20051v1.pdf)  
  Keywords: trajectory, diffusion model, distillation, denoising, video generation, video diffusion, dit, evaluation  
- **[Astronex-World 1.0: Real-Time Interactive World Model Foundation](https://arxiv.org/abs/2609.20034v1)**  
  Authors: Xin Zhou, Cong Miao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.20034v1.pdf)  
  Keywords: text-to-video, controllable, image-to-video, interactive, autonomous driving, dynamics, i2v, world model  
- **[PhysStream: Streaming Physics-Grounded Video Generation with Structured Scene Memory and Fine-Grained Motion Control](https://arxiv.org/abs/2609.17521v2)**  
  Authors: Chuhao Chen, Peter Wonka, Chaoyang Wang, Chen Wang, Qiao Feng, Sergey Tulyakov, Lingjie Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.17521v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://czzzzh.github.io/PhysStream)  
  Keywords: benchmark, physics, controllable, video synthesis, image-to-video, trajectory, streaming, interactive, autoregressive, physical, dynamics, video generation, dit, motion control  

### Human & Character Animation

- **[All modalities are equal, but video is more equal: Closing the Cross-Attention Gap in Joint Video Generation](https://arxiv.org/abs/2609.27901v1)**  
  Authors: Ohad Rahamim, Dvir Samuel, Idan Schwartz, Gal Chechik  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.27901v1.pdf)  
  Keywords: physical, diffusion transformer, video generation, body motion  
- **[When Visual Quality Misleads: Intent Recognition under Rendered Avatar Distortions](https://arxiv.org/abs/2609.27560v1)**  
  Authors: Ning-Hsuan Chang, Kai-Siang Ma, Yu-Chih Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.27560v1.pdf)  
  Keywords: dit, avatar, streaming  
- **[Vidu S2: Real-Time Interactive, Editable, and Spatial Video Generation](https://arxiv.org/abs/2609.11638v1)**  
  Authors: Jintao Zhang, Kai Jiang, Jintao Chen, Xu Wang, Deyuan Liu, Jungang Li, Dechuang Chen, Ming Lin, Jingjiang Zhou, Haopeng Jin, Qi Jia, Xiaohang Wang, Yaole Wang, Zhanqiang Zhang, Ran Li, Zhengkun Huang, Shuyue Xiong, Yuji Wang, Zikun Dai, Hui He, Yang Luo, Mang Ning, Weiqi Feng, Chengyang Ye, Xinyue Lin, Min Zhao, Hongzhou Zhu, Hengkai Tan, Zeyuan Wang, Chendong Xiang, Kaiwen Zheng, Zhijie Deng, Fan Bao, Jianfei Chen, Jun Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.11638v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://vidu.com/vidu-stream)  
  Keywords: interactive, style, video generation, dit, avatar, video editing  
- **[Decoupled Self-Forcing Distillation for Streaming Talking Head Generation](https://arxiv.org/abs/2609.10317v1)**  
  Authors: Yanru An, Ruiyan Wang, Wenwu Wei, Rui Bu, Qi Wang, Hongwei Hu, Zhengxue Cheng, Rong Xie, Li Song, Wenjun Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.10317v1.pdf)  
  Keywords: identity, streaming, autoregressive, diffusion model, distillation, talking head, video diffusion, dit  
- **[BooM-VVT: Boosting Mask-Free Video Virtual Try-On with Image-Level Pseudo Data](https://arxiv.org/abs/2609.04120v1)**  
  Authors: Wei Zhang, Xin Li, Peishu Shi, Jialin Gao, Xuekang Peng, Zhichao Lian, Yeying Jin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.04120v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://boomvvt.github.io/boomvvt)  
  Keywords: virtual try-on, temporal consistency, video generation  
- **[AvatarDynamizer: From Static to Dynamic Human Avatars via Generative Dynamic Textures](https://arxiv.org/abs/2608.19900v1)**  
  Authors: Guoxing Sun, Heming Zhu, Linjie Lyu, Pascal Fua, Christian Theobalt, Marc Habermann  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.19900v1.pdf)  
  Keywords: controllable, diffusion model, dynamics, video diffusion, dit, avatar  
- **[CL4D: Contrastive Language-4D Pretraining for Vision-Language Reasoning in Dynamic Scenes](https://arxiv.org/abs/2608.18734v2)**  
  Authors: Kumal Hewagamage, Isuranga Senavirathne, Sasika Amarasinghe, Hasitha Gallella, Dulanga Weerakoon, Vigneshwaran Subbaraju, Ranga Rodrigo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.18734v2.pdf)  
  Keywords: benchmark, physical, human motion, dynamics, dit  
- **[SingDance: Compositional Zero-Shot Singing-and-Dancing Video Generation with Role-Aware Audio Conditioning](https://arxiv.org/abs/2608.16220v1)**  
  Authors: Tao Feng, Xu Li, Xiangyang Luo, Ming Wen, Huadai Liu, Chen Zhang, Wei Xue  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.16220v1.pdf)  
  Keywords: controllable, body motion, video generation, video diffusion, dit, speech-driven  
- **[FlowDance: Music-Driven Dance Video Generation with Parallel Pose and RGB Streams](https://arxiv.org/abs/2608.15818v1)**  
  Authors: Genying Li, Boda Lin, Jiachen Li, Zijian Jia, Haojie Zheng, Yiming Wang, Shuchen Weng, Si Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.15818v1.pdf)  
  Keywords: identity, video synthesis, long video, denoising, body motion, human animation, video generation  
- **[Avatar-Forever: Decoupled Parallel Training for High-Quality Real-Time Infinite Avatars](https://arxiv.org/abs/2608.12107v1)**  
  Authors: Ruibin Li, Tao Yang, Zhiyuan Ma, Fangzhou Ai, Shilei Wen, Lei Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.12107v1.pdf)  
  Keywords: identity, streaming, interactive, autoregressive, distillation, audio-driven, video generation, dit, avatar, efficient  

### Image-to-Video Generation

- **[SparkDiffusion: Mitigating the High-Sparsity Trap --- A Unified Framework for up to $265\times$ Single-GPU Acceleration of Visual Generation](https://arxiv.org/abs/2609.23153v1)**  
  Authors: Yuxi Liu, Haoyu Li, Zekun Zhang, Tengxu Sun, Yixiang Cai, Jiayong Li, Yifei Xia, Tianle Liu, Baole Ai, Ang Wang, Jiamang Wang, Lin Qu, Kai Zhang, Kun Yuan, Bin Cui  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.23153v1.pdf)  
  Keywords: trajectory, architecture, distillation, diffusion transformer, t2v, acceleration, i2v, video diffusion  
- **[Astronex-World 1.0: Real-Time Interactive World Model Foundation](https://arxiv.org/abs/2609.20034v1)**  
  Authors: Xin Zhou, Cong Miao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.20034v1.pdf)  
  Keywords: text-to-video, controllable, image-to-video, interactive, autonomous driving, dynamics, i2v, world model  
- **[StrucPhysVideo: Learning Physical Dynamics from Structured Captions and Robot Actions](https://arxiv.org/abs/2609.18430v1)**  
  Authors: Awomo-WM Team, :, Enhui Ma, Kaiwen Guo, Tingrui Zhang, Wei Song, Yingshui Tan, Jianhua Xu, Tong Zhang, Kaicheng Yu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.18430v1.pdf)  
  Keywords: physics, image-to-video, interactive, physical, autoregressive, action-conditioned, distillation, dit, denoising, dynamics, i2v, video prediction, world model  
- **[PhysStream: Streaming Physics-Grounded Video Generation with Structured Scene Memory and Fine-Grained Motion Control](https://arxiv.org/abs/2609.17521v2)**  
  Authors: Chuhao Chen, Peter Wonka, Chaoyang Wang, Chen Wang, Qiao Feng, Sergey Tulyakov, Lingjie Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.17521v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://czzzzh.github.io/PhysStream)  
  Keywords: benchmark, physics, controllable, video synthesis, image-to-video, trajectory, streaming, interactive, autoregressive, physical, dynamics, video generation, dit, motion control  
- **[CrossDistill: Balancing Quality and Diversity via Trajectory-Level Hybrid Few-Step Distillation](https://arxiv.org/abs/2609.14725v2)**  
  Authors: Yuxi Liu, Haoyu Li, Yixiang Cai, Tengxu Sun, Zekun Zhang, Baole Ai, Ang Wang, Jiamang Wang, Lin Qu, Kun Yuan, Kai Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.14725v2.pdf)  
  Keywords: text-to-video, image-to-video, trajectory, diffusion model, distillation, video diffusion  
- **[DF26: We Cannot Tell Fake From Real Anymore](https://arxiv.org/abs/2609.07369v1)**  
  Authors: Severyn Shykula, Andrii Yermakov, Ivan Samarskyi, Dmytro Mishkin, Jan Cech, Anastasiia Mishchuk  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.07369v1.pdf)  
  Keywords: text-to-video, benchmark, evaluation, image-to-video  
- **[The Price of Consistency: Exploiting Visual Anchors for Multimodal Jailbreaking in Video Generation](https://arxiv.org/abs/2609.07216v1)**  
  Authors: Peng Li, Qianqian Xu, Yangbangyan Jiang, Zhipeng Yu, Qingming Huang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.07216v1.pdf)  
  Keywords: benchmark, controllable, temporal consistency, i2v, video generation, dit  
- **[PhysWeep: Does a Video Generator Realize the Physics You Ask For?](https://arxiv.org/abs/2609.06207v1)**  
  Authors: Rasul Khanbayov, Hasan Kurban  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.06207v1.pdf)  
  Keywords: benchmark, physics, image-to-video, physical, dit, dynamics, world model  
- **[TempJail: Temporal Jailbreak Attacks against Image-to-Video Generation Models](https://arxiv.org/abs/2608.26971v2)**  
  Authors: Qi Lu, Zehui Guo, David Yuanda Gan, Zijing Li, Hengda Zhang, Weijun Xu, Qiankun Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.26971v2.pdf) | [![GitHub](https://img.shields.io/github/stars/luqi-glory/TempJail?style=social)](https://github.com/luqi-glory/TempJail)  
  Keywords: video synthesis, image-to-video, i2v, video generation, dit, evaluation  
- **[Direct, Parallel, or Sequential? A Comparative Study of Training-Free Multi-Subject Image-to-Video Generation](https://arxiv.org/abs/2608.22819v1)**  
  Authors: Yanliang Qi, Kexi Chen, Muchao Ye, Haomiao Ni  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.22819v1.pdf)  
  Keywords: controllable, image-to-video, temporal consistency, i2v, video generation, dit  

### Long Video Generation

*Showing the latest 50 out of 121 papers*

- **[The Past Frames the Future: Memory for Autoregressive Video Generation](https://arxiv.org/abs/2609.28466v1)**  
  Authors: Harold Haodong Chen, Rongjin Guo, Disen Lan, Wen-Jie Shu, Hongfei Zhang, Hanzhe Hu, Shengtao Yao, Zixin Zhang, Guibin Zhang, Zhefan Rao, Jinxiu Liu, Yexin Liu, Rui Peng, Yuhao Liu, Bin Ren, Shuai Yang, Yukang Chen, Salman Khan, Ying-Cong Chen, Ser-Nam Lim, Rynson W. H. Lau, Nicu Sebe, Yu Cheng, Ming-Hsuan Yang, Qifeng Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.28466v1.pdf)  
  Keywords: interactive, architecture, physical, autoregressive, dit, video generation, world model, evaluation  
- **[When Visual Quality Misleads: Intent Recognition under Rendered Avatar Distortions](https://arxiv.org/abs/2609.27560v1)**  
  Authors: Ning-Hsuan Chang, Kai-Siang Ma, Yu-Chih Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.27560v1.pdf)  
  Keywords: dit, avatar, streaming  
- **[QuantWM: Temporally Consistent 2-Bit KV Cache Quantization for World Models and Video Generation](https://arxiv.org/abs/2609.26425v2)**  
  Authors: Jiaqi Zhao, Xiaobin Hu, Bo Yin, Junpeng Jiang, Miao Zhang, Shuicheng Yan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.26425v2.pdf)  
  Keywords: benchmark, temporal consistency, dit, video generation, world model, efficient  
- **[WorldCrafter: Consistent Video World Model with Implicit 3D-aware Memory](https://arxiv.org/abs/2609.24984v1)**  
  Authors: Wangbo Yu, Kunhao Liu, Wenbo Hu, Shenghai Yuan, Chaoran Feng, Haiyang Zhou, Yukun Huang, Yiran Wang, Wang Zhao, Yingmin Luo, Ying Shan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.24984v1.pdf)  
  Keywords: streaming, interactive, 3d-aware, distillation, dit, denoising, world model  
- **[Streaming Video Editing with Easy Adaptation](https://arxiv.org/abs/2609.24788v1)**  
  Authors: Yujia Hu, Jiajun Li, Zihao He, Songhua Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.24788v1.pdf) | [![GitHub](https://img.shields.io/github/stars/YujiaHu1109/SVEET?style=social)](https://github.com/YujiaHu1109/SVEET)  
  Keywords: controllable, video-to-video, streaming, architecture, diffusion model, acceleration, video generation, video diffusion, dit, video editing  
- **[Edit-VAR: Taming Visual Autoregressive Model for Precise Video Editing](https://arxiv.org/abs/2609.21268v1)**  
  Authors: Chongbo Zhao, Jiangming Wang, Xilai Wang, Xinyu Wang, Jingyi Tang, Chunjie Hao, Pengjie Song, Yue Ma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.21268v1.pdf)  
  Keywords: autoregressive, dit, video editing, trajectory  
- **[Recency Forcing: Bridging the Long-Horizon Gap in Autoregressive Video Generation](https://arxiv.org/abs/2609.19729v1)**  
  Authors: Tri Cao, Hung Nguyen, Phong Nguyen, Khoi Nguyen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.19729v1.pdf)  
  Keywords: autoregressive, dit, video generation, denoising  
- **[StrucPhysVideo: Learning Physical Dynamics from Structured Captions and Robot Actions](https://arxiv.org/abs/2609.18430v1)**  
  Authors: Awomo-WM Team, :, Enhui Ma, Kaiwen Guo, Tingrui Zhang, Wei Song, Yingshui Tan, Jianhua Xu, Tong Zhang, Kaicheng Yu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.18430v1.pdf)  
  Keywords: physics, image-to-video, interactive, physical, autoregressive, action-conditioned, distillation, dit, denoising, dynamics, i2v, video prediction, world model  
- **[PhysStream: Streaming Physics-Grounded Video Generation with Structured Scene Memory and Fine-Grained Motion Control](https://arxiv.org/abs/2609.17521v2)**  
  Authors: Chuhao Chen, Peter Wonka, Chaoyang Wang, Chen Wang, Qiao Feng, Sergey Tulyakov, Lingjie Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.17521v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://czzzzh.github.io/PhysStream)  
  Keywords: benchmark, physics, controllable, video synthesis, image-to-video, trajectory, streaming, interactive, autoregressive, physical, dynamics, video generation, dit, motion control  
- **[SlotDiT: Object-Centric Representations for Diffusion Transformers](https://arxiv.org/abs/2609.17414v1)**  
  Authors: Gjergj Plepi, Sven Behnke  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.17414v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://slot-dit.github.io)  
  Keywords: autoregressive, diffusion model, diffusion transformer, dynamics, video generation, dit, efficient  

### Personalization & Customization

*Showing the latest 50 out of 82 papers*

- **[HYDRO: Towards Non-Reversible Face De-Identification Using a High-Fidelity Hybrid Diffusion and Target-Oriented Approach](https://arxiv.org/abs/2609.27011v1)**  
  Authors: Felix Rosberg, Vitomir Štruc, Cristofer Englund, Eren Erdal Aksoy, Fernando Alonso-Fernandez  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.27011v1.pdf)  
  Keywords: identity, architecture  
- **[Code Plans, Diffusion Renders: Open-Ended Generative World Modeling](https://arxiv.org/abs/2609.26458v1)**  
  Authors: Zixun Fang, Yawen Shao, Kai Zhu, Jie Xiao, Shihan Chen, Yu Liu, Xueyang Fu, Yang Cao, Wei Zhai, Zheng-Jun Zha  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.26458v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://becauseimbatman0.github.io/CoDeR)  
  Keywords: concept, dynamics, video generation, world model, evaluation  
- **[VideoGen-Agent: Reinforcing Video Generation Agents](https://arxiv.org/abs/2609.24997v1)**  
  Authors: Binxu Li, Haoyi Duan, Yuhui Zhang, Yaohui Zhang, Zihao Lin, Kaituo Feng, Suozhi Huang, Xiangyi Li, Yu Li, Chunyuan Li, Shilong Liu, Mengdi Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.24997v1.pdf)  
  Keywords: text-to-video, benchmark, identity, physical, video generation, dit  
- **[Generative Tutorial: Towards Live Contextualized Visual Instructions for Physical Tasks](https://arxiv.org/abs/2609.24955v1)**  
  Authors: Muzhe Wu, Zuchen Li, Xu Wang, Anhong Guo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.24955v1.pdf)  
  Keywords: concept, evaluation, physical, video generation  
- **[OmniVBench: A Benchmark and Large-Scale Dataset for Omni Reference-to-Video Generation](https://arxiv.org/abs/2609.22069v1)**  
  Authors: Wenxue Li, Peiyan Guan, Haoyang Jiang, Junxian Cai, Hualuo Liu, Chunjie Zhang, Chong Guan, Kai Huang, Songlian Li, Taiyi Wu, Yongjian Yu, Xiaotong Zhao, Alan Zhao, Eric Liu, Xi Chen, Yu Liu, Lei Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.22069v1.pdf)  
  Keywords: benchmark, evaluation, style, video generation  
- **[OmniVChat: Synthesizing, Benchmarking, and Training for Native Audio-Visual Dialogue](https://arxiv.org/abs/2609.21465v1)**  
  Authors: Haolin He, Yunfei Chu, Qi Chen, Wen Huang, Yuan Feng, Muzhi Zhu, Zheqi Dai, Haoning Xu, Dongchao Yang, Chunyat Wu, Zining Liang, Zhengxi Liu, Xiquan Li, Xie Chen, Xize Cheng, Qize Yang, Jin Xu, Qiuqiang Kong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.21465v1.pdf)  
  Keywords: benchmark, evaluation, style, video generation  
- **[Dynamic Learning Solutions: A System for Personalized Educational Video Generation](https://arxiv.org/abs/2609.14408v1)**  
  Authors: Siddhanth Sridhar, Shreya Chaurasia, Baddela Sai Yaswantha Reddy, Deepak Parmar, Shylaja S S  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.14408v1.pdf)  
  Keywords: interactive, education, multi-modal, style, video generation  
- **[SignMimic: Robust High-Quality Sign Language Motion Generation via Human-Shape-Oblivious Pose Transfer Guidance](https://arxiv.org/abs/2609.14122v1)**  
  Authors: Zhewen He, Junyi Yu, Haomian Huang, Zhenhua Li, Yi Fang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.14122v1.pdf)  
  Keywords: identity, temporal consistency, style, video diffusion, dit  
- **[Vidu S2: Real-Time Interactive, Editable, and Spatial Video Generation](https://arxiv.org/abs/2609.11638v1)**  
  Authors: Jintao Zhang, Kai Jiang, Jintao Chen, Xu Wang, Deyuan Liu, Jungang Li, Dechuang Chen, Ming Lin, Jingjiang Zhou, Haopeng Jin, Qi Jia, Xiaohang Wang, Yaole Wang, Zhanqiang Zhang, Ran Li, Zhengkun Huang, Shuyue Xiong, Yuji Wang, Zikun Dai, Hui He, Yang Luo, Mang Ning, Weiqi Feng, Chengyang Ye, Xinyue Lin, Min Zhao, Hongzhou Zhu, Hengkai Tan, Zeyuan Wang, Chendong Xiang, Kaiwen Zheng, Zhijie Deng, Fan Bao, Jianfei Chen, Jun Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.11638v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://vidu.com/vidu-stream)  
  Keywords: interactive, style, video generation, dit, avatar, video editing  
- **[Harnessing Intrinsic Subject-Aware Attention for Controllable Multi-Subject Video Generation](https://arxiv.org/abs/2609.11507v1)**  
  Authors: Niange Yu, Ye Tian, Biaolong Chen, Miao Lu, Aixi Zhang, Hao Jiang, Yunhai Tong, Pipei Huang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.11507v1.pdf)  
  Keywords: benchmark, identity, controllable, diffusion transformer, video generation, dit  

### Physical Understanding

*Showing the latest 50 out of 138 papers*

- **[The Past Frames the Future: Memory for Autoregressive Video Generation](https://arxiv.org/abs/2609.28466v1)**  
  Authors: Harold Haodong Chen, Rongjin Guo, Disen Lan, Wen-Jie Shu, Hongfei Zhang, Hanzhe Hu, Shengtao Yao, Zixin Zhang, Guibin Zhang, Zhefan Rao, Jinxiu Liu, Yexin Liu, Rui Peng, Yuhao Liu, Bin Ren, Shuai Yang, Yukang Chen, Salman Khan, Ying-Cong Chen, Ser-Nam Lim, Rynson W. H. Lau, Nicu Sebe, Yu Cheng, Ming-Hsuan Yang, Qifeng Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.28466v1.pdf)  
  Keywords: interactive, architecture, physical, autoregressive, dit, video generation, world model, evaluation  
- **[All modalities are equal, but video is more equal: Closing the Cross-Attention Gap in Joint Video Generation](https://arxiv.org/abs/2609.27901v1)**  
  Authors: Ohad Rahamim, Dvir Samuel, Idan Schwartz, Gal Chechik  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.27901v1.pdf)  
  Keywords: physical, diffusion transformer, video generation, body motion  
- **[Latent evolving World Action Model](https://arxiv.org/abs/2609.27455v1)**  
  Authors: Xueji Fang, Boqiang Duan, Hua Wu, Jingdong Wang, Guo-Jun Qi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.27455v1.pdf)  
  Keywords: architecture, diffusion model, dynamics, video generation, video diffusion, dit  
- **[Code Plans, Diffusion Renders: Open-Ended Generative World Modeling](https://arxiv.org/abs/2609.26458v1)**  
  Authors: Zixun Fang, Yawen Shao, Kai Zhu, Jie Xiao, Shihan Chen, Yu Liu, Xueyang Fu, Yang Cao, Wei Zhai, Zheng-Jun Zha  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.26458v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://becauseimbatman0.github.io/CoDeR)  
  Keywords: concept, dynamics, video generation, world model, evaluation  
- **[VideoGen-Agent: Reinforcing Video Generation Agents](https://arxiv.org/abs/2609.24997v1)**  
  Authors: Binxu Li, Haoyi Duan, Yuhui Zhang, Yaohui Zhang, Zihao Lin, Kaituo Feng, Suozhi Huang, Xiangyi Li, Yu Li, Chunyuan Li, Shilong Liu, Mengdi Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.24997v1.pdf)  
  Keywords: text-to-video, benchmark, identity, physical, video generation, dit  
- **[DexTacWAM: A Visuo-Tactile World-Action Model for Dexterous Manipulation](https://arxiv.org/abs/2609.24976v1)**  
  Authors: Haoran Yuan, Zekai Wang, Boning Shao, Haoran Lu, Trevor Darrell, Ismini Lourentzou, Wei Zhan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.24976v1.pdf)  
  Keywords: dit, dynamics, video diffusion, world model, efficient  
- **[Generative Tutorial: Towards Live Contextualized Visual Instructions for Physical Tasks](https://arxiv.org/abs/2609.24955v1)**  
  Authors: Muzhe Wu, Zuchen Li, Xu Wang, Anhong Guo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.24955v1.pdf)  
  Keywords: concept, evaluation, physical, video generation  
- **[UniK: Universal Knowledge Perception for Digital and Physical AI](https://arxiv.org/abs/2609.23971v1)**  
  Authors: Nirmit Desai, Kunal Sawarkar, Aditya Mahakali, Dongkon Lee, Kevin Park, Eric Song  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.23971v1.pdf)  
  Keywords: physical, world model, evaluation, efficient, medical  
- **[Why Do Video Diffusion Models Violate Physics? Unveiling the Flaws in Attention Mechanisms](https://arxiv.org/abs/2609.23658v1)**  
  Authors: Yueyan Li, Haibo Wang, Caixia Yuan, Xiaojie Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.23658v1.pdf)  
  Keywords: text-to-video, physics, trajectory, physical, diffusion model, denoising, video diffusion  
- **[Detecting Phone-Induced Pedestrian Distraction via a Multimodal Fusion Transformer](https://arxiv.org/abs/2609.23507v1)**  
  Authors: Yuanzhe Li, Hounian Liu, Xiaotong Chang, Yidi Huang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.23507v1.pdf)  
  Keywords: dynamics  

### Surveys & Benchmarks

*Showing the latest 50 out of 230 papers*

- **[The Past Frames the Future: Memory for Autoregressive Video Generation](https://arxiv.org/abs/2609.28466v1)**  
  Authors: Harold Haodong Chen, Rongjin Guo, Disen Lan, Wen-Jie Shu, Hongfei Zhang, Hanzhe Hu, Shengtao Yao, Zixin Zhang, Guibin Zhang, Zhefan Rao, Jinxiu Liu, Yexin Liu, Rui Peng, Yuhao Liu, Bin Ren, Shuai Yang, Yukang Chen, Salman Khan, Ying-Cong Chen, Ser-Nam Lim, Rynson W. H. Lau, Nicu Sebe, Yu Cheng, Ming-Hsuan Yang, Qifeng Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.28466v1.pdf)  
  Keywords: interactive, architecture, physical, autoregressive, dit, video generation, world model, evaluation  
- **[LAYERSCOPE: A Layerwise Characterization of Video and Multimodal Learned Representations](https://arxiv.org/abs/2609.28086v1)**  
  Authors: Sandra Arcos-Holzinger, Debashish Chakraborty, Rohita Mocharla, Will Walden, Andrew Yates, Reno Kriz, Sarah M. Erfani, James Bailey, Vishal M. Patel, Sanjeev Khudanpur  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.28086v1.pdf)  
  Keywords: text-to-video, evaluation  
- **[Code Plans, Diffusion Renders: Open-Ended Generative World Modeling](https://arxiv.org/abs/2609.26458v1)**  
  Authors: Zixun Fang, Yawen Shao, Kai Zhu, Jie Xiao, Shihan Chen, Yu Liu, Xueyang Fu, Yang Cao, Wei Zhai, Zheng-Jun Zha  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.26458v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://becauseimbatman0.github.io/CoDeR)  
  Keywords: concept, dynamics, video generation, world model, evaluation  
- **[QuantWM: Temporally Consistent 2-Bit KV Cache Quantization for World Models and Video Generation](https://arxiv.org/abs/2609.26425v2)**  
  Authors: Jiaqi Zhao, Xiaobin Hu, Bo Yin, Junpeng Jiang, Miao Zhang, Shuicheng Yan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.26425v2.pdf)  
  Keywords: benchmark, temporal consistency, dit, video generation, world model, efficient  
- **[VideoGen-Agent: Reinforcing Video Generation Agents](https://arxiv.org/abs/2609.24997v1)**  
  Authors: Binxu Li, Haoyi Duan, Yuhui Zhang, Yaohui Zhang, Zihao Lin, Kaituo Feng, Suozhi Huang, Xiangyi Li, Yu Li, Chunyuan Li, Shilong Liu, Mengdi Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.24997v1.pdf)  
  Keywords: text-to-video, benchmark, identity, physical, video generation, dit  
- **[Generative Tutorial: Towards Live Contextualized Visual Instructions for Physical Tasks](https://arxiv.org/abs/2609.24955v1)**  
  Authors: Muzhe Wu, Zuchen Li, Xu Wang, Anhong Guo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.24955v1.pdf)  
  Keywords: concept, evaluation, physical, video generation  
- **[Ovis-Embedding: Pushing the Frontiers of Universal Omni-Modal Embeddings](https://arxiv.org/abs/2609.25165v1)**  
  Authors: Ovis-Embedding Team  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.25165v1.pdf)  
  Keywords: distillation, evaluation  
- **[UniK: Universal Knowledge Perception for Digital and Physical AI](https://arxiv.org/abs/2609.23971v1)**  
  Authors: Nirmit Desai, Kunal Sawarkar, Aditya Mahakali, Dongkon Lee, Kevin Park, Eric Song  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.23971v1.pdf)  
  Keywords: physical, world model, evaluation, efficient, medical  
- **[RewardVerse: Rubric-Guided Policy Optimization for Video Reward Modeling](https://arxiv.org/abs/2609.22947v2)**  
  Authors: Zhenchen Tang, Yang Li, Songlin Yang, Bo Peng, Xiaotong Zhao, Shuai Li, Haotian Fan, Alan Zhao, Jing Dong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.22947v2.pdf)  
  Keywords: benchmark, evaluation, efficient, video generation  
- **[OmniVBench: A Benchmark and Large-Scale Dataset for Omni Reference-to-Video Generation](https://arxiv.org/abs/2609.22069v1)**  
  Authors: Wenxue Li, Peiyan Guan, Haoyang Jiang, Junxian Cai, Hualuo Liu, Chunjie Zhang, Chong Guan, Kai Huang, Songlian Li, Taiyi Wu, Yongjian Yu, Xiaotong Zhao, Alan Zhao, Eric Liu, Xi Chen, Yu Liu, Lei Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.22069v1.pdf)  
  Keywords: benchmark, evaluation, style, video generation  

### Text-to-Video Generation

*Showing the latest 50 out of 72 papers*

- **[MotionSpec: Spectral Trajectory Supervision for Motion-Consistent Video Generation](https://arxiv.org/abs/2609.28095v1)**  
  Authors: Ziqi Ni, Rui Li, Shiqi Jiang, Wei Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.28095v1.pdf)  
  Keywords: text-to-video, trajectory, video generation  
- **[LAYERSCOPE: A Layerwise Characterization of Video and Multimodal Learned Representations](https://arxiv.org/abs/2609.28086v1)**  
  Authors: Sandra Arcos-Holzinger, Debashish Chakraborty, Rohita Mocharla, Will Walden, Andrew Yates, Reno Kriz, Sarah M. Erfani, James Bailey, Vishal M. Patel, Sanjeev Khudanpur  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.28086v1.pdf)  
  Keywords: text-to-video, evaluation  
- **[VideoGen-Agent: Reinforcing Video Generation Agents](https://arxiv.org/abs/2609.24997v1)**  
  Authors: Binxu Li, Haoyi Duan, Yuhui Zhang, Yaohui Zhang, Zihao Lin, Kaituo Feng, Suozhi Huang, Xiangyi Li, Yu Li, Chunyuan Li, Shilong Liu, Mengdi Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.24997v1.pdf)  
  Keywords: text-to-video, benchmark, identity, physical, video generation, dit  
- **[CoaG: Cylinders on a Grid: Coarse 3D Layout Control for Video Generation](https://arxiv.org/abs/2609.24208v1)**  
  Authors: Zhangsihao Yang, Mengyi Shan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.24208v1.pdf)  
  Keywords: text-to-video, layout, video generation  
- **[Why Do Video Diffusion Models Violate Physics? Unveiling the Flaws in Attention Mechanisms](https://arxiv.org/abs/2609.23658v1)**  
  Authors: Yueyan Li, Haibo Wang, Caixia Yuan, Xiaojie Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.23658v1.pdf)  
  Keywords: text-to-video, physics, trajectory, physical, diffusion model, denoising, video diffusion  
- **[SparkDiffusion: Mitigating the High-Sparsity Trap --- A Unified Framework for up to $265\times$ Single-GPU Acceleration of Visual Generation](https://arxiv.org/abs/2609.23153v1)**  
  Authors: Yuxi Liu, Haoyu Li, Zekun Zhang, Tengxu Sun, Yixiang Cai, Jiayong Li, Yifei Xia, Tianle Liu, Baole Ai, Ang Wang, Jiamang Wang, Lin Qu, Kai Zhang, Kun Yuan, Bin Cui  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.23153v1.pdf)  
  Keywords: trajectory, architecture, distillation, diffusion transformer, t2v, acceleration, i2v, video diffusion  
- **[CompAdapt: Adaptable Composite Motion Modeling for Physics-Consistent Text-to-Video Generation](https://arxiv.org/abs/2609.21455v2)**  
  Authors: Haoran Qin, Renlong Wu, Tianyu Huang, Yukang Ding, Hui Li, Wangmeng Zuo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.21455v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://makapic.github.io/CompAdapt)  
  Keywords: text-to-video, benchmark, physics, physical, t2v, dynamics, video generation, dit, physics-aware  
- **[Astronex-World 1.0: Real-Time Interactive World Model Foundation](https://arxiv.org/abs/2609.20034v1)**  
  Authors: Xin Zhou, Cong Miao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.20034v1.pdf)  
  Keywords: text-to-video, controllable, image-to-video, interactive, autonomous driving, dynamics, i2v, world model  
- **[LynnReal-Omni: Native multi-modal Video Generation for Agentic Visual Workflows](https://arxiv.org/abs/2609.15863v1)**  
  Authors: Xiaofeng Mao, Peijia Lin, Shaohao Rui, Yibo Zhang, Haibin Wan, Weijie Ma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.15863v1.pdf)  
  Keywords: text-to-video, efficient, controllable, streaming, diffusion model, multi-modal, diffusion transformer, acceleration, video generation, video diffusion, dit, evaluation, video restoration  
- **[Query-Conditioned Spherical Centroid Aggregation for Multimodal Retrieval](https://arxiv.org/abs/2609.15335v1)**  
  Authors: Ambuj Mehrish, Anindya Nag, Sebastiano Vascon  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.15335v1.pdf)  
  Keywords: text-to-video, dit, benchmark, evaluation  

### Video Editing

- **[VideoX-Qwen: Data-Centric Instruction-Based Video Editing](https://arxiv.org/abs/2609.26015v1)**  
  Authors: JJiahang Li, Dingbao Shao, Xinyu Chen, Song Wu, Jiang Lin, Duo Li, Yuhang Liu, Jiaxin Hu, Shengrong Gu, Ying Tai, Zili Yi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.26015v1.pdf)  
  Keywords: dit, video editing, video generation  
- **[Streaming Video Editing with Easy Adaptation](https://arxiv.org/abs/2609.24788v1)**  
  Authors: Yujia Hu, Jiajun Li, Zihao He, Songhua Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.24788v1.pdf) | [![GitHub](https://img.shields.io/github/stars/YujiaHu1109/SVEET?style=social)](https://github.com/YujiaHu1109/SVEET)  
  Keywords: controllable, video-to-video, streaming, architecture, diffusion model, acceleration, video generation, video diffusion, dit, video editing  
- **[Edit-VAR: Taming Visual Autoregressive Model for Precise Video Editing](https://arxiv.org/abs/2609.21268v1)**  
  Authors: Chongbo Zhao, Jiangming Wang, Xilai Wang, Xinyu Wang, Jingyi Tang, Chunjie Hao, Pengjie Song, Yue Ma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.21268v1.pdf)  
  Keywords: autoregressive, dit, video editing, trajectory  
- **[Video DeltaNet: A Video-Native Hybrid Attention for Livestream Video Generation](https://arxiv.org/abs/2609.20744v2)**  
  Authors: Haocheng Xi, Yiming Xie, Hexu Zhao, Yiwen Zhang, Michael Liu, Thomas Creavin, Kurt Keutzer, Xiuyu Li, Zhaoyang Lv, Chenfeng Xu, Haiwen Feng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.20744v2.pdf) | [![GitHub](https://img.shields.io/github/stars/OpenVDN/vdn-minimax-h3?style=social)](https://github.com/OpenVDN/vdn-minimax-h3) | [![Project](https://img.shields.io/badge/-Project-blue)](https://huggingface.co/OpenVDN/vdn-minimax-h3) | [![HuggingFace](https://img.shields.io/badge/-HuggingFace-yellow)](https://huggingface.co/OpenVDN/vdn-minimax-h3)  
  Keywords: video-to-video, diffusion model, distillation, denoising, video generation, video diffusion, dit  
- **[Vidu S2: Real-Time Interactive, Editable, and Spatial Video Generation](https://arxiv.org/abs/2609.11638v1)**  
  Authors: Jintao Zhang, Kai Jiang, Jintao Chen, Xu Wang, Deyuan Liu, Jungang Li, Dechuang Chen, Ming Lin, Jingjiang Zhou, Haopeng Jin, Qi Jia, Xiaohang Wang, Yaole Wang, Zhanqiang Zhang, Ran Li, Zhengkun Huang, Shuyue Xiong, Yuji Wang, Zikun Dai, Hui He, Yang Luo, Mang Ning, Weiqi Feng, Chengyang Ye, Xinyue Lin, Min Zhao, Hongzhou Zhu, Hengkai Tan, Zeyuan Wang, Chendong Xiang, Kaiwen Zheng, Zhijie Deng, Fan Bao, Jianfei Chen, Jun Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.11638v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://vidu.com/vidu-stream)  
  Keywords: interactive, style, video generation, dit, avatar, video editing  
- **[PAI-Actor: Cinematic Multi-Character Replacement in Dynamic Scenes](https://arxiv.org/abs/2609.05918v1)**  
  Authors: Bangxun Tang, Heyuan Gao, Yiren Song, Guian Fang, Zijian He, Jie Yang, Mike Zheng Shou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.05918v1.pdf)  
  Keywords: video-to-video, film, autoregressive, distillation, diffusion transformer, long-form, dynamics, video generation, efficient  
- **[FixAnything: 3D-Consistent Rendering Refinement via Video Generative Priors](https://arxiv.org/abs/2608.23549v1)**  
  Authors: Khiem Vuong, Deva Ramanan, Srinivasa Narasimhan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.23549v1.pdf)  
  Keywords: video translation, video-to-video, architecture  
- **[InfinityEdit: Infinite Video Editing with a Lightweight Edit-Ignition Adapter](https://arxiv.org/abs/2608.20910v1)**  
  Authors: Yunze Tong, Mushui Liu, Canyu Zhao, Shiyi Zhang, Didi Zhu, Peng Zhang, Wanggui He, Jinlong Liu, Ying Chen, Hao Jiang, Pipei Huang, Bo Zheng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.20910v1.pdf)  
  Keywords: dit, video editing, streaming, denoising  
- **[Identity-Preserving Text-to-Video Generation via Agentic Enhancement and Semantic Repair](https://arxiv.org/abs/2608.20749v1)**  
  Authors: Jiayi Gao, Changcheng Hua, Jiaqi Tang, Yuxin Peng, Yang Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.20749v1.pdf) | [![GitHub](https://img.shields.io/github/stars/oceanflowlab/AESR?style=social)](https://github.com/oceanflowlab/AESR)  
  Keywords: text-to-video, identity, video generation, dit, evaluation, video editing  
- **[EditStream: A Unified Autoregressive Framework for Interactive Video Generation and Editing](https://arxiv.org/abs/2608.21424v1)**  
  Authors: Yuqian Zhou, Zhenghong Zhou, Zongze Wu, Cameron Smith, Richard Zhang, Jiebo Luo, Eli Shechtman, Zhe Lin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.21424v1.pdf)  
  Keywords: text-to-video, image-to-video, video-to-video, streaming, interactive, autoregressive, distillation, video generation, creative, dit, video editing, efficient  

### Video Inpainting & Completion

- **[MT-WAM: Reorienting the One-Pass Predictive Representation Toward Action Generation](https://arxiv.org/abs/2609.21474v1)**  
  Authors: Yiguang Yang, Jiankun Peng, Xiaoming Wang, Yiran Zhang, Zhibo Fang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.21474v1.pdf)  
  Keywords: diffusion transformer, dit, dynamics, video diffusion, video prediction  
- **[StrucPhysVideo: Learning Physical Dynamics from Structured Captions and Robot Actions](https://arxiv.org/abs/2609.18430v1)**  
  Authors: Awomo-WM Team, :, Enhui Ma, Kaiwen Guo, Tingrui Zhang, Wei Song, Yingshui Tan, Jianhua Xu, Tong Zhang, Kaicheng Yu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.18430v1.pdf)  
  Keywords: physics, image-to-video, interactive, physical, autoregressive, action-conditioned, distillation, dit, denoising, dynamics, i2v, video prediction, world model  
- **[GeoLAM: Learning Geometry-Grounded Latent Actions from Unlabeled Human Videos](https://arxiv.org/abs/2609.17099v1)**  
  Authors: Yifan Xie, Hekun Tian, Jinkun Liu, YuAn Wang, Qiao Sun, Wenbo Ding  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.17099v1.pdf)  
  Keywords: benchmark, trajectory, video generation, video prediction, evaluation  
- **[AcrossVAM1.0: Particle World Modeling for Text-Assisted Robot Video Prediction](https://arxiv.org/abs/2608.28491v1)**  
  Authors: Yafei Zhang, Nan Wu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.28491v1.pdf)  
  Keywords: benchmark, film, trajectory, dynamics, video prediction, world model  
- **[V-RAE: Rethinking Video Latent Spaces for Generation](https://arxiv.org/abs/2608.13556v1)**  
  Authors: Minghui Guo, Shengqiong Wu, Hao Fei  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.13556v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://v-rae.github.io)  
  Keywords: latent video, architecture, dit, video generation, video prediction  
- **[GeoRoute: Geometry-Aware Hybrid Inference for Traffic Future-Frame Prediction](https://arxiv.org/abs/2608.09493v1)**  
  Authors: Khang Minh Le, Hieu Dinh Trung Pham, Luu Thanh Danh, Nam-Tien Le, Hieu Anh Ngo, Phuong Huu Vu Tran, Son Nguyen Minh Le, Nguyen Trong Nghia, Tu Tran Thi Cam, Huy Minh Nhat Nguyen, Cuong Tuan Nguyen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.09493v1.pdf)  
  Keywords: benchmark, latent video, architecture, diffusion model, dit, autonomous driving, video diffusion, video prediction  
- **[SimWAM: A Simple World Action Model for End-to-End Autonomous Driving](https://arxiv.org/abs/2608.07468v4)**  
  Authors: Zongchuang Zhao, Xin Zhou, Tianyang Xu, Zhengyang Sun, Kaixuan Zhou, Yu Wu, Honglin Li, Dingkang Liang, Xiang Bai  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.07468v4.pdf) | [![GitHub](https://img.shields.io/github/stars/H-EmbodVis/SimWAM?style=social)](https://github.com/H-EmbodVis/SimWAM)  
  Keywords: trajectory, flow matching, autonomous driving, dynamics, video generation, video prediction, efficient  
- **[MirrorWorld: Taming Video Diffusion Models for Mirror Reflection Generation](https://arxiv.org/abs/2608.07463v1)**  
  Authors: Youjun Zhao, Alex Warren, Gary K. L. Tam, Rynson W. H. Lau  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.07463v1.pdf)  
  Keywords: benchmark, video synthesis, diffusion model, distillation, video inpainting, video diffusion  
- **[UniVVT: A Unified End-to-End Framework for High-Fidelity Video Virtual Try-on](https://arxiv.org/abs/2608.05745v2)**  
  Authors: Yushe Cao, Shikun Feng, Fei Shen, Haikuo Peng, Jianqiang Xia, Yiheng Zhu, Dianxi Shi, Chun Yu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.05745v2.pdf)  
  Keywords: benchmark, identity, video inpainting, dynamics, virtual try-on, video generation, dit  
- **[CrossScope: A Role-Asymmetric World Model for Joint Dual-Scope Surgical Video Prediction](https://arxiv.org/abs/2608.03211v1)**  
  Authors: Wanhao Liu, Jinsong Lin, Rulin Zhou, Chi Kit Ng, Wenbin Pan, Zhiqing Tang, Dongyue Li, Liwei Luo, Yanshen Wu, Panshuo Li, Zhiyong Xiong, Huxin Gao, Tamas Haidegger, Hongliang Ren  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.03211v1.pdf)  
  Keywords: benchmark, dynamics, video generation, video prediction, evaluation, world model  

### Video Super-Resolution & Enhancement

*Showing the latest 50 out of 79 papers*

- **[WorldCrafter: Consistent Video World Model with Implicit 3D-aware Memory](https://arxiv.org/abs/2609.24984v1)**  
  Authors: Wangbo Yu, Kunhao Liu, Wenbo Hu, Shenghai Yuan, Chaoran Feng, Haiyang Zhou, Yukun Huang, Yiran Wang, Wang Zhao, Yingmin Luo, Ying Shan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.24984v1.pdf)  
  Keywords: streaming, interactive, 3d-aware, distillation, dit, denoising, world model  
- **[Why Do Video Diffusion Models Violate Physics? Unveiling the Flaws in Attention Mechanisms](https://arxiv.org/abs/2609.23658v1)**  
  Authors: Yueyan Li, Haibo Wang, Caixia Yuan, Xiaojie Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.23658v1.pdf)  
  Keywords: text-to-video, physics, trajectory, physical, diffusion model, denoising, video diffusion  
- **[4DGS-Fixer: Generative Sparse-View 4D Gaussian Splatting with Iterative Refinement Guided by Video Diffusion Priors](https://arxiv.org/abs/2609.21176v2)**  
  Authors: Haitao Huang, Shenghao Zhao, Boyuan Tian, Shin-Fang Chng, Songlin Yang, Sheila Lim, Huangying Zhan, Yi Xu, Anyi Rao, Frank Guan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.21176v2.pdf)  
  Keywords: benchmark, diffusion model, video restoration, video diffusion  
- **[Video DeltaNet: A Video-Native Hybrid Attention for Livestream Video Generation](https://arxiv.org/abs/2609.20744v2)**  
  Authors: Haocheng Xi, Yiming Xie, Hexu Zhao, Yiwen Zhang, Michael Liu, Thomas Creavin, Kurt Keutzer, Xiuyu Li, Zhaoyang Lv, Chenfeng Xu, Haiwen Feng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.20744v2.pdf) | [![GitHub](https://img.shields.io/github/stars/OpenVDN/vdn-minimax-h3?style=social)](https://github.com/OpenVDN/vdn-minimax-h3) | [![Project](https://img.shields.io/badge/-Project-blue)](https://huggingface.co/OpenVDN/vdn-minimax-h3) | [![HuggingFace](https://img.shields.io/badge/-HuggingFace-yellow)](https://huggingface.co/OpenVDN/vdn-minimax-h3)  
  Keywords: video-to-video, diffusion model, distillation, denoising, video generation, video diffusion, dit  
- **[DART: Distillation-Aware Reparameterization for Training-Free LoRA Reuse in Few-Step Video Diffusion Models](https://arxiv.org/abs/2609.20051v1)**  
  Authors: Shihong Li, Juntao Xu, JinCao, Maowen Tang, Jun Huang, Jintao Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.20051v1.pdf)  
  Keywords: trajectory, diffusion model, distillation, denoising, video generation, video diffusion, dit, evaluation  
- **[Recency Forcing: Bridging the Long-Horizon Gap in Autoregressive Video Generation](https://arxiv.org/abs/2609.19729v1)**  
  Authors: Tri Cao, Hung Nguyen, Phong Nguyen, Khoi Nguyen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.19729v1.pdf)  
  Keywords: autoregressive, dit, video generation, denoising  
- **[StrucPhysVideo: Learning Physical Dynamics from Structured Captions and Robot Actions](https://arxiv.org/abs/2609.18430v1)**  
  Authors: Awomo-WM Team, :, Enhui Ma, Kaiwen Guo, Tingrui Zhang, Wei Song, Yingshui Tan, Jianhua Xu, Tong Zhang, Kaicheng Yu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.18430v1.pdf)  
  Keywords: physics, image-to-video, interactive, physical, autoregressive, action-conditioned, distillation, dit, denoising, dynamics, i2v, video prediction, world model  
- **[Bi-FlowGS: Bridging Generative View Completion and Gaussian Geometry through Bidirectional Flow Co-Refinement](https://arxiv.org/abs/2609.17039v1)**  
  Authors: Yuetong Wang, Jinsheng Quan, Yi Yang, Yawei Luo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.17039v1.pdf)  
  Keywords: benchmark, distillation, video restoration  
- **[LynnReal-Omni: Native multi-modal Video Generation for Agentic Visual Workflows](https://arxiv.org/abs/2609.15863v1)**  
  Authors: Xiaofeng Mao, Peijia Lin, Shaohao Rui, Yibo Zhang, Haibin Wan, Weijie Ma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.15863v1.pdf)  
  Keywords: text-to-video, efficient, controllable, streaming, diffusion model, multi-modal, diffusion transformer, acceleration, video generation, video diffusion, dit, evaluation, video restoration  
- **[Rethinking Streaming Video Diffusion Model: Context, Execution, and Training](https://arxiv.org/abs/2609.22283v1)**  
  Authors: Hongchen Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.22283v1.pdf)  
  Keywords: streaming, diffusion model, denoising, video diffusion, dit  

### World Models & Simulation

*Showing the latest 50 out of 103 papers*

- **[The Past Frames the Future: Memory for Autoregressive Video Generation](https://arxiv.org/abs/2609.28466v1)**  
  Authors: Harold Haodong Chen, Rongjin Guo, Disen Lan, Wen-Jie Shu, Hongfei Zhang, Hanzhe Hu, Shengtao Yao, Zixin Zhang, Guibin Zhang, Zhefan Rao, Jinxiu Liu, Yexin Liu, Rui Peng, Yuhao Liu, Bin Ren, Shuai Yang, Yukang Chen, Salman Khan, Ying-Cong Chen, Ser-Nam Lim, Rynson W. H. Lau, Nicu Sebe, Yu Cheng, Ming-Hsuan Yang, Qifeng Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.28466v1.pdf)  
  Keywords: interactive, architecture, physical, autoregressive, dit, video generation, world model, evaluation  
- **[Code Plans, Diffusion Renders: Open-Ended Generative World Modeling](https://arxiv.org/abs/2609.26458v1)**  
  Authors: Zixun Fang, Yawen Shao, Kai Zhu, Jie Xiao, Shihan Chen, Yu Liu, Xueyang Fu, Yang Cao, Wei Zhai, Zheng-Jun Zha  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.26458v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://becauseimbatman0.github.io/CoDeR)  
  Keywords: concept, dynamics, video generation, world model, evaluation  
- **[QuantWM: Temporally Consistent 2-Bit KV Cache Quantization for World Models and Video Generation](https://arxiv.org/abs/2609.26425v2)**  
  Authors: Jiaqi Zhao, Xiaobin Hu, Bo Yin, Junpeng Jiang, Miao Zhang, Shuicheng Yan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.26425v2.pdf)  
  Keywords: benchmark, temporal consistency, dit, video generation, world model, efficient  
- **[WorldCrafter: Consistent Video World Model with Implicit 3D-aware Memory](https://arxiv.org/abs/2609.24984v1)**  
  Authors: Wangbo Yu, Kunhao Liu, Wenbo Hu, Shenghai Yuan, Chaoran Feng, Haiyang Zhou, Yukun Huang, Yiran Wang, Wang Zhao, Yingmin Luo, Ying Shan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.24984v1.pdf)  
  Keywords: streaming, interactive, 3d-aware, distillation, dit, denoising, world model  
- **[DexTacWAM: A Visuo-Tactile World-Action Model for Dexterous Manipulation](https://arxiv.org/abs/2609.24976v1)**  
  Authors: Haoran Yuan, Zekai Wang, Boning Shao, Haoran Lu, Trevor Darrell, Ismini Lourentzou, Wei Zhan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.24976v1.pdf)  
  Keywords: dit, dynamics, video diffusion, world model, efficient  
- **[UniK: Universal Knowledge Perception for Digital and Physical AI](https://arxiv.org/abs/2609.23971v1)**  
  Authors: Nirmit Desai, Kunal Sawarkar, Aditya Mahakali, Dongkon Lee, Kevin Park, Eric Song  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.23971v1.pdf)  
  Keywords: physical, world model, evaluation, efficient, medical  
- **[Omni Demand Understanding: A Benchmark for Contextual User-Intent Inference in Multimodal Interaction](https://arxiv.org/abs/2609.21392v1)**  
  Authors: Qi Chen, Yunfei Chu, Haolin He, Yifan Yang, Zihan Liu, Yuxuan Wang, Ziyang Ma, Ruiyang Xu, Meng Gao, Yinsong Yan, Ling Wang, Hui Wang, Wen Huang, Yiheng Chen, Guanrou Yang, Qiuqiang Kong, Jin Xu, Xie Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.21392v1.pdf)  
  Keywords: benchmark, evaluation, interactive, video generation  
- **[Astronex-World 1.0: Real-Time Interactive World Model Foundation](https://arxiv.org/abs/2609.20034v1)**  
  Authors: Xin Zhou, Cong Miao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.20034v1.pdf)  
  Keywords: text-to-video, controllable, image-to-video, interactive, autonomous driving, dynamics, i2v, world model  
- **[StrucPhysVideo: Learning Physical Dynamics from Structured Captions and Robot Actions](https://arxiv.org/abs/2609.18430v1)**  
  Authors: Awomo-WM Team, :, Enhui Ma, Kaiwen Guo, Tingrui Zhang, Wei Song, Yingshui Tan, Jianhua Xu, Tong Zhang, Kaicheng Yu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.18430v1.pdf)  
  Keywords: physics, image-to-video, interactive, physical, autoregressive, action-conditioned, distillation, dit, denoising, dynamics, i2v, video prediction, world model  
- **[Can MiniMax-H3 Reason About the Physical World? An Evaluation of Omni-Modal Generative Model](https://arxiv.org/abs/2609.18323v1)**  
  Authors: Haoyu Zhao, Zihao Zhao, Tianyu Deng, Ziqin Xu, Zihao Zhang, Xudong Wang, Jinxiang Guo, Chen Gao, Ziyi Ye, Yeying Jin, Jiaxi Gu, Zuxuan Wu, Shuicheng Yan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.18323v1.pdf) | [![GitHub](https://img.shields.io/github/stars/gulucaptain/MiniMax-H3-Reason?style=social)](https://github.com/gulucaptain/MiniMax-H3-Reason)  
  Keywords: physical, architecture, dynamics, video generation, world model, evaluation  



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
