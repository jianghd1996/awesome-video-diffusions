# Awesome Video Diffusions [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of latest research papers, projects and resources related to Video Diffusion Models and Video Generation. Content is automatically updated daily.

> Last Update: 2026-10-11 04:04:50

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

- [3D-aware Video Generation](#3d-aware-video-generation) (15 papers) - Video generation with 3D awareness, multi-view consistency, and 4D content creation
- [Applications](#applications) (33 papers) - Domain-specific applications of video diffusion models
- [Architecture & Efficiency](#architecture-&-efficiency) (345 papers) - Architectural innovations (DiT, UNet), flow matching, and training/inference efficiency
- [Audio & Multi-modal](#audio-&-multi-modal) (22 papers) - Audio-driven and multi-modal conditioned video generation
- [Controllable Generation](#controllable-generation) (110 papers) - Controllable video generation with motion, camera, pose, or layout guidance
- [Human & Character Animation](#human-&-character-animation) (15 papers) - Human-centric video generation including talking heads, dance, and character animation
- [Image-to-Video Generation](#image-to-video-generation) (32 papers) - Methods for animating still images into videos
- [Long Video Generation](#long-video-generation) (106 papers) - Generating temporally consistent long-form videos beyond short clips
- [Personalization & Customization](#personalization-&-customization) (64 papers) - Personalized video generation with custom subjects, identities, or styles
- [Physical Understanding](#physical-understanding) (137 papers) - Physics-aware video generation and dynamics modeling
- [Surveys & Benchmarks](#surveys-&-benchmarks) (252 papers) - Survey papers, benchmarks, and evaluation metrics for video generation
- [Text-to-Video Generation](#text-to-video-generation) (57 papers) - Foundation models and methods for generating videos from text prompts
- [Video Editing](#video-editing) (19 papers) - Diffusion-based video editing, style transfer, and manipulation
- [Video Inpainting & Completion](#video-inpainting-&-completion) (5 papers) - Video inpainting, completion, outpainting, and temporal prediction
- [Video Super-Resolution & Enhancement](#video-super-resolution-&-enhancement) (75 papers) - Video quality improvement, upscaling, restoration, and frame interpolation
- [World Models & Simulation](#world-models-&-simulation) (109 papers) - Video generation as world simulators and interactive environment generation



## Table of Contents

- [Categorized Papers](#categorized-papers)
- [Classic Papers](#classic-papers)
- [Open Source Projects](#open-source-projects)
- [Applications](#applications)
- [Tutorials & Blogs](#tutorials--blogs)





## Categorized Papers

### 3D-aware Video Generation

- **[LEGO: A Lifting-Free Approach for Exocentric-to-Egocentric Video Generation](https://arxiv.org/abs/2610.12442v1)**  
  Authors: Suhwan Cho, Yonwoo Choi, Soongjin Kim, Jicheol Park, Taegyu Lim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.12442v1.pdf)  
  Keywords: dit, style, video diffusion, layout, diffusion model, video generation, denoising, novel view  
- **[SepGen: Multi-Stem Audio-Video Separation and Generation in a Single Model](https://arxiv.org/abs/2610.11361v1)**  
  Authors: Aviad Dahan, Rajaei Khatib, Yonatan Bitton, Idan Szpektor, Lior Wolf, Raja Giryes  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.11361v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://sepgen.github.io)  
  Keywords: novel view, dit, sound, trajectory  
- **[GeoVerse: World-Consistent Novel View Synthesis in Geometric Latent Space](https://arxiv.org/abs/2609.35734v2)**  
  Authors: Kerui Ren, Tao Lu, Linning Xu, Changjian Jiang, Mu Huang, Chunhua Shen, Mulin Yu, Bo Dai  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.35734v2.pdf)  
  Keywords: diffusion model, novel view, style  
- **[GenNVS: Geometry-enhanced Novel View Synthesis via Disentangled 3D Prior](https://arxiv.org/abs/2609.34579v2)**  
  Authors: Yajiao Xiong, Youyu Luan, Xiaoyu Zhou, Yongtao Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.34579v2.pdf)  
  Keywords: novel view, diffusion model, dit, video diffusion  
- **[VGGT-Diff: Visual Geometry Meets Diffusion for Sparse-View Novel View Synthesis](https://arxiv.org/abs/2609.33253v1)**  
  Authors: Kangjie Chen, Xiangyu Li, Dongbin Zhang, Chaoda Zheng, Shijia Chen, Jinhao Deng, Hongbin Lin, Choo Sin Wai, Minqi Wang, Minghao Yang, Dake Zhong, Guorui Song, Yu Zhang, Xianming Liu, Boyang Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.33253v1.pdf) | [![GitHub](https://img.shields.io/github/stars/chenkangjie1123/VGGT-Diff?style=social)](https://github.com/chenkangjie1123/VGGT-Diff)  
  Keywords: dit, video diffusion, diffusion model, denoising, novel view  
- **[WorldCrafter: Consistent Video World Model with Implicit 3D-aware Memory](https://arxiv.org/abs/2609.24984v1)**  
  Authors: Wangbo Yu, Kunhao Liu, Wenbo Hu, Shenghai Yuan, Chaoran Feng, Haiyang Zhou, Yukun Huang, Yiran Wang, Wang Zhao, Yingmin Luo, Ying Shan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.24984v1.pdf)  
  Keywords: interactive, dit, distillation, streaming, denoising, 3d-aware, world model  
- **[Printing the Underdetermined: Materializing Multi-solutionness in Figurative Paintings](https://arxiv.org/abs/2609.19782v2)**  
  Authors: Yutao Ming, Teng Xu, Youjia Wang, Yunyang Liu, Fengmin Yang, Fuqiang Zhao, Jingyi Yu, Hua Yang, Yanjun Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.19782v2.pdf)  
  Keywords: physical, dit, multi-view video  
- **[Rethinking 3D Noise: Learning 3D-Aware Video Priors via Optimization-Free Morphological Perturbations](https://arxiv.org/abs/2609.03657v1)**  
  Authors: Onat Şahin, Mohammad Altillawi, George Eskandar, Carlos Carbone, Ziyuan Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.03657v1.pdf)  
  Keywords: 3d-aware, video diffusion, robotics  
- **[Stabilizing Camera-Controlled Novel View Synthesis at Inference Time](https://arxiv.org/abs/2609.03639v1)**  
  Authors: Prajwal Singh, Arjun Badola, Seema Kumari, Hajime Nagahara, Shanmuganathan Raman  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.03639v1.pdf)  
  Keywords: efficient, video diffusion, diffusion model, autoregressive, novel view  
- **[Building Pretraining Data for World Models: An Unreal Engine-Based Pipeline for Action-Conditioned Video Generation](https://arxiv.org/abs/2609.03557v1)**  
  Authors: Haoyu Wang, Songchun Zhang, Haoran Li, Haoyang Huang, Zeyue Xue, Nan Duan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.03557v1.pdf)  
  Keywords: architecture, dit, action-conditioned, trajectory, multi-view video, video generation, physics, world model  

### Applications

- **[AdSpark: A Large-Scale Dataset and Benchmark for Product-Centric Advertisement Video Generation](https://arxiv.org/abs/2610.10047v1)**  
  Authors: Zhifei Yang, Zhao Jiang, Keyang Lu, Honghe Zhu, Zheng Zhang, Jingjing Lv, Changping Peng, Ching Law, Zhen Xiao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.10047v1.pdf)  
  Keywords: creative, benchmark, video generation, identity, evaluation  
- **[Beyond Masks and Trajectories: Flow-Guided Latent Action Injection for Stable Surgical Video Generation](https://arxiv.org/abs/2610.09800v1)**  
  Authors: Tsz-Yui Qin, Siyu Zhou, Chi-Keung Tang, Yuxiang Nie, Shu Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.09800v1.pdf)  
  Keywords: architecture, dit, education, video generation, simulation, evaluation  
- **[DepthWorld: 3D World Model for Robot Manipulation](https://arxiv.org/abs/2610.08780v1)**  
  Authors: Jai Bardhan, Josef Sivic, Vladimir Petrik  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.08780v1.pdf)  
  Keywords: architecture, physical, dit, video diffusion, robotics, evaluation, world model  
- **[Transferable Spatial Temporal Coherence Adversarial Attack on Black-Box Vision Language Models for Autonomous Driving](https://arxiv.org/abs/2610.08331v1)**  
  Authors: Heyam Bin Jahlan Areej Alhothali Abeer Alhothali  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.08331v1.pdf)  
  Keywords: autonomous driving  
- **[DiVid: Diagnosing Dimension-Specific Diversity Collapse in Video Generation Models](https://arxiv.org/abs/2610.01661v1)**  
  Authors: Huanran Hu, Zihui Ren, Dingyi Yang, Zhinan Song, Guozheng Wu, Tiezheng Ge, Qin Jin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.01661v1.pdf)  
  Keywords: style, video generation, creative, evaluation, controllable  
- **[PhysicsLENS: Diagnosing Physical Property Blindness in Video Generation Models](https://arxiv.org/abs/2610.01162v1)**  
  Authors: Isaiah Milkey, Som Sagar, Aditya Taparia, Xinyuan Liu, Jiqing Wen, Ransalu Senanayake  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.01162v1.pdf)  
  Keywords: physical, dit, robotics, benchmark, video generation, physics, evaluation, world model  
- **[Bootstrapping Video Interaction Generation with Synthetic State Transitions](https://arxiv.org/abs/2610.01039v1)**  
  Authors: Jiho Jang, Jinyoung Kim, Nojun Kwak, Kyungjune Kim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.01039v1.pdf)  
  Keywords: physical, dit, robotics, evaluation, controllable  
- **[Harnessing Vision-Language Models for Perceptual Quality Assessment and Autonomous Content Adjustment in Augmented Reality](https://arxiv.org/abs/2610.00677v1)**  
  Authors: Elias Rotondo, Lin Duan, Yanming Xiu, Sangjun Eom, Conrad Li, Maria Gorlatova  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.00677v1.pdf)  
  Keywords: evaluation, dit, benchmark, education  
- **[GroundingPI: A Grounding Foundation Model towards Physical Intelligence with Visual Primitives](https://arxiv.org/abs/2609.39601v1)**  
  Authors: Qize Yu, Lianrui Fan, Boyu Chen, Jiaqi Liang, Xini Ding, Yue Chen, Zetian Song, Yuran Wang, Yi Zou, Kaixuan Wang, Tianxing Chen, Wenxuan Song, Bohan Zhou, Mingleyang Li, Siqiao Huang, Yuqi Ye, Caigao Jiang, Wei Wei, Ruihai Wu, Hang Zhang, Yixiao Ge, Shuchang Zhou, Shilong Liu, Xianming Liu, Ping Luo, Shiyu Huang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.39601v1.pdf)  
  Keywords: physical, autonomous driving, benchmark  
- **[Exo2EgoHOI: Hand-Object-Interaction Aware Exocentric-to-Egocentric Video Generation](https://arxiv.org/abs/2609.38615v1)**  
  Authors: Hongjia Zhai, Xiyu Zhang, Haoran Zhang, Zhichao Ye, Haomin Liu, Guofeng Zhang, Ian Reid, Xingxing Zuo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.38615v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://rcl-robotics.github.io/Exo2EgoHOI)  
  Keywords: video generation, robotics  

### Architecture & Efficiency

*Showing the latest 50 out of 345 papers*

- **[WorldGuide: Goal-Directed Video World Model for Procedural Task Execution](https://arxiv.org/abs/2610.12459v1)**  
  Authors: Ankan Deria, Komal Kumar, Hisham Cholakkal, Fahad Shahbaz Khan, Salman Khan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.12459v1.pdf)  
  Keywords: video generation, dit, world model  
- **[LEGO: A Lifting-Free Approach for Exocentric-to-Egocentric Video Generation](https://arxiv.org/abs/2610.12442v1)**  
  Authors: Suhwan Cho, Yonwoo Choi, Soongjin Kim, Jicheol Park, Taegyu Lim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.12442v1.pdf)  
  Keywords: dit, style, video diffusion, layout, diffusion model, video generation, denoising, novel view  
- **[WorldCast: Distributed Multiplayer World Models](https://arxiv.org/abs/2610.12412v1)**  
  Authors: Ziyang Ye, Junchao Huang, Evelyn Zhang, Zhihao Xie, Ruicheng Zhang, Boyao Han, Litao Ban, Ziye Wang, Xinting Hu, Shaoshuai Shi, Zhuotao Tian, Li Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.12412v1.pdf)  
  Keywords: dit, world model  
- **[Connected Self Forcing: Beyond Local Learning in Video Autoregression](https://arxiv.org/abs/2610.12156v1)**  
  Authors: Dongbin Zhang, Chaoda Zheng, Kangjie Chen, Xiangyu Li, Shijia Chen, Jinhao Deng, Yuqi Zhang, Guangfeng Jiang, Hongbin Lin, Choo Sin Wai, Minqi Wang, Puyi Wang, Jingye Zhang, Yu Zhang, Xianming Liu, Boyang Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.12156v1.pdf)  
  Keywords: temporal consistency, efficient, long video, distillation, video generation, autoregressive  
- **[VINCIE-NExT: Unlocking Video Editing from Images via In-Context Modeling](https://arxiv.org/abs/2610.12104v1)**  
  Authors: Leigang Qu, Feng Cheng, Ziyan Yang, Bangbang Yang, Zhaoyang Huang, Wei Chow, Yicong Li, Wenjie Wang, Tat-Seng Chua, Yan Zeng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.12104v1.pdf)  
  Keywords: video editing, dit  
- **[Reliability-Aware Future Conditioning for Temporally Robust Robot Manipulation](https://arxiv.org/abs/2610.11956v1)**  
  Authors: Mohammad Khoshnazar, Mohammad Dehghani Tezerjani, Zhiyuan Gao, Deyuan Qu, Max Gandyra, Yanxiang Zhan, Mehreen Naeem, Andrew Melnik, Jeroen Schafer, Qing Yang, Michael Beetz  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.11956v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://future-condition.github.io)  
  Keywords: dit, video diffusion  
- **[VEDJE: Video-Efficient Discriminative Joint Encoder for Scalable Video-Text Retrieval](https://arxiv.org/abs/2610.11850v1)**  
  Authors: Shahaf Wagner, Gabriele Serussi, Dan Ben Ami, Tomer Galanti, Chaim Baskin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.11850v1.pdf)  
  Keywords: text-to-video, efficient  
- **[Phase-aware video generation for physics-grounded dynamics and interactions](https://arxiv.org/abs/2610.11791v1)**  
  Authors: Jingfeng Ou, Kun Wang, Rui Zhao, Jingwei Guan, Limin Wang, Chao Dong, Xingyu Zeng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.11791v1.pdf)  
  Keywords: architecture, physical, video generation, simulation, physics, dynamics, evaluation  
- **[From Video Clips to Creation Trajectory: Sora100K for AI-Native Video Creation](https://arxiv.org/abs/2610.11770v1)**  
  Authors: Sicong Yang, Ruihuan Yang, Jian Lu, Jianfei Yuan, Xiaodong Cun, Xiuli Bi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.11770v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://huggingface.co/datasets/ysicong/Sora100K.) | [![Dataset](https://img.shields.io/badge/-Dataset-orange)](https://huggingface.co/datasets/ysicong/Sora100K)  
  Keywords: dit, trajectory, video editing, video generation, text-to-video, evaluation  
- **[Towards Unified Evaluation of Prompt Enhancers for Video Generation](https://arxiv.org/abs/2610.11736v1)**  
  Authors: Yawen Shao, Yubo Zhu, Ziyun Dai, Zixun Fang, Kai Zhu, Zeyinzi Jiang, Yufeng Ai, Siyang Sun, Haolan Xue, Yu Shang, Yuxiang Bao, Zoubin Bi, Jingming Luo, Jie Xiao, Chaojie Mao, Zhehan Kan, Hongchen Luo, Yu Liu, Sheng Zhong, Wei Tong, Xueyang Fu, Yang Cao, Wei Zhai, Zheng-Jun Zha  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.11736v1.pdf)  
  Keywords: dit, benchmark, video generation, text-to-video, image-to-video, evaluation  

### Audio & Multi-modal

- **[SepGen: Multi-Stem Audio-Video Separation and Generation in a Single Model](https://arxiv.org/abs/2610.11361v1)**  
  Authors: Aviad Dahan, Rajaei Khatib, Yonatan Bitton, Idan Szpektor, Lior Wolf, Raja Giryes  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.11361v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://sepgen.github.io)  
  Keywords: novel view, dit, sound, trajectory  
- **[PVSync: A Unified Lip-Sync Expert for Timing and Articulation](https://arxiv.org/abs/2610.09223v1)**  
  Authors: Kevin Stephen, Varun Menon, Timo Mertens, Nikita Drobyshev  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.09223v1.pdf)  
  Keywords: video generation, benchmark, sound  
- **[AiSearch: Interactive Multi-Modal Search with VLMs](https://arxiv.org/abs/2610.01389v1)**  
  Authors: Ali Koksal, Mei Chee Leong, Vicky Sintunata, Ching Ling Chin, Wee Teck Fong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.01389v1.pdf)  
  Keywords: interactive, benchmark, multi-modal  
- **[Watch Your Speech: Text-aware Video-to-Speech Synthesis with Textual Conditioning](https://arxiv.org/abs/2610.01012v1)**  
  Authors: Gunwoo Lee, Yoori Oh, Yoseob Han  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.01012v1.pdf) | [![GitHub](https://img.shields.io/github/stars/gunwoo5034/Watch-your-Speech?style=social)](https://github.com/gunwoo5034/Watch-your-Speech)  
  Keywords: dit, flow matching, sound, dynamics, evaluation  
- **[Soundwich: Video Generation with Layered and Controllable Audio](https://arxiv.org/abs/2610.00691v2)**  
  Authors: Zhuo Ning, AmirHossein Naghi Razlighi, Sagi Polaczek, Daniel Cohen-Or, Ali Mahdavi-Amiri  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.00691v2.pdf) | [![GitHub](https://img.shields.io/github/stars/CodyNing/Soundwich?style=social)](https://github.com/CodyNing/Soundwich)  
  Keywords: dit, sound, video generation, evaluation, controllable  
- **[GLARE: Generating Listening Heads with Appropriate Reactions](https://arxiv.org/abs/2609.40317v1)**  
  Authors: Zikai Liao, Yumin Suh, Yi Ouyang, Yi-Lun Lee, Yi-Hsuan Tsai, Zhaozheng Yin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.40317v1.pdf)  
  Keywords: dit, audio-driven, video generation, talking head, evaluation  
- **[Enabling Immersive Audio-Visual Experience from Any Video](https://arxiv.org/abs/2609.36295v1)**  
  Authors: Zitong Lan, Mutian Tong, Jiatao Gu, Mingmin Zhao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.36295v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://huggingface.co/spaces/CuriousAlien000/spatial-audio-360-demo) | [![HuggingFace](https://img.shields.io/badge/-HuggingFace-yellow)](https://huggingface.co/spaces/CuriousAlien000/spatial-audio-360-demo)  
  Keywords: physics, video generation, simulation, sound  
- **[SkillPE: Creativity-Oriented Cinematic Skill Evolution for Text-to-Video Prompt Engineering](https://arxiv.org/abs/2609.34335v1)**  
  Authors: Yanwei Huang, Mingxuan Zhu, Shujie Li, Shiyuan Liu, Yuanxing Zhang, Arpit Narechania  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.34335v1.pdf) | [![GitHub](https://img.shields.io/github/stars/Ais0n/SkillPE?style=social)](https://github.com/Ais0n/SkillPE)  
  Keywords: film, benchmark, sound, video generation, text-to-video, creative, evaluation  
- **[Where and When to Force: Routed Forcing for Streaming Avatars](https://arxiv.org/abs/2609.30963v1)**  
  Authors: Zihan Su, Siwen Lu, Junhao Zhuang, Zeyue Xue, Haoyang Huang, Guanghao Li, Xiaofeng Tan, Chun Yuan, Nan Duan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.30963v1.pdf)  
  Keywords: video diffusion, distillation, diffusion model, gesture, audio-driven, streaming, dynamics, avatar  
- **[WanPE: Towards Cinematic Prompt Enhancement for Modern Text-to-Video Generation](https://arxiv.org/abs/2609.30221v1)**  
  Authors: Yubo Zhu, Yawen Shao, Ziyun Dai, Zixun Fang, Kai Zhu, Siyang Sun, Haolan Xue, Chuxin Wang, Tingyu Weng, Jingming Luo, Chen Shi, Lianghua Huang, Yufeng Ai, Yuzheng Wang, Wenyuan Zhang, Yu Shang, Yuxiang Bao, Zoubin Bi, Jie Xiao, Jinbo Xing, Jiaxing Zhao, Chongyang Zhong, Hengjian Chen, Chenwei Xie, Akide Liu, Zhehan Kan, Yu Liu, Wei Zhai, Sheng Zhong, Wei Tong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.30221v1.pdf)  
  Keywords: dit, benchmark, sound, video generation, text-to-video  

### Controllable Generation

*Showing the latest 50 out of 110 papers*

- **[LEGO: A Lifting-Free Approach for Exocentric-to-Egocentric Video Generation](https://arxiv.org/abs/2610.12442v1)**  
  Authors: Suhwan Cho, Yonwoo Choi, Soongjin Kim, Jicheol Park, Taegyu Lim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.12442v1.pdf)  
  Keywords: dit, style, video diffusion, layout, diffusion model, video generation, denoising, novel view  
- **[From Video Clips to Creation Trajectory: Sora100K for AI-Native Video Creation](https://arxiv.org/abs/2610.11770v1)**  
  Authors: Sicong Yang, Ruihuan Yang, Jian Lu, Jianfei Yuan, Xiaodong Cun, Xiuli Bi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.11770v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://huggingface.co/datasets/ysicong/Sora100K.) | [![Dataset](https://img.shields.io/badge/-Dataset-orange)](https://huggingface.co/datasets/ysicong/Sora100K)  
  Keywords: dit, trajectory, video editing, video generation, text-to-video, evaluation  
- **[Parametric Trajectory Distillation for Few-Step Video Generation](https://arxiv.org/abs/2610.11498v1)**  
  Authors: Lan Feng, Peter Karkus, Maximilian Igl, Julius Berner, Yuxiao Chen, Shuhan Tan, Alexandre Alahi, Boris Ivanovic, Marco Pavone  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.11498v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://alan-lanfeng.github.io/PTD)  
  Keywords: architecture, video diffusion, trajectory, distillation, video generation, evaluation  
- **[SepGen: Multi-Stem Audio-Video Separation and Generation in a Single Model](https://arxiv.org/abs/2610.11361v1)**  
  Authors: Aviad Dahan, Rajaei Khatib, Yonatan Bitton, Idan Szpektor, Lior Wolf, Raja Giryes  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.11361v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://sepgen.github.io)  
  Keywords: novel view, dit, sound, trajectory  
- **[TKCAM: Text and Keyframe to Camera Trajectory Generation](https://arxiv.org/abs/2610.11105v1)**  
  Authors: Haozhe Yang, Zhiyang Dou, Zekai Gu, Cheng Lin, Wenping Wang, Yuan Liu, Taku Komura  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.11105v1.pdf) | [![GitHub](https://img.shields.io/github/stars/linearalgebrayhz/TKCAM?style=social)](https://github.com/linearalgebrayhz/TKCAM)  
  Keywords: architecture, dit, trajectory, benchmark, video synthesis, dynamics, evaluation, controllable  
- **[Fluid-Gen-Zero: Grounding Pretrained Video Generators in Physics without Training](https://arxiv.org/abs/2610.10984v1)**  
  Authors: Hong Huang, Yuqiu Liu, Chenyu You, Daniel Martin, Chuhang Zou, Wuyang Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.10984v1.pdf)  
  Keywords: physical, trajectory, benchmark, video generation, denoising, simulation, physics, dynamics, physics-aware  
- **[OmniCam: Omni-Camera Trajectory Generation via Geometry-Grounded Pose Token Learning](https://arxiv.org/abs/2610.09513v1)**  
  Authors: Zhenyang Liu, Chenjie Cao, Yisu Zhang, Xuhui Zuo, Xiangyang Xue, Yanwei Fu, Tengfei Wang, Chunchao Guo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.09513v1.pdf)  
  Keywords: dit, trajectory, video generation, autoregressive, evaluation  
- **[ChronoWorld: Camera-Controlled Consistent 4D World Generation via Spatiotemporal Cues and Geometric Reflections](https://arxiv.org/abs/2610.06687v2)**  
  Authors: Xiaoyu Zhou, Dingwei Xian, Zhenyu Wang, Yajiao Xiong, Yongtao Wang, Ming-Hsuan Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.06687v2.pdf)  
  Keywords: video generation, dit, controllable  
- **[SimForcing: Distilling Simulation Motion Priors into Real-Domain Robot World Models](https://arxiv.org/abs/2610.06598v1)**  
  Authors: Xiaodong Wang, Tianle Li, Chuanxin Song, Junliang Xie, Zhanmi Zhong, Suiying Wu, Peixi Peng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.06598v1.pdf) | [![GitHub](https://img.shields.io/github/stars/Wang-Xiaodong1899/SimForcing?style=social)](https://github.com/Wang-Xiaodong1899/SimForcing)  
  Keywords: dit, action-conditioned, distillation, video generation, simulation, dynamics, evaluation, world model, controllable  
- **[Level-of-Token Diffusion](https://arxiv.org/abs/2610.05816v1)**  
  Authors: Kiyohiro Nakayama, Brian Chao, Jan Ackermann, Hansheng Chen, Federico Tombari, Leonidas Guibas, Lior Yariv, Gordon Wetzstein  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.05816v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://georgenakayama.github.io/lotdiffusion)  
  Keywords: efficient, video diffusion, layout, diffusion model, video generation, diffusion transformer, denoising  

### Human & Character Animation

- **[PixReenact: Pixel-Conditioned Causal Video Diffusion for Streaming Head-Avatar Reenactment](https://arxiv.org/abs/2610.05233v1)**  
  Authors: Gavriel Habib, Dvir Samuel, Or Shimshi, Rami Ben-Ari  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.05233v1.pdf)  
  Keywords: dit, video diffusion, distillation, benchmark, streaming, autoregressive, denoising, identity, avatar  
- **[Parasitic Co-Denoising: Unlocking 3D Human Motion Generation in a Frozen Video Diffusion Model](https://arxiv.org/abs/2610.03047v1)**  
  Authors: Yunjiao Zhou, Junlang Qian, Lihua Xie, Jianfei Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03047v1.pdf)  
  Keywords: human motion, efficient, video diffusion, diffusion model, text-to-video, denoising  
- **[GLARE: Generating Listening Heads with Appropriate Reactions](https://arxiv.org/abs/2609.40317v1)**  
  Authors: Zikai Liao, Yumin Suh, Yi Ouyang, Yi-Lun Lee, Yi-Hsuan Tsai, Zhaozheng Yin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.40317v1.pdf)  
  Keywords: dit, audio-driven, video generation, talking head, evaluation  
- **[TexTailor: Texture-Preserving Video Virtual Try-On via Adaptive Garment Conditioning](https://arxiv.org/abs/2609.39335v1)**  
  Authors: Zijing Qin, Jun Zhou, Ruicheng Zhang, Jiaqi Hou, Zunnan Xu, Ronghui Li, Zhenyu Xie, Xiu Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.39335v1.pdf)  
  Keywords: temporal consistency, dit, video diffusion, benchmark, diffusion transformer, denoising, virtual try-on  
- **[WeLike2Party! In-Context Motion Transfer for Multi-Human Image Animation](https://arxiv.org/abs/2609.36937v1)**  
  Authors: Sangeyl Lee, Seunghyun Shin, Seungho Park, Wooseok Jeon, Hae-Gon Jeon  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.36937v1.pdf)  
  Keywords: dit, trajectory, benchmark, video generation, image animation, human animation, identity  
- **[FlowAct-R2: Beyond Talking Avatar via Streaming Multimodal References and Proactive Agent Planning](https://arxiv.org/abs/2609.35728v1)**  
  Authors: Ziyao Huang, Zhengkun Rong, Shiyang Qin, Shuang Liang, Wentao Hu, Yuxuan Luo, Yuan Zhang, Mingyuan Gao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.35728v1.pdf)  
  Keywords: interactive, dit, video generation, streaming, diffusion transformer, avatar  
- **[Where and When to Force: Routed Forcing for Streaming Avatars](https://arxiv.org/abs/2609.30963v1)**  
  Authors: Zihan Su, Siwen Lu, Junhao Zhuang, Zeyue Xue, Haoyang Huang, Guanghao Li, Xiaofeng Tan, Chun Yuan, Nan Duan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.30963v1.pdf)  
  Keywords: video diffusion, distillation, diffusion model, gesture, audio-driven, streaming, dynamics, avatar  
- **[All modalities are equal, but video is more equal: Closing the Cross-Attention Gap in Joint Video Generation](https://arxiv.org/abs/2609.27901v1)**  
  Authors: Ohad Rahamim, Dvir Samuel, Idan Schwartz, Gal Chechik  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.27901v1.pdf)  
  Keywords: physical, video generation, diffusion transformer, body motion  
- **[When Visual Quality Misleads: Intent Recognition under Rendered Avatar Distortions](https://arxiv.org/abs/2609.27560v1)**  
  Authors: Ning-Hsuan Chang, Kai-Siang Ma, Yu-Chih Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.27560v1.pdf)  
  Keywords: streaming, dit, avatar  
- **[Vidu S2: Real-Time Interactive, Editable, and Spatial Video Generation](https://arxiv.org/abs/2609.11638v1)**  
  Authors: Jintao Zhang, Kai Jiang, Jintao Chen, Xu Wang, Deyuan Liu, Jungang Li, Dechuang Chen, Ming Lin, Jingjiang Zhou, Haopeng Jin, Qi Jia, Xiaohang Wang, Yaole Wang, Zhanqiang Zhang, Ran Li, Zhengkun Huang, Shuyue Xiong, Yuji Wang, Zikun Dai, Hui He, Yang Luo, Mang Ning, Weiqi Feng, Chengyang Ye, Xinyue Lin, Min Zhao, Hongzhou Zhu, Hengkai Tan, Zeyuan Wang, Chendong Xiang, Kaiwen Zheng, Zhijie Deng, Fan Bao, Jianfei Chen, Jun Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.11638v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://vidu.com/vidu-stream)  
  Keywords: interactive, dit, style, video editing, video generation, avatar  

### Image-to-Video Generation

- **[WorldAlign: Decoupled 4D Reward for World-Consistent Video Generation](https://arxiv.org/abs/2610.12382v1)**  
  Authors: Jing He, Kaixin Ding, Xingye Tian, Guibao Shen, Wenhang Ge, Xin Tao, Pengfei Wan, Ying-Cong Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.12382v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://worldalign.github.io)  
  Keywords: physical, video generation, simulation, image-to-video, evaluation  
- **[Towards Unified Evaluation of Prompt Enhancers for Video Generation](https://arxiv.org/abs/2610.11736v1)**  
  Authors: Yawen Shao, Yubo Zhu, Ziyun Dai, Zixun Fang, Kai Zhu, Zeyinzi Jiang, Yufeng Ai, Siyang Sun, Haolan Xue, Yu Shang, Yuxiang Bao, Zoubin Bi, Jingming Luo, Jie Xiao, Chaojie Mao, Zhehan Kan, Hongchen Luo, Yu Liu, Sheng Zhong, Wei Tong, Xueyang Fu, Yang Cao, Wei Zhai, Zheng-Jun Zha  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.11736v1.pdf)  
  Keywords: dit, benchmark, video generation, text-to-video, image-to-video, evaluation  
- **[Transforming Image Editors into Video Editors](https://arxiv.org/abs/2610.11037v1)**  
  Authors: Feng Wang, Zijie Li, Ceyuan Yang, Alan Yuille, Peng Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.11037v1.pdf) | [![GitHub](https://img.shields.io/github/stars/wangf3014/AVE?style=social)](https://github.com/wangf3014/AVE)  
  Keywords: temporal consistency, dit, video diffusion, diffusion model, video editing, image-to-video  
- **[GRACE: Generation-aware latent compression for efficient video generation](https://arxiv.org/abs/2610.10524v1)**  
  Authors: Jiyoung Kim, Paul Hyunbin Cho, Jisu Nam, Donghoon Lee, Hyunsung Go, Yeonkyeong Lee, Hansaem Kim, Seungryong Kim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.10524v1.pdf)  
  Keywords: dit, efficient, i2v, video diffusion, diffusion model, video generation, diffusion transformer, denoising  
- **[TasteRoute: Personalized Routing for Video Generation](https://arxiv.org/abs/2610.05896v1)**  
  Authors: Zhi Rui Tam, Chao-Chung Wu, Sin-Han Yang, Peyton Ku, Brendan Kuang, Tzu-Ting Hsieh, Min-Fang Hsu, Fang-Ling Tsai, Yun-Nung Chen, Wei-Chiu Ma, Chieh-Yen Lin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.05896v1.pdf)  
  Keywords: video generation, efficient, text-to-video, image-to-video  
- **[Generating the Wild: Individual-Consistent Image-to-Video Generation for Wildlife](https://arxiv.org/abs/2610.05587v1)**  
  Authors: Yuzhuo Li, Di Zhao, Xinyu Zhang, Daniel Wilson, Yun Sing Koh  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.05587v1.pdf)  
  Keywords: dit, i2v, layout, video generation, motion control, identity, image-to-video, evaluation  
- **[How Does Geometry Enter Generated Motion?](https://arxiv.org/abs/2610.05135v1)**  
  Authors: Weihan Li, Junhao Wu, Yuhan Song, Xiaofeng Lin, Xinlei Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.05135v1.pdf)  
  Keywords: physical, dit, trajectory, video generation, image-to-video  
- **[VDOT++: Unified Few-Step Video Generation via Unbalanced Optimal Transport Distillation](https://arxiv.org/abs/2610.03221v1)**  
  Authors: Yutong Wang, Xingtong Ge, Enhuai Liu, Yunke Wang, Tianfan Xue, Yu Qiao, Yaohui Wang, Xinyuan Chen, Chang Xu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03221v1.pdf)  
  Keywords: dit, i2v, video diffusion, distillation, diffusion model, benchmark, video generation, text-to-video, image-to-video, t2v  
- **[Custom Forcing: Training-Free Subject Customization for Autoregressive Video Generation](https://arxiv.org/abs/2610.02914v2)**  
  Authors: Yunseung Ok, Hyunsoo Kim, Minseo Kim, Suhyun Kim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.02914v2.pdf)  
  Keywords: dit, long video, video generation, streaming, autoregressive, identity, customization, image-to-video  
- **[MosaiChunk: Compositing Spatio-Temporal Memory for Autoregressive Video Generation](https://arxiv.org/abs/2610.02153v1)**  
  Authors: Yiwen Zhang, Haocheng Xi, Michael Tian-Yue Liu, Alexei A. Efros, Hadar Averbuch-Elor, Qianqian Wang, Haiwen Feng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.02153v1.pdf)  
  Keywords: i2v, benchmark, video generation, text-to-video, autoregressive, image-to-video, t2v  

### Long Video Generation

*Showing the latest 50 out of 106 papers*

- **[Connected Self Forcing: Beyond Local Learning in Video Autoregression](https://arxiv.org/abs/2610.12156v1)**  
  Authors: Dongbin Zhang, Chaoda Zheng, Kangjie Chen, Xiangyu Li, Shijia Chen, Jinhao Deng, Yuqi Zhang, Guangfeng Jiang, Hongbin Lin, Choo Sin Wai, Minqi Wang, Puyi Wang, Jingye Zhang, Yu Zhang, Xianming Liu, Boyang Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.12156v1.pdf)  
  Keywords: temporal consistency, efficient, long video, distillation, video generation, autoregressive  
- **[Memory Forcing: Attendable Mid-Horizon History for Streaming Video Generation](https://arxiv.org/abs/2610.11756v1)**  
  Authors: Jiaming Zhang, Xinyu Wang, Huafeng Shi, Gangshan Wu, Limin Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.11756v1.pdf)  
  Keywords: physical, video diffusion, video generation, streaming, autoregressive  
- **[Conditional Residual Prediction: Improving Autoregressive Video Diffusion without a Bidirectional Teacher](https://arxiv.org/abs/2610.11479v1)**  
  Authors: Bowen Zheng, Zhiguang Liu, Jiarong Ou, Rui Chen, Tianyang Hu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.11479v1.pdf)  
  Keywords: interactive, dit, video diffusion, distillation, diffusion model, video generation, streaming, autoregressive  
- **[Transforming Image Editors into Video Editors](https://arxiv.org/abs/2610.11037v1)**  
  Authors: Feng Wang, Zijie Li, Ceyuan Yang, Alan Yuille, Peng Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.11037v1.pdf) | [![GitHub](https://img.shields.io/github/stars/wangf3014/AVE?style=social)](https://github.com/wangf3014/AVE)  
  Keywords: temporal consistency, dit, video diffusion, diffusion model, video editing, image-to-video  
- **[SGF+: Decoupling Gradient Flows for Autoregressive Video Generation](https://arxiv.org/abs/2610.10429v2)**  
  Authors: Zihan Su, Junhao Zhuang, Yaowei Li, Siwen Lu, Haoran Li, Lingen Li, Haoyu Wu, Weiyang Jin, Songchun Zhang, Haoyang Huang, Chun Yuan, Zeyue Xue, Nan Duan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.10429v2.pdf)  
  Keywords: temporal consistency, dit, video generation, autoregressive, denoising  
- **[Self-correction Optimization for Interleaved Multimodal Generation](https://arxiv.org/abs/2610.10400v1)**  
  Authors: Xin You, Zhiwei Ning, Zukai Chen, Minghui Zhang, Xuanke Shi, Hanxiao Zhang, Jingsong Liu, Jie Yang, Quan Wang, Yun Gu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.10400v1.pdf)  
  Keywords: temporal consistency, physical, dit, benchmark, video generation  
- **[Real-Time Joint Audio-Video Generation by Parallel Adapter Composition](https://arxiv.org/abs/2610.10343v2)**  
  Authors: Jingyu Li, Xiaoxiao Xiang, Yiwen Guo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.10343v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://pac-demo-2027.github.io/demo/) | [![Demo](https://img.shields.io/badge/-Demo-brightgreen)](https://pac-demo-2027.github.io/demo)  
  Keywords: interactive, dit, video diffusion, video generation, streaming, autoregressive, diffusion transformer  
- **[OmniCam: Omni-Camera Trajectory Generation via Geometry-Grounded Pose Token Learning](https://arxiv.org/abs/2610.09513v1)**  
  Authors: Zhenyang Liu, Chenjie Cao, Yisu Zhang, Xuhui Zuo, Xiangyang Xue, Yanwei Fu, Tengfei Wang, Chunchao Guo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.09513v1.pdf)  
  Keywords: dit, trajectory, video generation, autoregressive, evaluation  
- **[SPW-Nav: A Streaming Panoramic World Model for Language-Guided Navigation](https://arxiv.org/abs/2610.08941v1)**  
  Authors: Yunheng Liu, Ziqi Cai, Siqi Yang, Yimu Wang, Minggui Teng, Jiaming Tan, Shuchen Weng, Erwin Wu, Kaipeng Zhang, Boxin Shi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.08941v1.pdf)  
  Keywords: interactive, dit, video generation, streaming, world model  
- **[S2PD: Serial-to-Parallel Diffusion for Physically and Logically Consistent Video Generation](https://arxiv.org/abs/2610.06847v1)**  
  Authors: Jeffrey Hu, Daniel Olmeda Reino, Ayush Tewari  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.06847v1.pdf)  
  Keywords: architecture, physical, video diffusion, diffusion model, video generation, physical simulation, autoregressive, diffusion transformer, simulation  

### Personalization & Customization

*Showing the latest 50 out of 64 papers*

- **[LEGO: A Lifting-Free Approach for Exocentric-to-Egocentric Video Generation](https://arxiv.org/abs/2610.12442v1)**  
  Authors: Suhwan Cho, Yonwoo Choi, Soongjin Kim, Jicheol Park, Taegyu Lim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.12442v1.pdf)  
  Keywords: dit, style, video diffusion, layout, diffusion model, video generation, denoising, novel view  
- **[Expression-Diverse References for Identity-Preserving Video Generation](https://arxiv.org/abs/2610.11023v1)**  
  Authors: Tianwen Fu, Wenbin Teng, Gonglin Chen, Junyi Ouyang, Haolin Xiong, Yajie Zhao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.11023v1.pdf)  
  Keywords: dit, benchmark, video generation, identity, evaluation  
- **[AdSpark: A Large-Scale Dataset and Benchmark for Product-Centric Advertisement Video Generation](https://arxiv.org/abs/2610.10047v1)**  
  Authors: Zhifei Yang, Zhao Jiang, Keyang Lu, Honghe Zhu, Zheng Zhang, Jingjing Lv, Changping Peng, Ching Law, Zhen Xiao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.10047v1.pdf)  
  Keywords: creative, benchmark, video generation, identity, evaluation  
- **[Rethinking Visual Provenance: Detection and Watermarking Across Direct Visual Generation and LLM-Driven Code Rendering](https://arxiv.org/abs/2610.08137v1)**  
  Authors: Zheng Gao, Xiaoyu Li, Zhicheng Bao, Yang Song, Jiaojiao Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.08137v1.pdf)  
  Keywords: video generation, concept  
- **[Diverse Motion Customization via Control-based Dynamic Optimization](https://arxiv.org/abs/2610.07911v2)**  
  Authors: Youngyoon Choi, Kihyun Kim, Jeongwoo Shin, Joonseok Lee  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.07911v2.pdf)  
  Keywords: video generation, customization, dit, dynamics  
- **[Your Unlearning Gives You Away: Identifying Erased Concepts in Diffusion Models](https://arxiv.org/abs/2610.05601v1)**  
  Authors: Kaiyuan Deng, Yuchen Li, Yang Xiao, Bo Hui, Geng Yuan, Xiaolong Ma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.05601v1.pdf)  
  Keywords: text-to-video, concept, efficient, diffusion model  
- **[Generating the Wild: Individual-Consistent Image-to-Video Generation for Wildlife](https://arxiv.org/abs/2610.05587v1)**  
  Authors: Yuzhuo Li, Di Zhao, Xinyu Zhang, Daniel Wilson, Yun Sing Koh  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.05587v1.pdf)  
  Keywords: dit, i2v, layout, video generation, motion control, identity, image-to-video, evaluation  
- **[PixReenact: Pixel-Conditioned Causal Video Diffusion for Streaming Head-Avatar Reenactment](https://arxiv.org/abs/2610.05233v1)**  
  Authors: Gavriel Habib, Dvir Samuel, Or Shimshi, Rami Ben-Ari  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.05233v1.pdf)  
  Keywords: dit, video diffusion, distillation, benchmark, streaming, autoregressive, denoising, identity, avatar  
- **[SemCam: Semantic Camera Motion Control for Video Generation](https://arxiv.org/abs/2610.05141v1)**  
  Authors: Janna Bruner, Omer Talmi, Ianir Ideses, Lior Fritz, Lior Wolf, Sagie Benaim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.05141v1.pdf)  
  Keywords: dit, trajectory, video-to-video, benchmark, video generation, motion control, identity  
- **[FADE: Frame-Aware Diffusion-Transformer-based Multi-Concept Erasure for Video Unlearning](https://arxiv.org/abs/2610.03980v1)**  
  Authors: Yuchen Li, Kaiyuan Deng, Chaoran Feng, Zhenyu Tang, Li Yuan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03980v1.pdf)  
  Keywords: dit, style, diffusion model, concept, benchmark, text-to-video, denoising, t2v  

### Physical Understanding

*Showing the latest 50 out of 137 papers*

- **[Pumpire: Unified Benchmark for Metric Distance Estimation](https://arxiv.org/abs/2610.12423v1)**  
  Authors: Siyu Chen, Zehan Wang, Jiayang Xu, Yihan Wu, Jialei Wang, Junming Chen, Ziang Zhang, Yutong Ying, Zhou Zhao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.12423v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://pumpire.github.io)  
  Keywords: evaluation, physical, benchmark  
- **[WorldAlign: Decoupled 4D Reward for World-Consistent Video Generation](https://arxiv.org/abs/2610.12382v1)**  
  Authors: Jing He, Kaixin Ding, Xingye Tian, Guibao Shen, Wenhang Ge, Xin Tao, Pengfei Wan, Ying-Cong Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.12382v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://worldalign.github.io)  
  Keywords: physical, video generation, simulation, image-to-video, evaluation  
- **[Phase-aware video generation for physics-grounded dynamics and interactions](https://arxiv.org/abs/2610.11791v1)**  
  Authors: Jingfeng Ou, Kun Wang, Rui Zhao, Jingwei Guan, Limin Wang, Chao Dong, Xingyu Zeng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.11791v1.pdf)  
  Keywords: architecture, physical, video generation, simulation, physics, dynamics, evaluation  
- **[Memory Forcing: Attendable Mid-Horizon History for Streaming Video Generation](https://arxiv.org/abs/2610.11756v1)**  
  Authors: Jiaming Zhang, Xinyu Wang, Huafeng Shi, Gangshan Wu, Limin Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.11756v1.pdf)  
  Keywords: physical, video diffusion, video generation, streaming, autoregressive  
- **[4-Tensor Attention Model for Semantic Physical Reality](https://arxiv.org/abs/2610.11716v1)**  
  Authors: Jongwook Kim, Sangheon Yun  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.11716v1.pdf)  
  Keywords: video generation, physical  
- **[Rewiring Semantics, Dynamics, and Control: A Simple yet Effective Action-Centric Tri-Stream Transformer](https://arxiv.org/abs/2610.11416v1)**  
  Authors: Shuang Luo, Yilun Kong, Yunpeng Qing, Yihang Jiao, Zhi Hou, Shunyu Liu, Xiaogang Wang, Dacheng Tao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.11416v1.pdf)  
  Keywords: physical, dynamics, benchmark, world model  
- **[TKCAM: Text and Keyframe to Camera Trajectory Generation](https://arxiv.org/abs/2610.11105v1)**  
  Authors: Haozhe Yang, Zhiyang Dou, Zekai Gu, Cheng Lin, Wenping Wang, Yuan Liu, Taku Komura  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.11105v1.pdf) | [![GitHub](https://img.shields.io/github/stars/linearalgebrayhz/TKCAM?style=social)](https://github.com/linearalgebrayhz/TKCAM)  
  Keywords: architecture, dit, trajectory, benchmark, video synthesis, dynamics, evaluation, controllable  
- **[Fluid-Gen-Zero: Grounding Pretrained Video Generators in Physics without Training](https://arxiv.org/abs/2610.10984v1)**  
  Authors: Hong Huang, Yuqiu Liu, Chenyu You, Daniel Martin, Chuhang Zou, Wuyang Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.10984v1.pdf)  
  Keywords: physical, trajectory, benchmark, video generation, denoising, simulation, physics, dynamics, physics-aware  
- **[Self-correction Optimization for Interleaved Multimodal Generation](https://arxiv.org/abs/2610.10400v1)**  
  Authors: Xin You, Zhiwei Ning, Zukai Chen, Minghui Zhang, Xuanke Shi, Hanxiao Zhang, Jingsong Liu, Jie Yang, Quan Wang, Yun Gu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.10400v1.pdf)  
  Keywords: temporal consistency, physical, dit, benchmark, video generation  
- **[Do Generative Priors Align with Human Naturalness Perception?](https://arxiv.org/abs/2610.09928v1)**  
  Authors: Taiki Fukiage  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.09928v1.pdf)  
  Keywords: physical, denoising  

### Surveys & Benchmarks

*Showing the latest 50 out of 252 papers*

- **[Pumpire: Unified Benchmark for Metric Distance Estimation](https://arxiv.org/abs/2610.12423v1)**  
  Authors: Siyu Chen, Zehan Wang, Jiayang Xu, Yihan Wu, Jialei Wang, Junming Chen, Ziang Zhang, Yutong Ying, Zhou Zhao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.12423v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://pumpire.github.io)  
  Keywords: evaluation, physical, benchmark  
- **[OneSearch-VL: Unified Multimodal Deep Research Agent for Image and Video](https://arxiv.org/abs/2610.12419v1)**  
  Authors: Hongyu Li, Manyuan Zhang, Kaituo Feng, Shu Chen, Dian Zheng, Hao Li, Hao Yu, Zhangquan Chen, Zoey Guo, Ray Zhang, Shaofei Huang, Tianrui Hui, Linjiang Huang, Si Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.12419v1.pdf) | [![GitHub](https://img.shields.io/github/stars/appletea233/OneSearch-VL?style=social)](https://github.com/appletea233/OneSearch-VL)  
  Keywords: evaluation, benchmark  
- **[SpaceCast-Bench: Evaluating Predictive Spatial Reasoning in Vision-Language Models](https://arxiv.org/abs/2610.12402v1)**  
  Authors: Hongxing Li, Jinyue Su, Dingming Li, Wenqi Zhang, Weiming Lu, Jun Xiao, Yueting Zhuang, Yongliang Shen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.12402v1.pdf)  
  Keywords: benchmark  
- **[WorldAlign: Decoupled 4D Reward for World-Consistent Video Generation](https://arxiv.org/abs/2610.12382v1)**  
  Authors: Jing He, Kaixin Ding, Xingye Tian, Guibao Shen, Wenhang Ge, Xin Tao, Pengfei Wan, Ying-Cong Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.12382v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://worldalign.github.io)  
  Keywords: physical, video generation, simulation, image-to-video, evaluation  
- **[Phase-aware video generation for physics-grounded dynamics and interactions](https://arxiv.org/abs/2610.11791v1)**  
  Authors: Jingfeng Ou, Kun Wang, Rui Zhao, Jingwei Guan, Limin Wang, Chao Dong, Xingyu Zeng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.11791v1.pdf)  
  Keywords: architecture, physical, video generation, simulation, physics, dynamics, evaluation  
- **[From Video Clips to Creation Trajectory: Sora100K for AI-Native Video Creation](https://arxiv.org/abs/2610.11770v1)**  
  Authors: Sicong Yang, Ruihuan Yang, Jian Lu, Jianfei Yuan, Xiaodong Cun, Xiuli Bi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.11770v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://huggingface.co/datasets/ysicong/Sora100K.) | [![Dataset](https://img.shields.io/badge/-Dataset-orange)](https://huggingface.co/datasets/ysicong/Sora100K)  
  Keywords: dit, trajectory, video editing, video generation, text-to-video, evaluation  
- **[Towards Unified Evaluation of Prompt Enhancers for Video Generation](https://arxiv.org/abs/2610.11736v1)**  
  Authors: Yawen Shao, Yubo Zhu, Ziyun Dai, Zixun Fang, Kai Zhu, Zeyinzi Jiang, Yufeng Ai, Siyang Sun, Haolan Xue, Yu Shang, Yuxiang Bao, Zoubin Bi, Jingming Luo, Jie Xiao, Chaojie Mao, Zhehan Kan, Hongchen Luo, Yu Liu, Sheng Zhong, Wei Tong, Xueyang Fu, Yang Cao, Wei Zhai, Zheng-Jun Zha  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.11736v1.pdf)  
  Keywords: dit, benchmark, video generation, text-to-video, image-to-video, evaluation  
- **[Parametric Trajectory Distillation for Few-Step Video Generation](https://arxiv.org/abs/2610.11498v1)**  
  Authors: Lan Feng, Peter Karkus, Maximilian Igl, Julius Berner, Yuxiao Chen, Shuhan Tan, Alexandre Alahi, Boris Ivanovic, Marco Pavone  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.11498v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://alan-lanfeng.github.io/PTD)  
  Keywords: architecture, video diffusion, trajectory, distillation, video generation, evaluation  
- **[Generative Adversarial Loops](https://arxiv.org/abs/2610.11458v1)**  
  Authors: Kislay Aditya Oj, Nidhi Jain, Sri Surya Varma Datla, Priyanka Jayaswal, Kumar Krishna Agrawal, Aditya Desai  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.11458v1.pdf)  
  Keywords: video generation, efficient, benchmark  
- **[Rewiring Semantics, Dynamics, and Control: A Simple yet Effective Action-Centric Tri-Stream Transformer](https://arxiv.org/abs/2610.11416v1)**  
  Authors: Shuang Luo, Yilun Kong, Yunpeng Qing, Yihang Jiao, Zhi Hou, Shunyu Liu, Xiaogang Wang, Dacheng Tao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.11416v1.pdf)  
  Keywords: physical, dynamics, benchmark, world model  

### Text-to-Video Generation

*Showing the latest 50 out of 57 papers*

- **[VEDJE: Video-Efficient Discriminative Joint Encoder for Scalable Video-Text Retrieval](https://arxiv.org/abs/2610.11850v1)**  
  Authors: Shahaf Wagner, Gabriele Serussi, Dan Ben Ami, Tomer Galanti, Chaim Baskin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.11850v1.pdf)  
  Keywords: text-to-video, efficient  
- **[From Video Clips to Creation Trajectory: Sora100K for AI-Native Video Creation](https://arxiv.org/abs/2610.11770v1)**  
  Authors: Sicong Yang, Ruihuan Yang, Jian Lu, Jianfei Yuan, Xiaodong Cun, Xiuli Bi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.11770v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://huggingface.co/datasets/ysicong/Sora100K.) | [![Dataset](https://img.shields.io/badge/-Dataset-orange)](https://huggingface.co/datasets/ysicong/Sora100K)  
  Keywords: dit, trajectory, video editing, video generation, text-to-video, evaluation  
- **[Towards Unified Evaluation of Prompt Enhancers for Video Generation](https://arxiv.org/abs/2610.11736v1)**  
  Authors: Yawen Shao, Yubo Zhu, Ziyun Dai, Zixun Fang, Kai Zhu, Zeyinzi Jiang, Yufeng Ai, Siyang Sun, Haolan Xue, Yu Shang, Yuxiang Bao, Zoubin Bi, Jingming Luo, Jie Xiao, Chaojie Mao, Zhehan Kan, Hongchen Luo, Yu Liu, Sheng Zhong, Wei Tong, Xueyang Fu, Yang Cao, Wei Zhai, Zheng-Jun Zha  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.11736v1.pdf)  
  Keywords: dit, benchmark, video generation, text-to-video, image-to-video, evaluation  
- **[iCATS: Fast Video Generation via Interaction-Aware Sparse Attention and Timestep-Adaptive Sparsity](https://arxiv.org/abs/2610.11302v1)**  
  Authors: Chengfeng Han, Baole Ai, Xianlu Bian, Jie Yao, Zilong Huang, Ang Wang, Dandan Ding  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.11302v1.pdf)  
  Keywords: dit, efficient, video generation, diffusion transformer, denoising, acceleration, t2v  
- **[TasteRoute: Personalized Routing for Video Generation](https://arxiv.org/abs/2610.05896v1)**  
  Authors: Zhi Rui Tam, Chao-Chung Wu, Sin-Han Yang, Peyton Ku, Brendan Kuang, Tzu-Ting Hsieh, Min-Fang Hsu, Fang-Ling Tsai, Yun-Nung Chen, Wei-Chiu Ma, Chieh-Yen Lin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.05896v1.pdf)  
  Keywords: video generation, efficient, text-to-video, image-to-video  
- **[Your Unlearning Gives You Away: Identifying Erased Concepts in Diffusion Models](https://arxiv.org/abs/2610.05601v1)**  
  Authors: Kaiyuan Deng, Yuchen Li, Yang Xiao, Bo Hui, Geng Yuan, Xiaolong Ma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.05601v1.pdf)  
  Keywords: text-to-video, concept, efficient, diffusion model  
- **[FADE: Frame-Aware Diffusion-Transformer-based Multi-Concept Erasure for Video Unlearning](https://arxiv.org/abs/2610.03980v1)**  
  Authors: Yuchen Li, Kaiyuan Deng, Chaoran Feng, Zhenyu Tang, Li Yuan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03980v1.pdf)  
  Keywords: dit, style, diffusion model, concept, benchmark, text-to-video, denoising, t2v  
- **[VDOT++: Unified Few-Step Video Generation via Unbalanced Optimal Transport Distillation](https://arxiv.org/abs/2610.03221v1)**  
  Authors: Yutong Wang, Xingtong Ge, Enhuai Liu, Yunke Wang, Tianfan Xue, Yu Qiao, Yaohui Wang, Xinyuan Chen, Chang Xu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03221v1.pdf)  
  Keywords: dit, i2v, video diffusion, distillation, diffusion model, benchmark, video generation, text-to-video, image-to-video, t2v  
- **[Parasitic Co-Denoising: Unlocking 3D Human Motion Generation in a Frozen Video Diffusion Model](https://arxiv.org/abs/2610.03047v1)**  
  Authors: Yunjiao Zhou, Junlang Qian, Lihua Xie, Jianfei Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03047v1.pdf)  
  Keywords: human motion, efficient, video diffusion, diffusion model, text-to-video, denoising  
- **[DMAD: Distribution Matching as Adversarial Distillation for Fast Visual Generation](https://arxiv.org/abs/2610.02188v1)**  
  Authors: Zhengming Yu, Junkun Yuan, Haotian Yang, Gordon Guocheng Qian, Yizhi Wang, Angtian Wang, Yiding Yang, Bo Liu, Xin Li, Wenping Wang, Chongyang Ma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.02188v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://yzmblog.github.io/projects/DMAD)  
  Keywords: distillation, diffusion model, video generation, identity, t2v  

### Video Editing

- **[VINCIE-NExT: Unlocking Video Editing from Images via In-Context Modeling](https://arxiv.org/abs/2610.12104v1)**  
  Authors: Leigang Qu, Feng Cheng, Ziyan Yang, Bangbang Yang, Zhaoyang Huang, Wei Chow, Yicong Li, Wenjie Wang, Tat-Seng Chua, Yan Zeng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.12104v1.pdf)  
  Keywords: video editing, dit  
- **[From Video Clips to Creation Trajectory: Sora100K for AI-Native Video Creation](https://arxiv.org/abs/2610.11770v1)**  
  Authors: Sicong Yang, Ruihuan Yang, Jian Lu, Jianfei Yuan, Xiaodong Cun, Xiuli Bi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.11770v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://huggingface.co/datasets/ysicong/Sora100K.) | [![Dataset](https://img.shields.io/badge/-Dataset-orange)](https://huggingface.co/datasets/ysicong/Sora100K)  
  Keywords: dit, trajectory, video editing, video generation, text-to-video, evaluation  
- **[Transforming Image Editors into Video Editors](https://arxiv.org/abs/2610.11037v1)**  
  Authors: Feng Wang, Zijie Li, Ceyuan Yang, Alan Yuille, Peng Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.11037v1.pdf) | [![GitHub](https://img.shields.io/github/stars/wangf3014/AVE?style=social)](https://github.com/wangf3014/AVE)  
  Keywords: temporal consistency, dit, video diffusion, diffusion model, video editing, image-to-video  
- **[SemCam: Semantic Camera Motion Control for Video Generation](https://arxiv.org/abs/2610.05141v1)**  
  Authors: Janna Bruner, Omer Talmi, Ianir Ideses, Lior Fritz, Lior Wolf, Sagie Benaim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.05141v1.pdf)  
  Keywords: dit, trajectory, video-to-video, benchmark, video generation, motion control, identity  
- **[Unsupervised Domain Adaptation for Enhanced Radiometer Image Precipitation Estimation using Conditional Flow Matching](https://arxiv.org/abs/2610.01890v1)**  
  Authors: Victor Enescu, Assaad Zeghina, Matthieu Meignin, Nicolas Viltard, Cécile Mallet  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.01890v1.pdf)  
  Keywords: video editing, dit, flow matching  
- **[ViTeX-Bench: Benchmarking High-Fidelity Video Scene Text Editing](https://arxiv.org/abs/2609.40356v1)**  
  Authors: Xinghao Chen, Xiangbo Gao, Jiongze Yu, Yuheng Wu, Zhengzhong Tu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.40356v1.pdf)  
  Keywords: temporal consistency, dit, benchmark, video editing, video generation, dynamics, evaluation, controllable  
- **[Diffusion Editing with Soft Mask: Pixel Level Redo of Image and Video with Adjustable Strength](https://arxiv.org/abs/2610.00359v1)**  
  Authors: Candi Zheng, Yuan Lan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.00359v1.pdf)  
  Keywords: dit, efficient, video diffusion, diffusion model, video editing  
- **[Counterfactual Video Generation Enables Scalable Humanoid Loco-Manipulation](https://arxiv.org/abs/2609.38172v1)**  
  Authors: Zihan Wang, Zhen Wu, Pieter Abbeel, Rocky Duan, Jitendra Malik, Carmelo Sferrazza, C. Karen Liu, Guanya Shi, Angjoo Kanazawa  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.38172v1.pdf)  
  Keywords: video generation, physical, video-to-video  
- **[VideoPhysEdit: Physical Counterfactual Video Editing via Rigid-Body Physical Scene Reconstruction](https://arxiv.org/abs/2609.35134v1)**  
  Authors: Conghan Yue, Yuanjie Chen, Yue Han, Ya Gao, Yunyan Xiao, WeiYao Zhang, Zhineng Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.35134v1.pdf) | [![GitHub](https://img.shields.io/github/stars/Hammour-steak/VideoPhysEdit?style=social)](https://github.com/Hammour-steak/VideoPhysEdit)  
  Keywords: physical, dit, benchmark, video editing, video generation, simulation, physics, evaluation  
- **[Enhanced Video Text Editing with Trajectory-Aligned Glyph Rendering](https://arxiv.org/abs/2609.34178v2)**  
  Authors: Shulian Zhang, Xiangyu Shu, Wenbo Li, Jian Chen, Yong Guo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.34178v2.pdf)  
  Keywords: dit, video diffusion, trajectory, diffusion model, benchmark, video editing  

### Video Inpainting & Completion

- **[WorldWeave: Growing Persistent Geometric Worlds for Video Generation](https://arxiv.org/abs/2609.34221v2)**  
  Authors: Yifan Huang, Lifan Jiang, Qingyue Hao, Cheng Chen, Boxi Wu, Xiaoxue Ren, Xiaofei He, Dehai Zhao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.34221v2.pdf)  
  Keywords: dit, video generation, outpainting, video synthesis, world model  
- **[MT-WAM: Reorienting the One-Pass Predictive Representation Toward Action Generation](https://arxiv.org/abs/2609.21474v1)**  
  Authors: Yiguang Yang, Jiankun Peng, Xiaoming Wang, Yiran Zhang, Zhibo Fang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.21474v1.pdf)  
  Keywords: dit, video diffusion, video prediction, diffusion transformer, dynamics  
- **[StrucPhysVideo: Learning Physical Dynamics from Structured Captions and Robot Actions](https://arxiv.org/abs/2609.18430v1)**  
  Authors: Awomo-WM Team, :, Enhui Ma, Kaiwen Guo, Tingrui Zhang, Wei Song, Yingshui Tan, Jianhua Xu, Tong Zhang, Kaicheng Yu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.18430v1.pdf)  
  Keywords: interactive, physical, dit, i2v, action-conditioned, distillation, video prediction, autoregressive, denoising, physics, dynamics, image-to-video, world model  
- **[GeoLAM: Learning Geometry-Grounded Latent Actions from Unlabeled Human Videos](https://arxiv.org/abs/2609.17099v1)**  
  Authors: Yifan Xie, Hekun Tian, Jinkun Liu, YuAn Wang, Qiao Sun, Wenbo Ding  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.17099v1.pdf)  
  Keywords: trajectory, video prediction, benchmark, video generation, evaluation  
- **[AcrossVAM1.0: Particle World Modeling for Text-Assisted Robot Video Prediction](https://arxiv.org/abs/2608.28491v1)**  
  Authors: Yafei Zhang, Nan Wu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.28491v1.pdf)  
  Keywords: film, trajectory, video prediction, benchmark, dynamics, world model  

### Video Super-Resolution & Enhancement

*Showing the latest 50 out of 75 papers*

- **[LEGO: A Lifting-Free Approach for Exocentric-to-Egocentric Video Generation](https://arxiv.org/abs/2610.12442v1)**  
  Authors: Suhwan Cho, Yonwoo Choi, Soongjin Kim, Jicheol Park, Taegyu Lim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.12442v1.pdf)  
  Keywords: dit, style, video diffusion, layout, diffusion model, video generation, denoising, novel view  
- **[iCATS: Fast Video Generation via Interaction-Aware Sparse Attention and Timestep-Adaptive Sparsity](https://arxiv.org/abs/2610.11302v1)**  
  Authors: Chengfeng Han, Baole Ai, Xianlu Bian, Jie Yao, Zilong Huang, Ang Wang, Dandan Ding  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.11302v1.pdf)  
  Keywords: dit, efficient, video generation, diffusion transformer, denoising, acceleration, t2v  
- **[Fluid-Gen-Zero: Grounding Pretrained Video Generators in Physics without Training](https://arxiv.org/abs/2610.10984v1)**  
  Authors: Hong Huang, Yuqiu Liu, Chenyu You, Daniel Martin, Chuhang Zou, Wuyang Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.10984v1.pdf)  
  Keywords: physical, trajectory, benchmark, video generation, denoising, simulation, physics, dynamics, physics-aware  
- **[GRACE: Generation-aware latent compression for efficient video generation](https://arxiv.org/abs/2610.10524v1)**  
  Authors: Jiyoung Kim, Paul Hyunbin Cho, Jisu Nam, Donghoon Lee, Hyunsung Go, Yeonkyeong Lee, Hansaem Kim, Seungryong Kim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.10524v1.pdf)  
  Keywords: dit, efficient, i2v, video diffusion, diffusion model, video generation, diffusion transformer, denoising  
- **[MORCA: Offline-to-Online Reinforcement Learning for Adaptive Cache Reuse in Video Diffusion Acceleration](https://arxiv.org/abs/2610.10457v1)**  
  Authors: Yuxiang Xiong, Ruiyan Wang, Wenqiang Wang, Teng Hu, Songhang Shen, Bohao Feng, Hongqian Deng, Ran Yi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.10457v1.pdf) | [![GitHub](https://img.shields.io/github/stars/x10ngyx/MORCA?style=social)](https://github.com/x10ngyx/MORCA)  
  Keywords: dit, video diffusion, video generation, diffusion transformer, denoising, video synthesis, acceleration  
- **[SGF+: Decoupling Gradient Flows for Autoregressive Video Generation](https://arxiv.org/abs/2610.10429v2)**  
  Authors: Zihan Su, Junhao Zhuang, Yaowei Li, Siwen Lu, Haoran Li, Lingen Li, Haoyu Wu, Weiyang Jin, Songchun Zhang, Haoyang Huang, Chun Yuan, Zeyue Xue, Nan Duan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.10429v2.pdf)  
  Keywords: temporal consistency, dit, video generation, autoregressive, denoising  
- **[Do Generative Priors Align with Human Naturalness Perception?](https://arxiv.org/abs/2610.09928v1)**  
  Authors: Taiki Fukiage  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.09928v1.pdf)  
  Keywords: physical, denoising  
- **[RealtimeWAM: One-Step Asynchronous World Action Models](https://arxiv.org/abs/2610.06617v1)**  
  Authors: Chengtao Lv, Jinyang Du, Shuyi Feng, Yang Yong, Shiqiao Gu, Shunzi Yang, Ruihao Gong, Shen Ren, Tianwei Zhang, Wenya Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.06617v1.pdf) | [![GitHub](https://img.shields.io/github/stars/ModelTC/LightX2V?style=social)](https://github.com/ModelTC/LightX2V)  
  Keywords: architecture, dit, efficient, distillation, benchmark, video generation, denoising  
- **[Keepsake: Selective Spatial Memory for Long-Horizon Video Generation](https://arxiv.org/abs/2610.06588v1)**  
  Authors: Abdul Mohaimen Al Radi, Kunyang Li, Yuzhang Shang, Mubarak Shah, Yu Tian  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.06588v1.pdf)  
  Keywords: video generation, denoising  
- **[Level-of-Token Diffusion](https://arxiv.org/abs/2610.05816v1)**  
  Authors: Kiyohiro Nakayama, Brian Chao, Jan Ackermann, Hansheng Chen, Federico Tombari, Leonidas Guibas, Lior Yariv, Gordon Wetzstein  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.05816v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://georgenakayama.github.io/lotdiffusion)  
  Keywords: efficient, video diffusion, layout, diffusion model, video generation, diffusion transformer, denoising  

### World Models & Simulation

*Showing the latest 50 out of 109 papers*

- **[WorldGuide: Goal-Directed Video World Model for Procedural Task Execution](https://arxiv.org/abs/2610.12459v1)**  
  Authors: Ankan Deria, Komal Kumar, Hisham Cholakkal, Fahad Shahbaz Khan, Salman Khan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.12459v1.pdf)  
  Keywords: video generation, dit, world model  
- **[WorldCast: Distributed Multiplayer World Models](https://arxiv.org/abs/2610.12412v1)**  
  Authors: Ziyang Ye, Junchao Huang, Evelyn Zhang, Zhihao Xie, Ruicheng Zhang, Boyao Han, Litao Ban, Ziye Wang, Xinting Hu, Shaoshuai Shi, Zhuotao Tian, Li Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.12412v1.pdf)  
  Keywords: dit, world model  
- **[WorldAlign: Decoupled 4D Reward for World-Consistent Video Generation](https://arxiv.org/abs/2610.12382v1)**  
  Authors: Jing He, Kaixin Ding, Xingye Tian, Guibao Shen, Wenhang Ge, Xin Tao, Pengfei Wan, Ying-Cong Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.12382v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://worldalign.github.io)  
  Keywords: physical, video generation, simulation, image-to-video, evaluation  
- **[Phase-aware video generation for physics-grounded dynamics and interactions](https://arxiv.org/abs/2610.11791v1)**  
  Authors: Jingfeng Ou, Kun Wang, Rui Zhao, Jingwei Guan, Limin Wang, Chao Dong, Xingyu Zeng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.11791v1.pdf)  
  Keywords: architecture, physical, video generation, simulation, physics, dynamics, evaluation  
- **[Conditional Residual Prediction: Improving Autoregressive Video Diffusion without a Bidirectional Teacher](https://arxiv.org/abs/2610.11479v1)**  
  Authors: Bowen Zheng, Zhiguang Liu, Jiarong Ou, Rui Chen, Tianyang Hu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.11479v1.pdf)  
  Keywords: interactive, dit, video diffusion, distillation, diffusion model, video generation, streaming, autoregressive  
- **[Rewiring Semantics, Dynamics, and Control: A Simple yet Effective Action-Centric Tri-Stream Transformer](https://arxiv.org/abs/2610.11416v1)**  
  Authors: Shuang Luo, Yilun Kong, Yunpeng Qing, Yihang Jiao, Zhi Hou, Shunyu Liu, Xiaogang Wang, Dacheng Tao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.11416v1.pdf)  
  Keywords: physical, dynamics, benchmark, world model  
- **[WAM-Cache: Staleness-Bounded KV Reuse for Efficient World Action Models](https://arxiv.org/abs/2610.11401v1)**  
  Authors: Kai Ding, Yang He, Ruijie Quan, Yi Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.11401v1.pdf)  
  Keywords: dit, efficient, video diffusion, diffusion transformer, simulation, acceleration  
- **[IntactWorld: Joint World Modeling with Intact Features](https://arxiv.org/abs/2610.11174v1)**  
  Authors: Boming Tan, Xiangdong Zhang, Yan Xia, Qi Zhu, Deyi Ji, Xue Yang, Shaofeng Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.11174v1.pdf)  
  Keywords: architecture, efficient, benchmark, video generation, evaluation, world model  
- **[Fluid-Gen-Zero: Grounding Pretrained Video Generators in Physics without Training](https://arxiv.org/abs/2610.10984v1)**  
  Authors: Hong Huang, Yuqiu Liu, Chenyu You, Daniel Martin, Chuhang Zou, Wuyang Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.10984v1.pdf)  
  Keywords: physical, trajectory, benchmark, video generation, denoising, simulation, physics, dynamics, physics-aware  
- **[Real-Time Joint Audio-Video Generation by Parallel Adapter Composition](https://arxiv.org/abs/2610.10343v2)**  
  Authors: Jingyu Li, Xiaoxiao Xiang, Yiwen Guo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.10343v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://pac-demo-2027.github.io/demo/) | [![Demo](https://img.shields.io/badge/-Demo-brightgreen)](https://pac-demo-2027.github.io/demo)  
  Keywords: interactive, dit, video diffusion, video generation, streaming, autoregressive, diffusion transformer  



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
