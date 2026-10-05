# Awesome Video Diffusions [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of latest research papers, projects and resources related to Video Diffusion Models and Video Generation. Content is automatically updated daily.

> Last Update: 2026-10-05 04:07:42

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
- [Applications](#applications) (37 papers) - Domain-specific applications of video diffusion models
- [Architecture & Efficiency](#architecture-&-efficiency) (346 papers) - Architectural innovations (DiT, UNet), flow matching, and training/inference efficiency
- [Audio & Multi-modal](#audio-&-multi-modal) (26 papers) - Audio-driven and multi-modal conditioned video generation
- [Controllable Generation](#controllable-generation) (116 papers) - Controllable video generation with motion, camera, pose, or layout guidance
- [Human & Character Animation](#human-&-character-animation) (18 papers) - Human-centric video generation including talking heads, dance, and character animation
- [Image-to-Video Generation](#image-to-video-generation) (34 papers) - Methods for animating still images into videos
- [Long Video Generation](#long-video-generation) (111 papers) - Generating temporally consistent long-form videos beyond short clips
- [Personalization & Customization](#personalization-&-customization) (65 papers) - Personalized video generation with custom subjects, identities, or styles
- [Physical Understanding](#physical-understanding) (129 papers) - Physics-aware video generation and dynamics modeling
- [Surveys & Benchmarks](#surveys-&-benchmarks) (249 papers) - Survey papers, benchmarks, and evaluation metrics for video generation
- [Text-to-Video Generation](#text-to-video-generation) (63 papers) - Foundation models and methods for generating videos from text prompts
- [Video Editing](#video-editing) (17 papers) - Diffusion-based video editing, style transfer, and manipulation
- [Video Inpainting & Completion](#video-inpainting-&-completion) (9 papers) - Video inpainting, completion, outpainting, and temporal prediction
- [Video Super-Resolution & Enhancement](#video-super-resolution-&-enhancement) (82 papers) - Video quality improvement, upscaling, restoration, and frame interpolation
- [World Models & Simulation](#world-models-&-simulation) (103 papers) - Video generation as world simulators and interactive environment generation



## Table of Contents

- [Categorized Papers](#categorized-papers)
- [Classic Papers](#classic-papers)
- [Open Source Projects](#open-source-projects)
- [Applications](#applications)
- [Tutorials & Blogs](#tutorials--blogs)





## Categorized Papers

### 3D-aware Video Generation

- **[GeoVerse: World-Consistent Novel View Synthesis in Geometric Latent Space](https://arxiv.org/abs/2609.35734v2)**  
  Authors: Kerui Ren, Tao Lu, Linning Xu, Changjian Jiang, Mu Huang, Chunhua Shen, Mulin Yu, Bo Dai  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.35734v2.pdf)  
  Keywords: novel view, diffusion model, style  
- **[GenNVS: Geometry-enhanced Novel View Synthesis via Disentangled 3D Prior](https://arxiv.org/abs/2609.34579v2)**  
  Authors: Yajiao Xiong, Youyu Luan, Xiaoyu Zhou, Yongtao Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.34579v2.pdf)  
  Keywords: dit, diffusion model, novel view, video diffusion  
- **[VGGT-Diff: Visual Geometry Meets Diffusion for Sparse-View Novel View Synthesis](https://arxiv.org/abs/2609.33253v1)**  
  Authors: Kangjie Chen, Xiangyu Li, Dongbin Zhang, Chaoda Zheng, Shijia Chen, Jinhao Deng, Hongbin Lin, Choo Sin Wai, Minqi Wang, Minghao Yang, Dake Zhong, Guorui Song, Yu Zhang, Xianming Liu, Boyang Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.33253v1.pdf) | [![GitHub](https://img.shields.io/github/stars/chenkangjie1123/VGGT-Diff?style=social)](https://github.com/chenkangjie1123/VGGT-Diff)  
  Keywords: novel view, denoising, dit, video diffusion, diffusion model  
- **[WorldCrafter: Consistent Video World Model with Implicit 3D-aware Memory](https://arxiv.org/abs/2609.24984v1)**  
  Authors: Wangbo Yu, Kunhao Liu, Wenbo Hu, Shenghai Yuan, Chaoran Feng, Haiyang Zhou, Yukun Huang, Yiran Wang, Wang Zhao, Yingmin Luo, Ying Shan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.24984v1.pdf)  
  Keywords: 3d-aware, world model, denoising, interactive, dit, distillation, streaming  
- **[Printing the Underdetermined: Materializing Multi-solutionness in Figurative Paintings](https://arxiv.org/abs/2609.19782v2)**  
  Authors: Yutao Ming, Teng Xu, Youjia Wang, Yunyang Liu, Fengmin Yang, Fuqiang Zhao, Jingyi Yu, Hua Yang, Yanjun Zhou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.19782v2.pdf)  
  Keywords: physical, dit, multi-view video  
- **[Rethinking 3D Noise: Learning 3D-Aware Video Priors via Optimization-Free Morphological Perturbations](https://arxiv.org/abs/2609.03657v1)**  
  Authors: Onat Şahin, Mohammad Altillawi, George Eskandar, Carlos Carbone, Ziyuan Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.03657v1.pdf)  
  Keywords: robotics, video diffusion, 3d-aware  
- **[Stabilizing Camera-Controlled Novel View Synthesis at Inference Time](https://arxiv.org/abs/2609.03639v1)**  
  Authors: Prajwal Singh, Arjun Badola, Seema Kumari, Hajime Nagahara, Shanmuganathan Raman  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.03639v1.pdf)  
  Keywords: efficient, novel view, autoregressive, video diffusion, diffusion model  
- **[Building Pretraining Data for World Models: An Unreal Engine-Based Pipeline for Action-Conditioned Video Generation](https://arxiv.org/abs/2609.03557v1)**  
  Authors: Haoyu Wang, Songchun Zhang, Haoran Li, Haoyang Huang, Zeyue Xue, Nan Duan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.03557v1.pdf)  
  Keywords: action-conditioned, multi-view video, world model, architecture, dit, video generation, physics, trajectory  
- **[RoGe: Novel View Synthesis via End-to-End Implicit Reconstruction and Generation](https://arxiv.org/abs/2609.02847v3)**  
  Authors: Xiaolei Lang, Ze Kang, Zehao Huang, Naiyan Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.02847v3.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://jerry-locker.github.io/roge)  
  Keywords: novel view, dit, video diffusion, trajectory, diffusion model  
- **[Spatially Aware World Action Model via Geometric Latent Diffusion](https://arxiv.org/abs/2609.02531v1)**  
  Authors: Javier Alejandro Lopetegui Gonzalez, Paul Pacaud, Cordelia Schmid  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.02531v1.pdf)  
  Keywords: physical, evaluation, world model, video diffusion, benchmark, diffusion model, 3d-aware  

### Applications

- **[DiVid: Diagnosing Dimension-Specific Diversity Collapse in Video Generation Models](https://arxiv.org/abs/2610.01661v1)**  
  Authors: Huanran Hu, Zihui Ren, Dingyi Yang, Zhinan Song, Guozheng Wu, Tiezheng Ge, Qin Jin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.01661v1.pdf)  
  Keywords: controllable, evaluation, video generation, creative, style  
- **[PhysicsLENS: Diagnosing Physical Property Blindness in Video Generation Models](https://arxiv.org/abs/2610.01162v1)**  
  Authors: Isaiah Milkey, Som Sagar, Aditya Taparia, Xinyuan Liu, Jiqing Wen, Ransalu Senanayake  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.01162v1.pdf)  
  Keywords: evaluation, world model, video generation, dit, physics, robotics, benchmark, physical  
- **[Bootstrapping Video Interaction Generation with Synthetic State Transitions](https://arxiv.org/abs/2610.01039v1)**  
  Authors: Jiho Jang, Jinyoung Kim, Nojun Kwak, Kyungjune Kim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.01039v1.pdf)  
  Keywords: controllable, evaluation, dit, robotics, physical  
- **[Harnessing Vision-Language Models for Perceptual Quality Assessment and Autonomous Content Adjustment in Augmented Reality](https://arxiv.org/abs/2610.00677v1)**  
  Authors: Elias Rotondo, Lin Duan, Yanming Xiu, Sangjun Eom, Conrad Li, Maria Gorlatova  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.00677v1.pdf)  
  Keywords: evaluation, dit, education, benchmark  
- **[GroundingPI: A Grounding Foundation Model towards Physical Intelligence with Visual Primitives](https://arxiv.org/abs/2609.39601v1)**  
  Authors: Qize Yu, Lianrui Fan, Boyu Chen, Jiaqi Liang, Xini Ding, Yue Chen, Zetian Song, Yuran Wang, Yi Zou, Kaixuan Wang, Tianxing Chen, Wenxuan Song, Bohan Zhou, Mingleyang Li, Siqiao Huang, Yuqi Ye, Caigao Jiang, Wei Wei, Ruihai Wu, Hang Zhang, Yixiao Ge, Shuchang Zhou, Shilong Liu, Xianming Liu, Ping Luo, Shiyu Huang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.39601v1.pdf)  
  Keywords: autonomous driving, physical, benchmark  
- **[Exo2EgoHOI: Hand-Object-Interaction Aware Exocentric-to-Egocentric Video Generation](https://arxiv.org/abs/2609.38615v1)**  
  Authors: Hongjia Zhai, Xiyu Zhang, Haoran Zhang, Zhichao Ye, Haomin Liu, Guofeng Zhang, Ian Reid, Xingxing Zuo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.38615v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://rcl-robotics.github.io/Exo2EgoHOI)  
  Keywords: video generation, robotics  
- **[LongLive-Plug: Once-for-All Distillation for Video Generation](https://arxiv.org/abs/2609.38154v1)**  
  Authors: Shuai Yang, Luozhou Wang, Wei Huang, ZhiFei Chen, Bohan Zhang, Xiao Fu, Qianli Ma, Chen-Hsuan Lin, Weian Mao, Bryan Chu, Song Han, Yukang Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.38154v1.pdf)  
  Keywords: distillation, world model, video generation, autoregressive, dit, video diffusion, robotics, diffusion model  
- **[S4VY: Segment Anything in Feed-Forward 4D Visual Geometry](https://arxiv.org/abs/2609.36875v1)**  
  Authors: Jingdong Zhang, Xin Li, Jan Kautz, Wenping Wang, Chris Choy  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.36875v1.pdf)  
  Keywords: evaluation, identity, autonomous driving, dit, robotics  
- **[SkillPE: Creativity-Oriented Cinematic Skill Evolution for Text-to-Video Prompt Engineering](https://arxiv.org/abs/2609.34335v1)**  
  Authors: Yanwei Huang, Mingxuan Zhu, Shujie Li, Shiyuan Liu, Yuanxing Zhang, Arpit Narechania  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.34335v1.pdf) | [![GitHub](https://img.shields.io/github/stars/Ais0n/SkillPE?style=social)](https://github.com/Ais0n/SkillPE)  
  Keywords: text-to-video, evaluation, video generation, creative, benchmark, sound, film  
- **[REMEDY: How Far Is Video Generation from Medical Education World Models?](https://arxiv.org/abs/2609.32460v1)**  
  Authors: Lixing Tan, Yanghao Zhou, Qing Xia, Yuting Guo, Shuai Li, Aimin Hao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.32460v1.pdf)  
  Keywords: education, temporal consistency, evaluation, world model, medical, video generation, benchmark  

### Architecture & Efficiency

*Showing the latest 50 out of 346 papers*

- **[ProAR: Learning Prospective Reasoning with Autoregressive Video Models](https://arxiv.org/abs/2610.03664v1)**  
  Authors: Linghui Shen, Tinghui Zhu, Sheng Zhang, Muhao Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03664v1.pdf)  
  Keywords: efficient, video generation, autoregressive, benchmark, dynamics  
- **[LoGo: Local-Global Rewards for Consistent Long-Horizon Video Generation](https://arxiv.org/abs/2610.03636v1)**  
  Authors: Ziqi Ma, Shreya Sharma, Mohamed El Banani, Katja Schwarz, Chongjie Ye, Chao-Yuan Wu, Li Fei-Fei, Ben Mildenhall, Georgia Gkioxari, Justin Johnson, Gowthami Somepalli  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03636v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://ziqi-ma.github.io/logo-website)  
  Keywords: evaluation, camera control, video generation, dit, benchmark, trajectory  
- **[Rethinking What to Cache in Few-Step Diffusion Transformers: Solver-Aware Target Selection](https://arxiv.org/abs/2610.03577v1)**  
  Authors: Shuo Yang, Lihao Fang, Yi Zhang, Haixiang Wang, Xincheng Ye, Shufan Chen, Jipeng Guo, Youqing Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03577v1.pdf) | [![GitHub](https://img.shields.io/github/stars/wali1024-offical/AutoTarget?style=social)](https://github.com/wali1024-offical/AutoTarget)  
  Keywords: diffusion transformer, evaluation, dit, trajectory, distillation  
- **[DuoMatching: Joint-Marginal Distribution Matching for Few-Step Video Generation](https://arxiv.org/abs/2610.03543v1)**  
  Authors: Jiahao Zhan, Yan Wang, Yongrui Ma, Qunliang Xing, Ruchang Yao, Runtao Liu, Shijie Zhao, Tianfan Xue  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03543v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://johnzhan2023.github.io/DuoMatching)  
  Keywords: evaluation, video generation, autoregressive, dit, dynamics, distillation, streaming  
- **[XGenAct: Geometry-Enhanced World Action Models through Cross-Task Generation](https://arxiv.org/abs/2610.03516v1)**  
  Authors: Tingting Du, Ziyao Wang, Guoheng Sun, Ang Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03516v1.pdf)  
  Keywords: video diffusion, architecture, diffusion transformer  
- **[Weave Forcing: Compositional Memory Routing for Interactive Long Video Generation](https://arxiv.org/abs/2610.03510v1)**  
  Authors: Ziyi Wang, Junchi Yao, Heqian Qiu, Wenbo Shi, Chengjiu Wang, Jinyang He, Binkai Hong, Hongliang Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03510v1.pdf)  
  Keywords: temporal consistency, interactive, long video, video generation, autoregressive, dit  
- **[VDOT++: Unified Few-Step Video Generation via Unbalanced Optimal Transport Distillation](https://arxiv.org/abs/2610.03221v1)**  
  Authors: Yutong Wang, Xingtong Ge, Enhuai Liu, Yunke Wang, Tianfan Xue, Yu Qiao, Yaohui Wang, Xinyuan Chen, Chang Xu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03221v1.pdf)  
  Keywords: text-to-video, distillation, video generation, i2v, dit, video diffusion, benchmark, t2v, image-to-video, diffusion model  
- **[Contextual Flow Matching: Adaptive Step Selection in Flow Models for Efficient Visual Generation](https://arxiv.org/abs/2610.03202v1)**  
  Authors: Divya Jyoti Bajpai, Arun Verma, Manjesh Kumar Hanawal  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03202v1.pdf)  
  Keywords: efficient, evaluation, acceleration, video generation, dit, dynamics, flow matching  
- **[Does Physics Live in the Activations? Localizing Physical Quantities in Video Diffusion Models](https://arxiv.org/abs/2610.03154v1)**  
  Authors: Jonas Kneifl, Jakub Skalski, Bartłomiej Twardowski, Kamil Deja  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03154v1.pdf)  
  Keywords: physical, world model, denoising, video generation, dit, physics, video diffusion, benchmark, diffusion transformer, dynamics, diffusion model  
- **[In-Distribution Forcing for Long Video Generation at Test Time](https://arxiv.org/abs/2610.03120v1)**  
  Authors: Jeongwoo Shin, Youngyoon Choi, Sangwoo Jo, Hyunmog Kim, Sungjoon Choi, Joonseok Lee, Jaewoong Choi, Jaemoo Choi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03120v1.pdf)  
  Keywords: evaluation, long video, video generation, autoregressive, dit, video diffusion, benchmark, dynamics, diffusion model  

### Audio & Multi-modal

- **[AiSearch: Interactive Multi-Modal Search with VLMs](https://arxiv.org/abs/2610.01389v1)**  
  Authors: Ali Koksal, Mei Chee Leong, Vicky Sintunata, Ching Ling Chin, Wee Teck Fong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.01389v1.pdf)  
  Keywords: multi-modal, benchmark, interactive  
- **[Watch Your Speech: Text-aware Video-to-Speech Synthesis with Textual Conditioning](https://arxiv.org/abs/2610.01012v1)**  
  Authors: Gunwoo Lee, Yoori Oh, Yoseob Han  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.01012v1.pdf) | [![GitHub](https://img.shields.io/github/stars/gunwoo5034/Watch-your-Speech?style=social)](https://github.com/gunwoo5034/Watch-your-Speech)  
  Keywords: evaluation, dit, dynamics, sound, flow matching  
- **[Soundwich: Video Generation with Layered and Controllable Audio](https://arxiv.org/abs/2610.00691v2)**  
  Authors: Zhuo Ning, AmirHossein Naghi Razlighi, Sagi Polaczek, Daniel Cohen-Or, Ali Mahdavi-Amiri  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.00691v2.pdf) | [![GitHub](https://img.shields.io/github/stars/CodyNing/Soundwich?style=social)](https://github.com/CodyNing/Soundwich)  
  Keywords: controllable, evaluation, video generation, dit, sound  
- **[GLARE: Generating Listening Heads with Appropriate Reactions](https://arxiv.org/abs/2609.40317v1)**  
  Authors: Zikai Liao, Yumin Suh, Yi Ouyang, Yi-Lun Lee, Yi-Hsuan Tsai, Zhaozheng Yin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.40317v1.pdf)  
  Keywords: talking head, evaluation, audio-driven, video generation, dit  
- **[Enabling Immersive Audio-Visual Experience from Any Video](https://arxiv.org/abs/2609.36295v1)**  
  Authors: Zitong Lan, Mutian Tong, Jiatao Gu, Mingmin Zhao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.36295v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://huggingface.co/spaces/CuriousAlien000/spatial-audio-360-demo) | [![HuggingFace](https://img.shields.io/badge/-HuggingFace-yellow)](https://huggingface.co/spaces/CuriousAlien000/spatial-audio-360-demo)  
  Keywords: physics, video generation, sound, simulation  
- **[SkillPE: Creativity-Oriented Cinematic Skill Evolution for Text-to-Video Prompt Engineering](https://arxiv.org/abs/2609.34335v1)**  
  Authors: Yanwei Huang, Mingxuan Zhu, Shujie Li, Shiyuan Liu, Yuanxing Zhang, Arpit Narechania  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.34335v1.pdf) | [![GitHub](https://img.shields.io/github/stars/Ais0n/SkillPE?style=social)](https://github.com/Ais0n/SkillPE)  
  Keywords: text-to-video, evaluation, video generation, creative, benchmark, sound, film  
- **[Where and When to Force: Routed Forcing for Streaming Avatars](https://arxiv.org/abs/2609.30963v1)**  
  Authors: Zihan Su, Siwen Lu, Junhao Zhuang, Zeyue Xue, Haoyang Huang, Guanghao Li, Xiaofeng Tan, Chun Yuan, Nan Duan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.30963v1.pdf)  
  Keywords: distillation, audio-driven, video diffusion, dynamics, avatar, gesture, diffusion model, streaming  
- **[WanPE: Towards Cinematic Prompt Enhancement for Modern Text-to-Video Generation](https://arxiv.org/abs/2609.30221v1)**  
  Authors: Yubo Zhu, Yawen Shao, Ziyun Dai, Zixun Fang, Kai Zhu, Siyang Sun, Haolan Xue, Chuxin Wang, Tingyu Weng, Jingming Luo, Chen Shi, Lianghua Huang, Yufeng Ai, Yuzheng Wang, Wenyuan Zhang, Yu Shang, Yuxiang Bao, Zoubin Bi, Jie Xiao, Jinbo Xing, Jiaxing Zhao, Chongyang Zhong, Hengjian Chen, Chenwei Xie, Akide Liu, Zhehan Kan, Yu Liu, Wei Zhai, Sheng Zhong, Wei Tong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.30221v1.pdf)  
  Keywords: text-to-video, video generation, dit, benchmark, sound  
- **[Dreaming the Sound of Contact: Leveraging Video and Audio Generation for Zero-Shot Force-Aware Manipulation and Data Generation](https://arxiv.org/abs/2609.19137v2)**  
  Authors: Guanhua Ji, Tianyu Li, Dayoon Suh, Yuqian Zhang, Boyan Zhang, Nadia Figueroa  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.19137v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://dreamingcontactsound.github.io)  
  Keywords: video generation, sound  
- **[LynnReal-Omni: Native multi-modal Video Generation for Agentic Visual Workflows](https://arxiv.org/abs/2609.15863v1)**  
  Authors: Xiaofeng Mao, Peijia Lin, Shaohao Rui, Yibo Zhang, Haibin Wan, Weijie Ma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.15863v1.pdf)  
  Keywords: efficient, text-to-video, controllable, evaluation, multi-modal, video restoration, acceleration, video generation, dit, video diffusion, diffusion transformer, diffusion model, streaming  

### Controllable Generation

*Showing the latest 50 out of 116 papers*

- **[LoGo: Local-Global Rewards for Consistent Long-Horizon Video Generation](https://arxiv.org/abs/2610.03636v1)**  
  Authors: Ziqi Ma, Shreya Sharma, Mohamed El Banani, Katja Schwarz, Chongjie Ye, Chao-Yuan Wu, Li Fei-Fei, Ben Mildenhall, Georgia Gkioxari, Justin Johnson, Gowthami Somepalli  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03636v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://ziqi-ma.github.io/logo-website)  
  Keywords: evaluation, camera control, video generation, dit, benchmark, trajectory  
- **[Rethinking What to Cache in Few-Step Diffusion Transformers: Solver-Aware Target Selection](https://arxiv.org/abs/2610.03577v1)**  
  Authors: Shuo Yang, Lihao Fang, Yi Zhang, Haixiang Wang, Xincheng Ye, Shufan Chen, Jipeng Guo, Youqing Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03577v1.pdf) | [![GitHub](https://img.shields.io/github/stars/wali1024-offical/AutoTarget?style=social)](https://github.com/wali1024-offical/AutoTarget)  
  Keywords: diffusion transformer, evaluation, dit, trajectory, distillation  
- **[TRAC: Trajectory-aware Reuse and Adaptive Correction for Efficient Autoregressive Video Generation](https://arxiv.org/abs/2610.02779v1)**  
  Authors: Jiaxing Song, Weiqi Yan, You Huang, Mingte Qiu, Huazhong Liu, Xiaofeng Zhu, Yunshan Zhong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.02779v1.pdf)  
  Keywords: efficient, denoising, acceleration, video generation, autoregressive, trajectory  
- **[A Simulation-Grounded Agentic VLM Framework for Wildfire Monitoring and Reporting](https://arxiv.org/abs/2610.02451v1)**  
  Authors: Duowen Chen, Yuchen Sun, Zhiqi Li, Yuxuan Liao, Sinan Wang, Bart van Bloemen Waanders, Bo Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.02451v1.pdf)  
  Keywords: controllable, evaluation, layout, video generation, dynamics, simulation, physical  
- **[Generative Cinematographer: Composing Camera and Object Motion in 3D](https://arxiv.org/abs/2610.02180v1)**  
  Authors: Jiahan Zhang, Chaohao Yang, Namitha Guruprasad, Vivekjyoti Banerjee, Trong-Tung Nguyen, Alan Yuille, Anand Bhattad  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.02180v1.pdf)  
  Keywords: controllable, video generation, dit, physics, trajectory  
- **[DiVid: Diagnosing Dimension-Specific Diversity Collapse in Video Generation Models](https://arxiv.org/abs/2610.01661v1)**  
  Authors: Huanran Hu, Zihui Ren, Dingyi Yang, Zhinan Song, Guozheng Wu, Tiezheng Ge, Qin Jin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.01661v1.pdf)  
  Keywords: controllable, evaluation, video generation, creative, style  
- **[Oneira: From Open-Ended Generation to Open-World Interaction in Video World Models](https://arxiv.org/abs/2610.01614v1)**  
  Authors: Xindi Yang, Baolu Li, Liam Lee, Zhenfei Yin, Songxin Zhang, Zhuoyang Song, Xu Jia, Jianfei Cai, Tien-Tsin Wong, Bingyi Jing, Mengyue Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.01614v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://madaoer.github.io/projects/oneira)  
  Keywords: world model, dit, interactive, trajectory  
- **[DeFA: Dependency-Guided Failure Attribution for LLM Agents](https://arxiv.org/abs/2610.01256v1)**  
  Authors: Bo Deng, Xinlei Zheng, Yi Wei, Kang Zhou, Chongyang Tao, Renzhao Liang, Xuanren Chen, Lifan Guo, Chi Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.01256v1.pdf)  
  Keywords: trajectory  
- **[Bootstrapping Video Interaction Generation with Synthetic State Transitions](https://arxiv.org/abs/2610.01039v1)**  
  Authors: Jiho Jang, Jinyoung Kim, Nojun Kwak, Kyungjune Kim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.01039v1.pdf)  
  Keywords: controllable, evaluation, dit, robotics, physical  
- **[Video Generation Models: A Survey of Post-Training and Alignment](https://arxiv.org/abs/2610.00812v1)**  
  Authors: Chaoyu Li, Xiaoyi Gu, Yogesh Kulkarni, Eun Woo Im, Mohammadmahdi Honarmand, Zeyu Wang, Juntong Song, Fei Du, Xilin Jiang, Kexin Zheng, Tianzhi Li, Fei Tao, Pooyan Fazli  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.00812v1.pdf)  
  Keywords: physical, controllable, temporal consistency, evaluation, video generation, benchmark, dynamics, distillation, survey, concept  

### Human & Character Animation

- **[Parasitic Co-Denoising: Unlocking 3D Human Motion Generation in a Frozen Video Diffusion Model](https://arxiv.org/abs/2610.03047v1)**  
  Authors: Yunjiao Zhou, Junlang Qian, Lihua Xie, Jianfei Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03047v1.pdf)  
  Keywords: efficient, text-to-video, denoising, human motion, video diffusion, diffusion model  
- **[GLARE: Generating Listening Heads with Appropriate Reactions](https://arxiv.org/abs/2609.40317v1)**  
  Authors: Zikai Liao, Yumin Suh, Yi Ouyang, Yi-Lun Lee, Yi-Hsuan Tsai, Zhaozheng Yin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.40317v1.pdf)  
  Keywords: talking head, evaluation, audio-driven, video generation, dit  
- **[TexTailor: Texture-Preserving Video Virtual Try-On via Adaptive Garment Conditioning](https://arxiv.org/abs/2609.39335v1)**  
  Authors: Zijing Qin, Jun Zhou, Ruicheng Zhang, Jiaqi Hou, Zunnan Xu, Ronghui Li, Zhenyu Xie, Xiu Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.39335v1.pdf)  
  Keywords: temporal consistency, denoising, dit, video diffusion, benchmark, diffusion transformer, virtual try-on  
- **[WeLike2Party! In-Context Motion Transfer for Multi-Human Image Animation](https://arxiv.org/abs/2609.36937v1)**  
  Authors: Sangeyl Lee, Seunghyun Shin, Seungho Park, Wooseok Jeon, Hae-Gon Jeon  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.36937v1.pdf)  
  Keywords: identity, human animation, video generation, dit, image animation, benchmark, trajectory  
- **[FlowAct-R2: Beyond Talking Avatar via Streaming Multimodal References and Proactive Agent Planning](https://arxiv.org/abs/2609.35728v1)**  
  Authors: Ziyao Huang, Zhengkun Rong, Shiyang Qin, Shuang Liang, Wentao Hu, Yuxuan Luo, Yuan Zhang, Mingyuan Gao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.35728v1.pdf)  
  Keywords: interactive, video generation, dit, diffusion transformer, avatar, streaming  
- **[Where and When to Force: Routed Forcing for Streaming Avatars](https://arxiv.org/abs/2609.30963v1)**  
  Authors: Zihan Su, Siwen Lu, Junhao Zhuang, Zeyue Xue, Haoyang Huang, Guanghao Li, Xiaofeng Tan, Chun Yuan, Nan Duan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.30963v1.pdf)  
  Keywords: distillation, audio-driven, video diffusion, dynamics, avatar, gesture, diffusion model, streaming  
- **[All modalities are equal, but video is more equal: Closing the Cross-Attention Gap in Joint Video Generation](https://arxiv.org/abs/2609.27901v1)**  
  Authors: Ohad Rahamim, Dvir Samuel, Idan Schwartz, Gal Chechik  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.27901v1.pdf)  
  Keywords: body motion, video generation, physical, diffusion transformer  
- **[When Visual Quality Misleads: Intent Recognition under Rendered Avatar Distortions](https://arxiv.org/abs/2609.27560v1)**  
  Authors: Ning-Hsuan Chang, Kai-Siang Ma, Yu-Chih Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.27560v1.pdf)  
  Keywords: avatar, dit, streaming  
- **[Vidu S2: Real-Time Interactive, Editable, and Spatial Video Generation](https://arxiv.org/abs/2609.11638v1)**  
  Authors: Jintao Zhang, Kai Jiang, Jintao Chen, Xu Wang, Deyuan Liu, Jungang Li, Dechuang Chen, Ming Lin, Jingjiang Zhou, Haopeng Jin, Qi Jia, Xiaohang Wang, Yaole Wang, Zhanqiang Zhang, Ran Li, Zhengkun Huang, Shuyue Xiong, Yuji Wang, Zikun Dai, Hui He, Yang Luo, Mang Ning, Weiqi Feng, Chengyang Ye, Xinyue Lin, Min Zhao, Hongzhou Zhu, Hengkai Tan, Zeyuan Wang, Chendong Xiang, Kaiwen Zheng, Zhijie Deng, Fan Bao, Jianfei Chen, Jun Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.11638v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://vidu.com/vidu-stream)  
  Keywords: video editing, interactive, video generation, dit, avatar, style  
- **[Decoupled Self-Forcing Distillation for Streaming Talking Head Generation](https://arxiv.org/abs/2609.10317v1)**  
  Authors: Yanru An, Ruiyan Wang, Wenwu Wei, Rui Bu, Qi Wang, Hongwei Hu, Zhengxue Cheng, Rong Xie, Li Song, Wenjun Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.10317v1.pdf)  
  Keywords: talking head, distillation, identity, dit, autoregressive, video diffusion, diffusion model, streaming  

### Image-to-Video Generation

- **[VDOT++: Unified Few-Step Video Generation via Unbalanced Optimal Transport Distillation](https://arxiv.org/abs/2610.03221v1)**  
  Authors: Yutong Wang, Xingtong Ge, Enhuai Liu, Yunke Wang, Tianfan Xue, Yu Qiao, Yaohui Wang, Xinyuan Chen, Chang Xu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03221v1.pdf)  
  Keywords: text-to-video, distillation, video generation, i2v, dit, video diffusion, benchmark, t2v, image-to-video, diffusion model  
- **[Custom Forcing: Training-Free Subject Customization for Autoregressive Video Generation](https://arxiv.org/abs/2610.02914v1)**  
  Authors: Yunseung Ok, Hyunsoo Kim, Minseo Kim, Suhyun Kim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.02914v1.pdf)  
  Keywords: identity, long video, video generation, autoregressive, dit, customization, image-to-video, streaming  
- **[MosaiChunk: Compositing Spatio-Temporal Memory for Autoregressive Video Generation](https://arxiv.org/abs/2610.02153v1)**  
  Authors: Yiwen Zhang, Haocheng Xi, Michael Tian-Yue Liu, Alexei A. Efros, Hadar Averbuch-Elor, Qianqian Wang, Haiwen Feng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.02153v1.pdf)  
  Keywords: text-to-video, video generation, i2v, autoregressive, benchmark, image-to-video, t2v  
- **[PickMoment: Continuous-Time Single-Image-to-Video via Learning Deblurring and Blur-to-Video](https://arxiv.org/abs/2610.01279v1)**  
  Authors: Junseong Shin, Hyeonsu Jo, Daehyun Kim, Tae Hyun Kim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.01279v1.pdf)  
  Keywords: image-to-video, video generation, physical, dit  
- **[Towards Subject Consistency over Dynamic Subject Sets in Video Generation](https://arxiv.org/abs/2610.01052v1)**  
  Authors: Tongcheng Zhang, Jun Zhu, Jianfei Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.01052v1.pdf)  
  Keywords: evaluation, video generation, identity, i2v  
- **[MindWorldBench: Evaluating Mental-State-to-Behavior Reasoning in Image-to-Video Generation](https://arxiv.org/abs/2609.39147v1)**  
  Authors: Ruiqi Li, Xuanyi Liu, Sijia Li, Haofeng Wang, Yuxin Liu, Feng Xie, Songchao Tan, Shiqi Wang, Hanwei Zhu, Yizong Wang, Chuanmin Jia, Siwei Ma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.39147v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://richard2049-lee.github.io/MindWorldBench)  
  Keywords: evaluation, video generation, dit, image-to-video, physical  
- **[LIFT: Layout-In-Future Video Generation under Large Viewpoint Change via On-Policy Self-Distillation](https://arxiv.org/abs/2609.38146v1)**  
  Authors: Shengxiang Ji, Boyang Wang, Haiyang Xu, Bingnan Li, Yucheng Mao, Zeyuan Chen, Xiaojun Shan, Xiang Zhang, Gang Hua, Jianwen Xie, Zezhou Cheng, Zhuowen Tu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.38146v1.pdf)  
  Keywords: controllable, layout, camera control, video generation, dit, image-to-video, distillation  
- **[WeLike2Party! In-Context Motion Transfer for Multi-Human Image Animation](https://arxiv.org/abs/2609.36937v1)**  
  Authors: Sangeyl Lee, Seunghyun Shin, Seungho Park, Wooseok Jeon, Hae-Gon Jeon  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.36937v1.pdf)  
  Keywords: identity, human animation, video generation, dit, image animation, benchmark, trajectory  
- **[Beyond Legibility: Benchmarking Visual Text Rendering and In-Place Editing in Unified Video Generation](https://arxiv.org/abs/2609.36598v2)**  
  Authors: Ziying Zhang, Litao Li, Junchao Liao, Tianyi Zeng, Siyu Zhu, Long Qin, Zhenghao Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.36598v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://huggingface.co/datasets/Vicky0720/VidScribe.) | [![Dataset](https://img.shields.io/badge/-Dataset-orange)](https://huggingface.co/datasets/Vicky0720/VidScribe)  
  Keywords: physical, evaluation, identity, video generation, i2v, dit, benchmark, dynamics, t2v  
- **[OPIS: An Input-Grounded Benchmark for Multi-Object Memory in Video World Models](https://arxiv.org/abs/2609.35052v1)**  
  Authors: Hao Wang, Tao Yu, Liuzhou Zhang, HeXin Wang, Haopeng Jin, Yuxuan Zhou, Xinming Wang, Hongzhu Yi, Xinye Li, Yuanlei Wang, Ping Nie, Yan Huang, Yuxuan Zhang, Pengfei Zhou, Yanyan Zou, Wei Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.35052v1.pdf)  
  Keywords: evaluation, world model, identity, dit, benchmark, image-to-video  

### Long Video Generation

*Showing the latest 50 out of 111 papers*

- **[ProAR: Learning Prospective Reasoning with Autoregressive Video Models](https://arxiv.org/abs/2610.03664v1)**  
  Authors: Linghui Shen, Tinghui Zhu, Sheng Zhang, Muhao Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03664v1.pdf)  
  Keywords: efficient, video generation, autoregressive, benchmark, dynamics  
- **[DuoMatching: Joint-Marginal Distribution Matching for Few-Step Video Generation](https://arxiv.org/abs/2610.03543v1)**  
  Authors: Jiahao Zhan, Yan Wang, Yongrui Ma, Qunliang Xing, Ruchang Yao, Runtao Liu, Shijie Zhao, Tianfan Xue  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03543v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://johnzhan2023.github.io/DuoMatching)  
  Keywords: evaluation, video generation, autoregressive, dit, dynamics, distillation, streaming  
- **[Weave Forcing: Compositional Memory Routing for Interactive Long Video Generation](https://arxiv.org/abs/2610.03510v1)**  
  Authors: Ziyi Wang, Junchi Yao, Heqian Qiu, Wenbo Shi, Chengjiu Wang, Jinyang He, Binkai Hong, Hongliang Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03510v1.pdf)  
  Keywords: temporal consistency, interactive, long video, video generation, autoregressive, dit  
- **[In-Distribution Forcing for Long Video Generation at Test Time](https://arxiv.org/abs/2610.03120v1)**  
  Authors: Jeongwoo Shin, Youngyoon Choi, Sangwoo Jo, Hyunmog Kim, Sungjoon Choi, Joonseok Lee, Jaewoong Choi, Jaemoo Choi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03120v1.pdf)  
  Keywords: evaluation, long video, video generation, autoregressive, dit, video diffusion, benchmark, dynamics, diffusion model  
- **[Custom Forcing: Training-Free Subject Customization for Autoregressive Video Generation](https://arxiv.org/abs/2610.02914v1)**  
  Authors: Yunseung Ok, Hyunsoo Kim, Minseo Kim, Suhyun Kim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.02914v1.pdf)  
  Keywords: identity, long video, video generation, autoregressive, dit, customization, image-to-video, streaming  
- **[TRAC: Trajectory-aware Reuse and Adaptive Correction for Efficient Autoregressive Video Generation](https://arxiv.org/abs/2610.02779v1)**  
  Authors: Jiaxing Song, Weiqi Yan, You Huang, Mingte Qiu, Huazhong Liu, Xiaofeng Zhu, Yunshan Zhong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.02779v1.pdf)  
  Keywords: efficient, denoising, acceleration, video generation, autoregressive, trajectory  
- **[MosaiChunk: Compositing Spatio-Temporal Memory for Autoregressive Video Generation](https://arxiv.org/abs/2610.02153v1)**  
  Authors: Yiwen Zhang, Haocheng Xi, Michael Tian-Yue Liu, Alexei A. Efros, Hadar Averbuch-Elor, Qianqian Wang, Haiwen Feng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.02153v1.pdf)  
  Keywords: text-to-video, video generation, i2v, autoregressive, benchmark, image-to-video, t2v  
- **[Video Generation Models: A Survey of Post-Training and Alignment](https://arxiv.org/abs/2610.00812v1)**  
  Authors: Chaoyu Li, Xiaoyi Gu, Yogesh Kulkarni, Eun Woo Im, Mohammadmahdi Honarmand, Zeyu Wang, Juntong Song, Fei Du, Xilin Jiang, Kexin Zheng, Tianzhi Li, Fei Tao, Pooyan Fazli  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.00812v1.pdf)  
  Keywords: physical, controllable, temporal consistency, evaluation, video generation, benchmark, dynamics, distillation, survey, concept  
- **[SemanTok: Predictable Semantic Tokens for Efficient Autoregressive Video Generation](https://arxiv.org/abs/2610.00686v1)**  
  Authors: Mikhail Dereviannykh, Vikram Voleti, Simon Donne, Mallikarjun Byrasandra Ramalinga Reddy, Shimon Vainer, Mark Boss  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.00686v1.pdf)  
  Keywords: efficient, world model, video generation, autoregressive, diffusion model  
- **[ViTeX-Bench: Benchmarking High-Fidelity Video Scene Text Editing](https://arxiv.org/abs/2609.40356v1)**  
  Authors: Xinghao Chen, Xiangbo Gao, Jiongze Yu, Yuheng Wu, Zhengzhong Tu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.40356v1.pdf)  
  Keywords: video editing, controllable, temporal consistency, evaluation, video generation, dit, benchmark, dynamics  

### Personalization & Customization

*Showing the latest 50 out of 65 papers*

- **[BeeWhere: Segmenting Bumble Bee Colonies to Quantify Behavioral Effects](https://arxiv.org/abs/2610.03051v1)**  
  Authors: Roberta Hunt, August Easton-Calabria, James Crall  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03051v1.pdf)  
  Keywords: dit, identity  
- **[Custom Forcing: Training-Free Subject Customization for Autoregressive Video Generation](https://arxiv.org/abs/2610.02914v1)**  
  Authors: Yunseung Ok, Hyunsoo Kim, Minseo Kim, Suhyun Kim  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.02914v1.pdf)  
  Keywords: identity, long video, video generation, autoregressive, dit, customization, image-to-video, streaming  
- **[DMAD: Distribution Matching as Adversarial Distillation for Fast Visual Generation](https://arxiv.org/abs/2610.02188v1)**  
  Authors: Zhengming Yu, Junkun Yuan, Haotian Yang, Gordon Guocheng Qian, Yizhi Wang, Angtian Wang, Yiding Yang, Bo Liu, Xin Li, Wenping Wang, Chongyang Ma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.02188v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://yzmblog.github.io/projects/DMAD)  
  Keywords: distillation, identity, video generation, t2v, diffusion model  
- **[Memory-Guided B-Roll Generation from User Video Collections](https://arxiv.org/abs/2610.01884v1)**  
  Authors: Cusuh Ham, Fabian Caba Heilbron, Josef Sivic, Bryan Russell  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.01884v1.pdf)  
  Keywords: dit, identity, text-to-video, style  
- **[DiVid: Diagnosing Dimension-Specific Diversity Collapse in Video Generation Models](https://arxiv.org/abs/2610.01661v1)**  
  Authors: Huanran Hu, Zihui Ren, Dingyi Yang, Zhinan Song, Guozheng Wu, Tiezheng Ge, Qin Jin  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.01661v1.pdf)  
  Keywords: controllable, evaluation, video generation, creative, style  
- **[Towards Subject Consistency over Dynamic Subject Sets in Video Generation](https://arxiv.org/abs/2610.01052v1)**  
  Authors: Tongcheng Zhang, Jun Zhu, Jianfei Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.01052v1.pdf)  
  Keywords: evaluation, video generation, identity, i2v  
- **[Video Generation Models: A Survey of Post-Training and Alignment](https://arxiv.org/abs/2610.00812v1)**  
  Authors: Chaoyu Li, Xiaoyi Gu, Yogesh Kulkarni, Eun Woo Im, Mohammadmahdi Honarmand, Zeyu Wang, Juntong Song, Fei Du, Xilin Jiang, Kexin Zheng, Tianzhi Li, Fei Tao, Pooyan Fazli  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.00812v1.pdf)  
  Keywords: physical, controllable, temporal consistency, evaluation, video generation, benchmark, dynamics, distillation, survey, concept  
- **[Strike a Chord! Modal Kinetic Typography](https://arxiv.org/abs/2609.38325v1)**  
  Authors: Maham Tanveer, Jiyeon Han, Nanxuan Zhao, Hao Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.38325v1.pdf)  
  Keywords: diffusion model, video diffusion, concept, distillation  
- **[WeLike2Party! In-Context Motion Transfer for Multi-Human Image Animation](https://arxiv.org/abs/2609.36937v1)**  
  Authors: Sangeyl Lee, Seunghyun Shin, Seungho Park, Wooseok Jeon, Hae-Gon Jeon  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.36937v1.pdf)  
  Keywords: identity, human animation, video generation, dit, image animation, benchmark, trajectory  
- **[S4VY: Segment Anything in Feed-Forward 4D Visual Geometry](https://arxiv.org/abs/2609.36875v1)**  
  Authors: Jingdong Zhang, Xin Li, Jan Kautz, Wenping Wang, Chris Choy  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.36875v1.pdf)  
  Keywords: evaluation, identity, autonomous driving, dit, robotics  

### Physical Understanding

*Showing the latest 50 out of 129 papers*

- **[ProAR: Learning Prospective Reasoning with Autoregressive Video Models](https://arxiv.org/abs/2610.03664v1)**  
  Authors: Linghui Shen, Tinghui Zhu, Sheng Zhang, Muhao Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03664v1.pdf)  
  Keywords: efficient, video generation, autoregressive, benchmark, dynamics  
- **[World Embedding Benchmark](https://arxiv.org/abs/2610.03632v1)**  
  Authors: Yiqi Liu, Ruifeng Yuan, Yang Wang, Long Li, Fengyu Cai, Hou Pong Chan, Jialin Yu, Hao Zhang, Chenghua Lin, Chenghao Xiao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03632v1.pdf)  
  Keywords: world model, video generation, physics, benchmark, dynamics, simulation, physical  
- **[DuoMatching: Joint-Marginal Distribution Matching for Few-Step Video Generation](https://arxiv.org/abs/2610.03543v1)**  
  Authors: Jiahao Zhan, Yan Wang, Yongrui Ma, Qunliang Xing, Ruchang Yao, Runtao Liu, Shijie Zhao, Tianfan Xue  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03543v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://johnzhan2023.github.io/DuoMatching)  
  Keywords: evaluation, video generation, autoregressive, dit, dynamics, distillation, streaming  
- **[Contextual Flow Matching: Adaptive Step Selection in Flow Models for Efficient Visual Generation](https://arxiv.org/abs/2610.03202v1)**  
  Authors: Divya Jyoti Bajpai, Arun Verma, Manjesh Kumar Hanawal  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03202v1.pdf)  
  Keywords: efficient, evaluation, acceleration, video generation, dit, dynamics, flow matching  
- **[Does Physics Live in the Activations? Localizing Physical Quantities in Video Diffusion Models](https://arxiv.org/abs/2610.03154v1)**  
  Authors: Jonas Kneifl, Jakub Skalski, Bartłomiej Twardowski, Kamil Deja  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03154v1.pdf)  
  Keywords: physical, world model, denoising, video generation, dit, physics, video diffusion, benchmark, diffusion transformer, dynamics, diffusion model  
- **[In-Distribution Forcing for Long Video Generation at Test Time](https://arxiv.org/abs/2610.03120v1)**  
  Authors: Jeongwoo Shin, Youngyoon Choi, Sangwoo Jo, Hyunmog Kim, Sungjoon Choi, Joonseok Lee, Jaewoong Choi, Jaemoo Choi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03120v1.pdf)  
  Keywords: evaluation, long video, video generation, autoregressive, dit, video diffusion, benchmark, dynamics, diffusion model  
- **[World Action Modeling with Progressive Visual Planning](https://arxiv.org/abs/2610.02508v1)**  
  Authors: Fei Zhang, Zhaochong An, Duncan Frost, Yikai Wang, Pengfei Liu, Ya Zhang, Michal Drozdzal, Amir Bar  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.02508v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://sii-ferenas.github.io/ProWAM-page)  
  Keywords: efficient, evaluation, denoising, video generation, benchmark, dynamics, simulation  
- **[A Simulation-Grounded Agentic VLM Framework for Wildfire Monitoring and Reporting](https://arxiv.org/abs/2610.02451v1)**  
  Authors: Duowen Chen, Yuchen Sun, Zhiqi Li, Yuxuan Liao, Sinan Wang, Bart van Bloemen Waanders, Bo Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.02451v1.pdf)  
  Keywords: controllable, evaluation, layout, video generation, dynamics, simulation, physical  
- **[HiPhy: Hierarchical Alignment for Physically-Plausible Multi-Principle Video Generation](https://arxiv.org/abs/2610.02197v1)**  
  Authors: Tahira Kazimi, Shubhankar Borse, Munawar Hayat, Fatih Porikli, Pinar Yanardag  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.02197v1.pdf)  
  Keywords: video generation, physics, benchmark, dynamics, world simulator, physical  
- **[Generative Cinematographer: Composing Camera and Object Motion in 3D](https://arxiv.org/abs/2610.02180v1)**  
  Authors: Jiahan Zhang, Chaohao Yang, Namitha Guruprasad, Vivekjyoti Banerjee, Trong-Tung Nguyen, Alan Yuille, Anand Bhattad  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.02180v1.pdf)  
  Keywords: controllable, video generation, dit, physics, trajectory  

### Surveys & Benchmarks

*Showing the latest 50 out of 249 papers*

- **[ProAR: Learning Prospective Reasoning with Autoregressive Video Models](https://arxiv.org/abs/2610.03664v1)**  
  Authors: Linghui Shen, Tinghui Zhu, Sheng Zhang, Muhao Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03664v1.pdf)  
  Keywords: efficient, video generation, autoregressive, benchmark, dynamics  
- **[LoGo: Local-Global Rewards for Consistent Long-Horizon Video Generation](https://arxiv.org/abs/2610.03636v1)**  
  Authors: Ziqi Ma, Shreya Sharma, Mohamed El Banani, Katja Schwarz, Chongjie Ye, Chao-Yuan Wu, Li Fei-Fei, Ben Mildenhall, Georgia Gkioxari, Justin Johnson, Gowthami Somepalli  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03636v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://ziqi-ma.github.io/logo-website)  
  Keywords: evaluation, camera control, video generation, dit, benchmark, trajectory  
- **[World Embedding Benchmark](https://arxiv.org/abs/2610.03632v1)**  
  Authors: Yiqi Liu, Ruifeng Yuan, Yang Wang, Long Li, Fengyu Cai, Hou Pong Chan, Jialin Yu, Hao Zhang, Chenghua Lin, Chenghao Xiao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03632v1.pdf)  
  Keywords: world model, video generation, physics, benchmark, dynamics, simulation, physical  
- **[Rethinking What to Cache in Few-Step Diffusion Transformers: Solver-Aware Target Selection](https://arxiv.org/abs/2610.03577v1)**  
  Authors: Shuo Yang, Lihao Fang, Yi Zhang, Haixiang Wang, Xincheng Ye, Shufan Chen, Jipeng Guo, Youqing Wang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03577v1.pdf) | [![GitHub](https://img.shields.io/github/stars/wali1024-offical/AutoTarget?style=social)](https://github.com/wali1024-offical/AutoTarget)  
  Keywords: diffusion transformer, evaluation, dit, trajectory, distillation  
- **[DuoMatching: Joint-Marginal Distribution Matching for Few-Step Video Generation](https://arxiv.org/abs/2610.03543v1)**  
  Authors: Jiahao Zhan, Yan Wang, Yongrui Ma, Qunliang Xing, Ruchang Yao, Runtao Liu, Shijie Zhao, Tianfan Xue  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03543v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://johnzhan2023.github.io/DuoMatching)  
  Keywords: evaluation, video generation, autoregressive, dit, dynamics, distillation, streaming  
- **[VDOT++: Unified Few-Step Video Generation via Unbalanced Optimal Transport Distillation](https://arxiv.org/abs/2610.03221v1)**  
  Authors: Yutong Wang, Xingtong Ge, Enhuai Liu, Yunke Wang, Tianfan Xue, Yu Qiao, Yaohui Wang, Xinyuan Chen, Chang Xu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03221v1.pdf)  
  Keywords: text-to-video, distillation, video generation, i2v, dit, video diffusion, benchmark, t2v, image-to-video, diffusion model  
- **[Contextual Flow Matching: Adaptive Step Selection in Flow Models for Efficient Visual Generation](https://arxiv.org/abs/2610.03202v1)**  
  Authors: Divya Jyoti Bajpai, Arun Verma, Manjesh Kumar Hanawal  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03202v1.pdf)  
  Keywords: efficient, evaluation, acceleration, video generation, dit, dynamics, flow matching  
- **[Does Physics Live in the Activations? Localizing Physical Quantities in Video Diffusion Models](https://arxiv.org/abs/2610.03154v1)**  
  Authors: Jonas Kneifl, Jakub Skalski, Bartłomiej Twardowski, Kamil Deja  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03154v1.pdf)  
  Keywords: physical, world model, denoising, video generation, dit, physics, video diffusion, benchmark, diffusion transformer, dynamics, diffusion model  
- **[In-Distribution Forcing for Long Video Generation at Test Time](https://arxiv.org/abs/2610.03120v1)**  
  Authors: Jeongwoo Shin, Youngyoon Choi, Sangwoo Jo, Hyunmog Kim, Sungjoon Choi, Joonseok Lee, Jaewoong Choi, Jaemoo Choi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03120v1.pdf)  
  Keywords: evaluation, long video, video generation, autoregressive, dit, video diffusion, benchmark, dynamics, diffusion model  
- **[Spatial Memory Intelligence: Endowing World Models with Understanding-Driven Long-Term Memory](https://arxiv.org/abs/2610.02521v1)**  
  Authors: Ying Yang, Guiyu Zhang, Lianghua Huang, Chang Nie, Chenyang Si, Haofan Wang, Shaoshuai Shi, Li Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.02521v1.pdf)  
  Keywords: world model, interactive, video generation, dit, benchmark, simulation  

### Text-to-Video Generation

*Showing the latest 50 out of 63 papers*

- **[VDOT++: Unified Few-Step Video Generation via Unbalanced Optimal Transport Distillation](https://arxiv.org/abs/2610.03221v1)**  
  Authors: Yutong Wang, Xingtong Ge, Enhuai Liu, Yunke Wang, Tianfan Xue, Yu Qiao, Yaohui Wang, Xinyuan Chen, Chang Xu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03221v1.pdf)  
  Keywords: text-to-video, distillation, video generation, i2v, dit, video diffusion, benchmark, t2v, image-to-video, diffusion model  
- **[Parasitic Co-Denoising: Unlocking 3D Human Motion Generation in a Frozen Video Diffusion Model](https://arxiv.org/abs/2610.03047v1)**  
  Authors: Yunjiao Zhou, Junlang Qian, Lihua Xie, Jianfei Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03047v1.pdf)  
  Keywords: efficient, text-to-video, denoising, human motion, video diffusion, diffusion model  
- **[DMAD: Distribution Matching as Adversarial Distillation for Fast Visual Generation](https://arxiv.org/abs/2610.02188v1)**  
  Authors: Zhengming Yu, Junkun Yuan, Haotian Yang, Gordon Guocheng Qian, Yizhi Wang, Angtian Wang, Yiding Yang, Bo Liu, Xin Li, Wenping Wang, Chongyang Ma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.02188v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://yzmblog.github.io/projects/DMAD)  
  Keywords: distillation, identity, video generation, t2v, diffusion model  
- **[MosaiChunk: Compositing Spatio-Temporal Memory for Autoregressive Video Generation](https://arxiv.org/abs/2610.02153v1)**  
  Authors: Yiwen Zhang, Haocheng Xi, Michael Tian-Yue Liu, Alexei A. Efros, Hadar Averbuch-Elor, Qianqian Wang, Haiwen Feng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.02153v1.pdf)  
  Keywords: text-to-video, video generation, i2v, autoregressive, benchmark, image-to-video, t2v  
- **[Memory-Guided B-Roll Generation from User Video Collections](https://arxiv.org/abs/2610.01884v1)**  
  Authors: Cusuh Ham, Fabian Caba Heilbron, Josef Sivic, Bryan Russell  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.01884v1.pdf)  
  Keywords: dit, identity, text-to-video, style  
- **[Motion Concept Unlearning in Video Diffusion Models](https://arxiv.org/abs/2609.36832v1)**  
  Authors: Ping Liu, Chi Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.36832v1.pdf)  
  Keywords: text-to-video, denoising, architecture, video generation, dit, video diffusion, t2v, diffusion transformer, dynamics, diffusion model, concept  
- **[Beyond Legibility: Benchmarking Visual Text Rendering and In-Place Editing in Unified Video Generation](https://arxiv.org/abs/2609.36598v2)**  
  Authors: Ziying Zhang, Litao Li, Junchao Liao, Tianyi Zeng, Siyu Zhu, Long Qin, Zhenghao Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.36598v2.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://huggingface.co/datasets/Vicky0720/VidScribe.) | [![Dataset](https://img.shields.io/badge/-Dataset-orange)](https://huggingface.co/datasets/Vicky0720/VidScribe)  
  Keywords: physical, evaluation, identity, video generation, i2v, dit, benchmark, dynamics, t2v  
- **[CoRe: Co-Evolving Reward Models for Mitigating Latent Reward Hacking in Video Diffusion Models](https://arxiv.org/abs/2609.36245v1)**  
  Authors: Zhaolong Su, Yujin Han, Feng Wang, Jameson Dong, Hins Hu, Difan Zou  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.36245v1.pdf)  
  Keywords: efficient, diffusion model, video diffusion, t2v  
- **[Generative Uncertainty as a Self-supervised Signal for Semantic Similarity Learning](https://arxiv.org/abs/2609.35341v1)**  
  Authors: Enrico Pallotta, Sina Raoufi, Lars Doorenbos, Gianni Franchi, Juergen Gall  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.35341v1.pdf)  
  Keywords: diffusion model, text-to-video, t2v, concept  
- **[G$^3$-LoRA: Organizing Reward-Weighted Video Data with Gradient-Guided Grouped LoRA](https://arxiv.org/abs/2609.35189v1)**  
  Authors: Jia Song, Wenhow Li, Lichen Bai, Bada Ye, Zeke Xie  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.35189v1.pdf)  
  Keywords: text-to-video, distillation, evaluation, denoising, t2v, flow matching  

### Video Editing

- **[Unsupervised Domain Adaptation for Enhanced Radiometer Image Precipitation Estimation using Conditional Flow Matching](https://arxiv.org/abs/2610.01890v1)**  
  Authors: Victor Enescu, Assaad Zeghina, Matthieu Meignin, Nicolas Viltard, Cécile Mallet  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.01890v1.pdf)  
  Keywords: dit, video editing, flow matching  
- **[ViTeX-Bench: Benchmarking High-Fidelity Video Scene Text Editing](https://arxiv.org/abs/2609.40356v1)**  
  Authors: Xinghao Chen, Xiangbo Gao, Jiongze Yu, Yuheng Wu, Zhengzhong Tu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.40356v1.pdf)  
  Keywords: video editing, controllable, temporal consistency, evaluation, video generation, dit, benchmark, dynamics  
- **[Diffusion Editing with Soft Mask: Pixel Level Redo of Image and Video with Adjustable Strength](https://arxiv.org/abs/2610.00359v1)**  
  Authors: Candi Zheng, Yuan Lan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.00359v1.pdf)  
  Keywords: efficient, video editing, dit, video diffusion, diffusion model  
- **[Counterfactual Video Generation Enables Scalable Humanoid Loco-Manipulation](https://arxiv.org/abs/2609.38172v1)**  
  Authors: Zihan Wang, Zhen Wu, Pieter Abbeel, Rocky Duan, Jitendra Malik, Carmelo Sferrazza, C. Karen Liu, Guanya Shi, Angjoo Kanazawa  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.38172v1.pdf)  
  Keywords: video generation, physical, video-to-video  
- **[VideoPhysEdit: Physical Counterfactual Video Editing via Rigid-Body Physical Scene Reconstruction](https://arxiv.org/abs/2609.35134v1)**  
  Authors: Conghan Yue, Yuanjie Chen, Yue Han, Ya Gao, Yunyan Xiao, WeiYao Zhang, Zhineng Chen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.35134v1.pdf) | [![GitHub](https://img.shields.io/github/stars/Hammour-steak/VideoPhysEdit?style=social)](https://github.com/Hammour-steak/VideoPhysEdit)  
  Keywords: video editing, evaluation, video generation, dit, physics, benchmark, simulation, physical  
- **[Enhanced Video Text Editing with Trajectory-Aligned Glyph Rendering](https://arxiv.org/abs/2609.34178v1)**  
  Authors: Shulian Zhang, Xiangyu Shu, Wenbo Li, Jian Chen, Yong Guo  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.34178v1.pdf)  
  Keywords: video editing, dit, video diffusion, benchmark, trajectory, diffusion model  
- **[VideoX-Qwen: Data-Centric Instruction-Based Video Editing](https://arxiv.org/abs/2609.26015v1)**  
  Authors: JJiahang Li, Dingbao Shao, Xinyu Chen, Song Wu, Jiang Lin, Duo Li, Yuhang Liu, Jiaxin Hu, Shengrong Gu, Ying Tai, Zili Yi  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.26015v1.pdf)  
  Keywords: video generation, video editing, dit  
- **[Streaming Video Editing with Easy Adaptation](https://arxiv.org/abs/2609.24788v1)**  
  Authors: Yujia Hu, Jiajun Li, Zihao He, Songhua Liu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.24788v1.pdf) | [![GitHub](https://img.shields.io/github/stars/YujiaHu1109/SVEET?style=social)](https://github.com/YujiaHu1109/SVEET)  
  Keywords: video editing, controllable, architecture, acceleration, video generation, dit, video diffusion, diffusion model, streaming, video-to-video  
- **[Edit-VAR: Taming Visual Autoregressive Model for Precise Video Editing](https://arxiv.org/abs/2609.21268v1)**  
  Authors: Chongbo Zhao, Jiangming Wang, Xilai Wang, Xinyu Wang, Jingyi Tang, Chunjie Hao, Pengjie Song, Yue Ma  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.21268v1.pdf)  
  Keywords: dit, video editing, autoregressive, trajectory  
- **[Video DeltaNet: A Video-Native Hybrid Attention for Livestream Video Generation](https://arxiv.org/abs/2609.20744v3)**  
  Authors: Haocheng Xi, Yiming Xie, Hexu Zhao, Yiwen Zhang, Michael Liu, Thomas Creavin, Kurt Keutzer, Xiuyu Li, Zhaoyang Lv, Chenfeng Xu, Haiwen Feng  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.20744v3.pdf) | [![GitHub](https://img.shields.io/github/stars/OpenVDN/vdn-minimax-h3?style=social)](https://github.com/OpenVDN/vdn-minimax-h3) | [![Project](https://img.shields.io/badge/-Project-blue)](https://huggingface.co/OpenVDN/vdn-minimax-h3) | [![HuggingFace](https://img.shields.io/badge/-HuggingFace-yellow)](https://huggingface.co/OpenVDN/vdn-minimax-h3)  
  Keywords: distillation, denoising, video generation, dit, video diffusion, diffusion model, video-to-video  

### Video Inpainting & Completion

- **[WorldWeave: Growing Persistent Geometric Worlds for Video Generation](https://arxiv.org/abs/2609.34221v1)**  
  Authors: Yifan Huang, Lifan Jiang, Qingyue Hao, Cheng Chen, Boxi Wu, Xiaoxue Ren, Xiaofei He, Dehai Zhao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.34221v1.pdf)  
  Keywords: video synthesis, world model, outpainting, video generation, dit  
- **[MT-WAM: Reorienting the One-Pass Predictive Representation Toward Action Generation](https://arxiv.org/abs/2609.21474v1)**  
  Authors: Yiguang Yang, Jiankun Peng, Xiaoming Wang, Yiran Zhang, Zhibo Fang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.21474v1.pdf)  
  Keywords: dit, video diffusion, video prediction, diffusion transformer, dynamics  
- **[StrucPhysVideo: Learning Physical Dynamics from Structured Captions and Robot Actions](https://arxiv.org/abs/2609.18430v1)**  
  Authors: Awomo-WM Team, :, Enhui Ma, Kaiwen Guo, Tingrui Zhang, Wei Song, Yingshui Tan, Jianhua Xu, Tong Zhang, Kaicheng Yu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.18430v1.pdf)  
  Keywords: action-conditioned, physical, world model, denoising, interactive, i2v, autoregressive, dit, physics, video prediction, dynamics, image-to-video, distillation  
- **[GeoLAM: Learning Geometry-Grounded Latent Actions from Unlabeled Human Videos](https://arxiv.org/abs/2609.17099v1)**  
  Authors: Yifan Xie, Hekun Tian, Jinkun Liu, YuAn Wang, Qiao Sun, Wenbo Ding  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.17099v1.pdf)  
  Keywords: evaluation, video generation, benchmark, video prediction, trajectory  
- **[AcrossVAM1.0: Particle World Modeling for Text-Assisted Robot Video Prediction](https://arxiv.org/abs/2608.28491v1)**  
  Authors: Yafei Zhang, Nan Wu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.28491v1.pdf)  
  Keywords: world model, benchmark, video prediction, dynamics, trajectory, film  
- **[V-RAE: Rethinking Video Latent Spaces for Generation](https://arxiv.org/abs/2608.13556v1)**  
  Authors: Minghui Guo, Shengqiong Wu, Hao Fei  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.13556v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://v-rae.github.io)  
  Keywords: latent video, architecture, video generation, dit, video prediction  
- **[GeoRoute: Geometry-Aware Hybrid Inference for Traffic Future-Frame Prediction](https://arxiv.org/abs/2608.09493v1)**  
  Authors: Khang Minh Le, Hieu Dinh Trung Pham, Luu Thanh Danh, Nam-Tien Le, Hieu Anh Ngo, Phuong Huu Vu Tran, Son Nguyen Minh Le, Nguyen Trong Nghia, Tu Tran Thi Cam, Huy Minh Nhat Nguyen, Cuong Tuan Nguyen  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.09493v1.pdf)  
  Keywords: latent video, autonomous driving, architecture, dit, video diffusion, benchmark, video prediction, diffusion model  
- **[SimWAM: A Simple World Action Model for End-to-End Autonomous Driving](https://arxiv.org/abs/2608.07468v5)**  
  Authors: Zongchuang Zhao, Xin Zhou, Tianyang Xu, Zhengyang Sun, Kaixuan Zhou, Yu Wu, Honglin Li, Dingkang Liang, Xiang Bai  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.07468v5.pdf) | [![GitHub](https://img.shields.io/github/stars/H-EmbodVis/SimWAM?style=social)](https://github.com/H-EmbodVis/SimWAM)  
  Keywords: efficient, autonomous driving, video generation, video prediction, trajectory, dynamics, physical, flow matching  
- **[MirrorWorld: Taming Video Diffusion Models for Mirror Reflection Generation](https://arxiv.org/abs/2608.07463v1)**  
  Authors: Youjun Zhao, Alex Warren, Gary K. L. Tam, Rynson W. H. Lau  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2608.07463v1.pdf)  
  Keywords: video synthesis, distillation, video inpainting, video diffusion, benchmark, diffusion model  

### Video Super-Resolution & Enhancement

*Showing the latest 50 out of 82 papers*

- **[Does Physics Live in the Activations? Localizing Physical Quantities in Video Diffusion Models](https://arxiv.org/abs/2610.03154v1)**  
  Authors: Jonas Kneifl, Jakub Skalski, Bartłomiej Twardowski, Kamil Deja  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03154v1.pdf)  
  Keywords: physical, world model, denoising, video generation, dit, physics, video diffusion, benchmark, diffusion transformer, dynamics, diffusion model  
- **[Parasitic Co-Denoising: Unlocking 3D Human Motion Generation in a Frozen Video Diffusion Model](https://arxiv.org/abs/2610.03047v1)**  
  Authors: Yunjiao Zhou, Junlang Qian, Lihua Xie, Jianfei Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03047v1.pdf)  
  Keywords: efficient, text-to-video, denoising, human motion, video diffusion, diffusion model  
- **[TRAC: Trajectory-aware Reuse and Adaptive Correction for Efficient Autoregressive Video Generation](https://arxiv.org/abs/2610.02779v1)**  
  Authors: Jiaxing Song, Weiqi Yan, You Huang, Mingte Qiu, Huazhong Liu, Xiaofeng Zhu, Yunshan Zhong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.02779v1.pdf)  
  Keywords: efficient, denoising, acceleration, video generation, autoregressive, trajectory  
- **[SymRegFlow: Symmetry-Regularized Flow Matching for Video World Models](https://arxiv.org/abs/2610.02726v1)**  
  Authors: Xi Ye, Yuzhu Wang, Xiaoyang Liu, Jiayi Wang, Yangyang Xu, Ruyu Wang, Wenlin Chen, Duo Su, Jun Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.02726v1.pdf)  
  Keywords: world model, denoising, video generation, dit, flow matching  
- **[World Action Modeling with Progressive Visual Planning](https://arxiv.org/abs/2610.02508v1)**  
  Authors: Fei Zhang, Zhaochong An, Duncan Frost, Yikai Wang, Pengfei Liu, Ya Zhang, Michal Drozdzal, Amir Bar  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.02508v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://sii-ferenas.github.io/ProWAM-page)  
  Keywords: efficient, evaluation, denoising, video generation, benchmark, dynamics, simulation  
- **[Token-Level Video Reinforcement Learning](https://arxiv.org/abs/2610.01973v1)**  
  Authors: Yifan Wang, Gordon Guocheng Qian, Yanyu Li, Anil Kag, Yun Fu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.01973v1.pdf)  
  Keywords: video generation, denoising, dit  
- **[Enhancing Autoregressive Video Generation via Representation Adversarial Distillation](https://arxiv.org/abs/2609.40037v1)**  
  Authors: Fangyu Lin, Xingtong Ge, Lunjie Zhu, Yi Zhang, Zhening Liu, Tianhang Wang, Mengfei Li, Yumeng Zhang, Guanglu Song, Yu Liu, Jun Zhang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.40037v1.pdf)  
  Keywords: efficient, denoising, architecture, video generation, autoregressive, dit, distillation, streaming  
- **[The Golden Path Hypothesis: Reusable Schedules in Diffusion Caching](https://arxiv.org/abs/2609.39343v1)**  
  Authors: Dong Wang, Wenwu Tang, Francesco Corti, Yun Cheng, Lothar Thiele, Olga Saukh  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.39343v1.pdf)  
  Keywords: evaluation, dit, denoising  
- **[TexTailor: Texture-Preserving Video Virtual Try-On via Adaptive Garment Conditioning](https://arxiv.org/abs/2609.39335v1)**  
  Authors: Zijing Qin, Jun Zhou, Ruicheng Zhang, Jiaqi Hou, Zunnan Xu, Ronghui Li, Zhenyu Xie, Xiu Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.39335v1.pdf)  
  Keywords: temporal consistency, denoising, dit, video diffusion, benchmark, diffusion transformer, virtual try-on  
- **[DeCoPrune: Efficient KV-Cache Pruning for Autoregressive Video Diffusion via Denoising Consistency](https://arxiv.org/abs/2609.39096v1)**  
  Authors: Zeqi Xiao, Qingle Liu, Kaiwen Zhang, Yifan Zhou, Zihan Ding, Xingang Pan  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2609.39096v1.pdf) | [![GitHub](https://img.shields.io/github/stars/DeCoPrune/CMBench?style=social)](https://github.com/DeCoPrune/CMBench) | [![Project](https://img.shields.io/badge/-Project-blue)](https://decoprune.github.io) | [![Dataset](https://img.shields.io/badge/-Dataset-orange)](https://huggingface.co/datasets/Aoraku/CMBench)  
  Keywords: efficient, denoising, interactive, autoregressive, video diffusion, benchmark, streaming  

### World Models & Simulation

*Showing the latest 50 out of 103 papers*

- **[World Embedding Benchmark](https://arxiv.org/abs/2610.03632v1)**  
  Authors: Yiqi Liu, Ruifeng Yuan, Yang Wang, Long Li, Fengyu Cai, Hou Pong Chan, Jialin Yu, Hao Zhang, Chenghua Lin, Chenghao Xiao  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03632v1.pdf)  
  Keywords: world model, video generation, physics, benchmark, dynamics, simulation, physical  
- **[Weave Forcing: Compositional Memory Routing for Interactive Long Video Generation](https://arxiv.org/abs/2610.03510v1)**  
  Authors: Ziyi Wang, Junchi Yao, Heqian Qiu, Wenbo Shi, Chengjiu Wang, Jinyang He, Binkai Hong, Hongliang Li  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03510v1.pdf)  
  Keywords: temporal consistency, interactive, long video, video generation, autoregressive, dit  
- **[Does Physics Live in the Activations? Localizing Physical Quantities in Video Diffusion Models](https://arxiv.org/abs/2610.03154v1)**  
  Authors: Jonas Kneifl, Jakub Skalski, Bartłomiej Twardowski, Kamil Deja  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.03154v1.pdf)  
  Keywords: physical, world model, denoising, video generation, dit, physics, video diffusion, benchmark, diffusion transformer, dynamics, diffusion model  
- **[SymRegFlow: Symmetry-Regularized Flow Matching for Video World Models](https://arxiv.org/abs/2610.02726v1)**  
  Authors: Xi Ye, Yuzhu Wang, Xiaoyang Liu, Jiayi Wang, Yangyang Xu, Ruyu Wang, Wenlin Chen, Duo Su, Jun Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.02726v1.pdf)  
  Keywords: world model, denoising, video generation, dit, flow matching  
- **[Spatial Memory Intelligence: Endowing World Models with Understanding-Driven Long-Term Memory](https://arxiv.org/abs/2610.02521v1)**  
  Authors: Ying Yang, Guiyu Zhang, Lianghua Huang, Chang Nie, Chenyang Si, Haofan Wang, Shaoshuai Shi, Li Jiang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.02521v1.pdf)  
  Keywords: world model, interactive, video generation, dit, benchmark, simulation  
- **[World Action Modeling with Progressive Visual Planning](https://arxiv.org/abs/2610.02508v1)**  
  Authors: Fei Zhang, Zhaochong An, Duncan Frost, Yikai Wang, Pengfei Liu, Ya Zhang, Michal Drozdzal, Amir Bar  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.02508v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://sii-ferenas.github.io/ProWAM-page)  
  Keywords: efficient, evaluation, denoising, video generation, benchmark, dynamics, simulation  
- **[A Simulation-Grounded Agentic VLM Framework for Wildfire Monitoring and Reporting](https://arxiv.org/abs/2610.02451v1)**  
  Authors: Duowen Chen, Yuchen Sun, Zhiqi Li, Yuxuan Liao, Sinan Wang, Bart van Bloemen Waanders, Bo Zhu  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.02451v1.pdf)  
  Keywords: controllable, evaluation, layout, video generation, dynamics, simulation, physical  
- **[HiPhy: Hierarchical Alignment for Physically-Plausible Multi-Principle Video Generation](https://arxiv.org/abs/2610.02197v1)**  
  Authors: Tahira Kazimi, Shubhankar Borse, Munawar Hayat, Fatih Porikli, Pinar Yanardag  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.02197v1.pdf)  
  Keywords: video generation, physics, benchmark, dynamics, world simulator, physical  
- **[Oneira: From Open-Ended Generation to Open-World Interaction in Video World Models](https://arxiv.org/abs/2610.01614v1)**  
  Authors: Xindi Yang, Baolu Li, Liam Lee, Zhenfei Yin, Songxin Zhang, Zhuoyang Song, Xu Jia, Jianfei Cai, Tien-Tsin Wong, Bingyi Jing, Mengyue Yang  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.01614v1.pdf) | [![Project](https://img.shields.io/badge/-Project-blue)](https://madaoer.github.io/projects/oneira)  
  Keywords: world model, dit, interactive, trajectory  
- **[AiSearch: Interactive Multi-Modal Search with VLMs](https://arxiv.org/abs/2610.01389v1)**  
  Authors: Ali Koksal, Mei Chee Leong, Vicky Sintunata, Ching Ling Chin, Wee Teck Fong  
  Links: [![PDF](https://img.shields.io/badge/PDF-arXiv-b31b1b.svg)](https://arxiv.org/pdf/2610.01389v1.pdf)  
  Keywords: multi-modal, benchmark, interactive  



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
