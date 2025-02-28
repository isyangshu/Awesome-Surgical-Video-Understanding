# Awesome-Surgical-Video-Understanding
There are compilations of surgery-related tasks, datasets, and papers.

``Pretraining Part`` includes all endoscopic methods, whether related to surgery or examination.

## Contents
- [Dataset](#dataset)
  - [Endoscopy](#endoscopy)
    - [Public Dataset](#public-dataset)
  - [Endoscopic Surgery](#endoscopic-surgery)
    - [Public Dataset](#public-dataset)
    - [Private Dataset](#private-dataset)
  - [Egocentric Open Surgery](#egocentric-open-surgery)
  - [Ophthalmic Surgery](#ophthalmic-surgery)
- [Specific Task](#specific-task)
  - [Surgical Phase Recognition](#surgical-phase-recognition)
  - [Surgical Triplet Recognition](#surgical-triplet-recognition)
  - [Surgical Tool Detection](#surgical-tool-detection)
  - [Segmentation](#segmentation)
  - [Surgical Scene Reconstruction](#surgical-scene-reconstruction)
  - [Surgical Video Generation](#surgical-video-generation)
  - [Surgical VQA](#surgical_vqa)
  - [Surgical Type Recognition](#surgical-type-recognition)
- [Pretraining](#pretraining)
  - [Vision Pretraining](#vision-pretraining)
  - [Vision-language Pretraining](#vision-language-pretraining)
  - [LLM-based VLM](#llm-based-vlm)
- [Comprehensive Journals](#comprehensive-journals)

## Dataset

### Endoscopy

#### Public Dataset
| Dataset| Paper | Link | Data Type | Task | Type |
| :-------- | :---- | :-------- | :-------- |  :-------- |  :-------- |
| Kvasir-VQA | [Paper](https://arxiv.org/pdf/2409.01437)| [Link](https://datasets.simula.no/kvasir-vqa) | GI Endoscopy + Surgery | Visual Question Answering| Image-level |

### Endoscopic Surgery

#### Public Dataset

| Dataset| Paper | Link | Procedure | Task | Type |
| :-------- | :---- | :-------- | :-------- |  :-------- |  :-------- |
| Cholec80 | [Paper](https://arxiv.org/pdf/1602.03012)| [Link](https://camma.unistra.fr/datasets/) | Cholecystectomy Surgery | Surgical Phase Recognition | Video-level |
| Cholec80-CSV | [Paper](https://www.nature.com/articles/s41597-023-02073-7)| [Link](https://github.com/ManuelRios18/CHOLEC80-CVS-PUBLIC) | Cholecystectomy Surgery | Critical View of Safety (CVS) | Video-level |
|M2CAI16-Workflow| [Paper](https://arxiv.org/pdf/1610.09278)| [Link](https://camma.unistra.fr/datasets/) | Cholecystectomy Surgery | Surgical Phase Recognition | Video-level |
|M2CAI16-Tool| [Paper](https://arxiv.org/pdf/1602.03012)| [Link](https://camma.unistra.fr/datasets/) | Cholecystectomy Surgery | Surgical Tool Recognition | Video-level |
| CholecT50| [Paper](https://arxiv.org/pdf/2109.03223)| [Link](https://camma.unistra.fr/datasets/) | Cholecystectomy Surgery | Surgical Triplet Recognition | Video-level |
| HeiChole| [Paper](https://arxiv.org/pdf/2109.14956#page=29.04)| [Link](https://www.synapse.org/Synapse:syn18824884/wiki/591922) | Cholecystectomy Surgery | Surgical Phase/Action/Instrument Recognition / Skill Assessment | Video-level |
| Pit-Vis| [Paper](https://arxiv.org/pdf/2409.01184)| [Link](https://rdr.ucl.ac.uk/articles/dataset/PitVis_Challenge_Endoscopic_Pituitary_Surgery_videos/26531686) | Pituitary Surgery | Surgical Step/Instrument Recognition | Video-level |
| PSI-AVA| [Paper](https://arxiv.org/pdf/2212.04582)| [Link](https://github.com/BCV-Uniandes/TAPIR) | Prostatectomy Surgery | Surgical Phase/Step/Action/Instrument Recognition | Video-level |
| GraSP | [Paper](https://arxiv.org/pdf/2401.11174)| [Link](https://github.com/BCV-Uniandes/GraSP) | Prostatectomy Surgery | Surgical Phase/Step/Action/Instrument Recognition / Surgical Instrument Segmentation | Video-level |
| AutoLaparo| [Paper](https://arxiv.org/pdf/2208.02049)| [Link](https://autolaparo.github.io/) | Hysterectomy Surgery | Surgical Phase Recognition / Motion Prediction | Video-level |
| MultiBypass140| [Paper](https://arxiv.org/pdf/2312.11250)| [Link](https://github.com/CAMMA-public/MultiBypass140) | Laparoscopic Roux-en-Y Gastric Bypass Surgery | Surgical Phase/Step Recognition | Video-level |
| SurgToolLoc22| [Paper](https://arxiv.org/pdf/2305.07152)| [Link](https://surgtoolloc23.grand-challenge.org/) |  DaVinci Robotic Surgery | Surgical Tool Recognition/Detection | Video-level |
| SurgT| [Paper](https://arxiv.org/pdf/2302.03022)| [Link](https://surgt.grand-challenge.org/) |  - | Surgical Tissue Tracking | Video-level (30s) |
| SSG-VQA| [Paper](https://arxiv.org/pdf/2312.10251)| [Link](https://github.com/CAMMA-public/SSG-VQA) |Cholecystectomy Surgery | Visual Question Answering| Image-level |
| EndoVis-18-VQA| [Paper](https://arxiv.org/pdf/2206.11053)| [Link](https://github.com/lalithjets/Surgical_VQA) |Robotic Nephrectomy Surgery | Visual Question Answering| Image-level |
| Cholec80-VQA| [Paper](https://arxiv.org/pdf/2206.11053)| [Link](https://github.com/lalithjets/Surgical_VQA) |Cholecystectomy Surgery | Visual Question Answering| Image-level |
| Endoscapes | [Paper](https://arxiv.org/pdf/2312.12429)| [Link](https://github.com/CAMMA-public/Endoscapes) |Cholecystectomy Surgery | Segmentation/Detection/CVS| Image-level |
| StereoMIS | [Paper](https://arxiv.org/pdf/2304.08023)| [Link](https://zenodo.org/records/7727692) | DaVinci Robotic Surgery| Surgical Scene Reconstruction |
| EndoNeRF | [Paper](https://arxiv.org/pdf/2206.15255)| [Link](https://github.com/med-air/EndoNeRF?tab=readme-ov-file) | DaVinci robotic prostatectomy | Surgical Scene Reconstruction |

#### Private Dataset
| Dataset| Paper | Procedure | Task | Type |
| :-------- | :---- | :-------- |  :-------- |  :-------- |
| Laparo425 | [Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8772203)| Laparoscopic Surgery | Surgical Type Recognition | Video-level |
| MultiCholec2022 | [Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9950359)| Cholecystectomy Surgery | Surgical Phase Recognition | Video-level |
| Laparo23.3M | [Paper](https://arxiv.org/pdf/2308.12394)| Laparoscopic Surgery | - | Video-level |
|ESD385| [Paper](https://arxiv.org/pdf/2409.12108v1)| Endoscopic Submucosal Dissection | Surgical Phase Recognition | Video-level|


### Egocentric Open Surgery
| Dataset| Paper | Link | Type | Task |
| :-------- | :---- | :-------- | :-------- |  :-------- |
| EgoSurgery-Tool | [Paper](https://arxiv.org/pdf/2406.03095)| [Link](https://github.com/Fujiry0/EgoSurgery) | Distinct Surgical Procedures | Surgical Tool/Hand Detection |
| EgoSurgery-Phase | [Paper](https://www.arxiv.org/pdf/2405.19644) | [Link](https://github.com/Fujiry0/EgoSurgery)  | Distinct Surgical Procedures | Surgical Phase Recognition |

## Specific Task
### Surgical Phase Recognition

| Paper | Surgery | Image | Link | Code | Type |
| :-------- | :---- | :---- | :-------- | :-------- | :-------- |
| EndoNet: A Deep Architecture for Recognition Tasks on Laparoscopic Videos (**TMI-16**) |Endoscopic Surgery | ![image](https://github.com/user-attachments/assets/5997553c-83e1-4da5-be34-63cf1fa8c4a1) | [Link](https://arxiv.org/pdf/1602.03012) | | Vision |
| SV-RCNet: Workflow Recognition From Surgical Videos Using Recurrent Convolutional Network (**TMI-18**) |Endoscopic Surgery | ![image](https://github.com/user-attachments/assets/64d48b27-b423-4e66-ab48-0917bed762d7) | [Link](https://ieeexplore.ieee.org/abstract/document/8240734) | [Code](https://github.com/YuemingJin/SV-RCNet) | Vision |
| Hard Frame Detection and Online Mapping for Surgical Phase Recognition (**MICCAI-19**) |Endoscopic Surgery | ![image](https://github.com/user-attachments/assets/f5734c0e-da10-4104-8876-1a84a957c308)  | [Link](https://link.springer.com/chapter/10.1007/978-3-030-32254-0_50) | [Code](https://github.com/ChinaYi/miccai19) | Vision |
| Multi-task recurrent convolutional network with correlation loss for surgical video analysis (**MIA-20**) |Endoscopic Surgery | ![image](https://github.com/user-attachments/assets/610b5e6c-ba61-4ba3-bb41-d342b8416185) | [Link](https://arxiv.org/pdf/1907.06099) | [Code](https://github.com/YuemingJin/MTRCNet-CL) | Vision |
| TeCNO: Surgical Phase Recognition with Multi-stage Temporal Convolutional Networks (**MICCAI-20**) |Endoscopic Surgery | ![image](https://github.com/user-attachments/assets/c958e6d4-5225-42b0-8e97-69c5d2e31900) | [Link](https://arxiv.org/pdf/2003.10751) | [Code](https://github.com/tobiascz/TeCNO) | Vision |
| Temporal Memory Relation Network for Workflow Recognition from Surgical Video (**TMI-21**) |Endoscopic Surgery |![image](https://github.com/user-attachments/assets/5da08fd6-eb30-46e6-a33f-b477f464684f) | [Link](https://arxiv.org/pdf/2103.16327) | [Code](https://github.com/YuemingJin/TMRNet) | Vision |
| Trans-SVNet: Accurate Phase Recognition from Surgical Videos via Hybrid Embedding Aggregation Transformer (**MICCAI-21**) |Endoscopic Surgery | ![image](https://github.com/user-attachments/assets/26e5a64b-4628-4970-ab52-8700c4c3ef6a)| [Link](https://arxiv.org/pdf/2103.09712) | [Code](https://github.com/xjgaocs/Trans-SVNet) | Vision |
| Federated Cycling (FedCy): Semi-supervised Federated Learning of Surgical Phases (**TMI-22**) |Endoscopic Surgery | ![image](https://github.com/user-attachments/assets/80934215-3edb-4d85-b714-5ae8c8f4a455) | [Link](https://arxiv.org/pdf/2203.07345) | | Vision |
| SKiT: a Fast Key Information Video Transformer for Online Surgical Phase Recognition (**ICCV-23**) |Endoscopic Surgery | ![image](https://github.com/user-attachments/assets/3a8cd25d-abfd-499a-bf68-16b62fcf34da) | [Link](https://openaccess.thecvf.com/content/ICCV2023/papers/Liu_SKiT_a_Fast_Key_Information_Video_Transformer_for_Online_Surgical_ICCV_2023_paper.pdf) | [Code](https://github.com/MRUIL/SKiT) | Vision |
| Surgformer: Surgical Transformer with Hierarchical Temporal Attention for Surgical Phase Recognition (**MICCAI-24**) |Endoscopic Surgery | ![image](https://github.com/user-attachments/assets/5f03c2d0-ede0-4ece-be2a-6203d6d15812) | [Link](https://arxiv.org/pdf/2408.03867) | [Code](https://github.com/isyangshu/Surgformer) | Vision |
| Label-guided Teacher for Surgical Phase Recognition via Knowledge Distillation (**MICCAI-24**) |Endoscopic Surgery | ![image](https://github.com/user-attachments/assets/018579a5-d4fa-4960-850a-1b4753f8f861) | [Link](https://papers.miccai.org/miccai-2024/paper/1997_paper.pdf) | | Vision |
| EgoSurgery-Phase: A Dataset of Surgical Phase Recognition from Egocentric Open Surgery Videos (**MICCAI-24**) |Egocentric Open Surgery | <img width="727" alt="image" src="https://github.com/user-attachments/assets/7c45a776-8c71-4d37-accf-08d6fcf9a936"> | [Link](https://www.arxiv.org/pdf/2405.19644) | [Code](https://github.com/Fujiry0/EgoSurgery) | Vision |
| HecVL: Hierarchical Video-Language Pretraining for Zero-shot Surgical Phase Recognition  (**MICCAI-24**) | Endoscopic Surgery | ![image](https://github.com/user-attachments/assets/84640ba3-043b-4ca4-b1c0-24ee8f4e3598) | [Link](https://papers.miccai.org/miccai-2024/paper/1025_paper.pdf) |  | Vision-Language |
| Jumpstarting Surgical Computer Vision  (**MICCAI-24**) | Endoscopic Surgery | ![image](https://github.com/user-attachments/assets/9a65de04-2669-498d-9f92-174b3d0b3c48) | [Link](https://papers.miccai.org/miccai-2024/paper/1998_paper.pdf) |  | Vision |
| SPRMamba: Surgical Phase Recognition for Endoscopic Submucosal Dissection with Mamba | Endoscopic Surgery | <img width="838" alt="image" src="https://github.com/user-attachments/assets/b325ffa9-04a8-4d65-b602-85b82fbe1b6c" /> | [Link](https://arxiv.org/pdf/2409.12108v1) | | Vision |
| SR-Mamba: Effective Surgical Phase Recognition with State Space Model | Endoscopic Surgery | ![image](https://github.com/user-attachments/assets/f0bd8285-472e-4d89-8329-44f9ac3ee8b9) | [Link](https://arxiv.org/pdf/2407.08333) | [Code](https://github.com/rcao-hk/SR-Mamba) | Vision |
| LoViT: Long Video Transformer for surgical phase recognition  (**MIA-25**) | Endoscopic Surgery | ![image](https://github.com/user-attachments/assets/951b8b2a-968b-435b-b650-1a2b2463f027) | [Link](https://www.sciencedirect.com/science/article/pii/S1361841524002913) | [Code](https://github.com/MRUIL/LoViT) | Vision |
| Surgical Video Workflow Analysis via Visual-Language Learning  (**npj-under review**) | Endoscopic Surgery | ![image](https://github.com/user-attachments/assets/e5407ed5-e697-4edd-89d4-4a0d0976d7c5) | [Link](https://www.researchsquare.com/article/rs-5205336/v1) | [Code](https://github.com/halamadrid-lpp/Surgical-video-workflow-analysis-I2TM) | Vision-Language |
| Neural Finite-State Machines for Surgical Phase Recognition | Endoscopic Surgery | ![image](https://github.com/user-attachments/assets/d9aef4f3-43de-42b2-97c6-e19e97687e55) | [Link](https://www.arxiv.org/pdf/2411.18018) | | Vision |
| SWAG: Long-term Surgical Workflow Prediction with Generative-based Anticipation | | <img width="838" alt="image" src="https://github.com/user-attachments/assets/cd52bc9c-fd5c-4831-acba-ee3298f2359a" /> | [Link](https://arxiv.org/pdf/2412.18849) | [Code](https://maxboels.github.io/swag) | Vision |
| Benchmarking and Enhancing Surgical Phase Recognition Models for Robotic-Assisted Esophagectomy | | <img width="1062" alt="image" src="https://github.com/user-attachments/assets/53efa181-93c2-49af-b89e-61f6f6b278dc" /> | [Link](https://arxiv.org/pdf/2412.04039) | | Vision |



### Surgical Triplet Recognition
| Paper | Surgery | Image | Link | Code | Type |
| :-------- | :---- | :---- | :-------- | :-------- | :-------- |
| Tail-Enhanced Representation Learning for Surgical Triplet Recognition | Endoscopic Surgery | ![image](https://github.com/user-attachments/assets/a43c5fed-a607-4b8f-92f1-a8d68397195b)| [Link](https://papers.miccai.org/miccai-2024/paper/0026_paper.pdf) | [Code](https://github.com/CIAM-Group/ComputerVision_Codes/tree/main/TERL) | Vision |

### Surgical Tool Detection
| Paper | Surgery | Image | Link | Code | Type |
| :-------- | :---- | :---- | :-------- | :-------- | :-------- |
| EgoSurgery-Tool: A Dataset of Surgical Tool and Hand Detection from Egocentric Open Surgery Videos | Endoscopic Surgery | ![image](https://github.com/user-attachments/assets/1519bb1a-4eb3-4246-960e-6d74c66e67bf) | [Link](https://arxiv.org/pdf/2406.03095) | [Code](https://github.com/Fujiry0/EgoSurgery) | Vision |

### Segmentation
| Paper | Surgery | Image | Link | Code | Type |
| :-------- | :---- | :---- | :-------- | :-------- | :-------- |
| Image Compositing for Segmentation of Surgical Tools without Manual Annotations (**TMI-21**) | Endoscopic Surgery | ![image](https://github.com/user-attachments/assets/c40945f5-fd05-4295-8843-12d914394df0) | [Link](https://arxiv.org/pdf/2102.09528) | [Code](https://github.com/luiscarlosgph/semi-synthetic) | Vision |

### Surgical Scene Reconstruction
| Paper | Surgery | Image | Link | Code | Type |
| :-------- | :---- | :---- | :-------- | :-------- | :-------- |
| Neural Rendering for Stereo 3D Reconstruction of Deformable Tissues in Robotic Surgery (**MICCAI-22**) | Endoscopic Surgery | ![image](https://github.com/user-attachments/assets/f7ed9a07-3083-4840-8f02-213f793f3318) | [Link](https://arxiv.org/pdf/2206.15255)| [Code](https://github.com/med-air/EndoNeRF?tab=readme-ov-file) | Vision |
| EndoSurf: Neural Surface Reconstruction of Deformable Tissues with Stereo Endoscope Videos (**MICCAI-23 Oral**) | Endoscopic Surgery | ![image](https://github.com/user-attachments/assets/22dabb83-4d3b-4310-8d16-8b78680fbe05) | [Link](https://arxiv.org/pdf/2307.11307) | [Code](https://github.com/Ruyi-Zha/endosurf) | Vision |
| Deform3DGS: Flexible Deformation for Fast Surgical Scene Reconstruction with Gaussian Splatting (**MICCAI-24**) | Endoscopic Surgery | ![image](https://github.com/user-attachments/assets/18ebd8a6-b6ed-42cf-aa2f-17d52a5f5616) | [Link](https://arxiv.org/pdf/2405.17835) | [Code](https://github.com/jinlab-imvr/Deform3DGS) | Vision |
| Free-SurGS: SfM-Free 3D Gaussian Splatting for Surgical Scene Reconstruction (**MICCAI-24**) | Endoscopic Surgery | ![image](https://github.com/user-attachments/assets/6920425f-a7b7-4b60-8224-90a4714de1c9) | [Link](https://papers.miccai.org/miccai-2024/paper/1818_paper.pdf) | [Code](https://github.com/wrld/Free-SurGS) | Vision |
| LGS: A Light-weight 4D Gaussian Splatting for Efficient Surgical Scene Reconstruction (**MICCAI-24**) | Endoscopic Surgery | ![image](https://github.com/user-attachments/assets/4028ad49-ea1f-4d55-ba20-c5881bd9cd9f) | [Link](https://arxiv.org/pdf/2406.16073) | [Code](https://github.com/CUHK-AIM-Group/LGS) | Vision |
| SurgicalGaussian: Deformable 3D Gaussians for High-Fidelity Surgical Scene Reconstruction (**MICCAI-24**) | Endoscopic Surgery | ![image](https://github.com/user-attachments/assets/d47b5ccc-f9d1-4420-98bc-e9b39f1db594) | [Link](https://arxiv.org/pdf/2407.05023) | [Code](https://surgicalgaussian.github.io/) | Vision |

### Surgical Video Generation
| Paper | Surgery | Image | Link | Code | Type |
| :-------- | :---- | :---- | :-------- | :-------- | :-------- |
| See, Predict, Plan: Diffusion for Procedure Planning in Robotic Surgical Videos (**MICCAI-24**) | Endoscopic Surgery | ![image](https://github.com/user-attachments/assets/79d5788a-ac25-4fec-8102-068c3f4dc73e) | [Link](https://papers.miccai.org/miccai-2024/paper/2373_paper.pdf) | | Vision |

### Surgical VQA
| Paper | Surgery | Image | Link | Code | Type |
| :-------- | :---- | :---- | :-------- | :-------- | :-------- |
| Surgical-VQA: Visual Question Answering in Surgical Scenes using Transformer (**MICCAI-22**) | Endoscopic Surgery | ![image](https://github.com/user-attachments/assets/6c6fe2c8-bfb1-49a5-8c2a-6d0367053d39) | [Link](https://arxiv.org/pdf/2206.11053) | [Code](https://github.com/lalithjets/Surgical_VQA.git) | Vision-Language |
| Advancing Surgical VQA with Scene Graph Knowledge (**IPCAI-24**) | Endoscopic Surgery | ![image](https://github.com/user-attachments/assets/dfb6ca09-7316-44a6-b1df-1b721f97d894) | [Link](https://arxiv.org/pdf/2312.10251) | [Code](https://github.com/CAMMA-public/SSG-VQA) | Vision-Language |

### Surgical Type Recognition
| Paper | Surgery | Image | Link | Code | Type |
| :-------- | :---- | :---- | :-------- | :-------- | :-------- |
| Future-State Predicting LSTM for Early Surgery Type Recognition (**TMI-20**) | Endoscopic Surgery | ![image](https://github.com/user-attachments/assets/b9fe3c19-7d63-4553-96c5-b3142afe1484)  | [Link](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8772203) | | Vision |

## Pretraining
### Vision Pretraining
#### GI Endoscopy
| Paper | Type | Level | Number| Method | Link | Code |
| :-------- | :---- | :---- | :-------- | :-------- | :-------- |:-------- |
| Unsupervised Segmentation of Colonoscopy Images | Colonoscope | Image-level | 525,711 (5,145 clips) | DINOv1 | [Link](https://arxiv.org/pdf/2312.12599) | |
| Arges: Spatio-Temporal Transformer for Ulcerative Colitis Severity Assessment in Endoscopy Videos | GI Endoscopy | Image-level | 61M (3,927 clips) | DINOv2 | [Link](https://link.springer.com/chapter/10.1007/978-3-031-73290-4_20) | |
| Foundation Model for Endoscopy Video Analysis via Large-Scale Self-supervised Pre-train | GI Endoscopy (little laparoscope) | Video-level | 5M (32,896 clips) | Endo-FM | [Link](https://link.springer.com/chapter/10.1007/978-3-031-43996-4_10) | [Code](https://github.com/med-air/Endo-FM) |
| Self-Supervised Learning for Endoscopy Video Analysis | Colonoscope | Image-level | 2.2M (13,979 clips) | MSN | [Link](https://arxiv.org/pdf/2308.12394) | [Code](https://github.com/RoyHirsch/endossl)|
| EndoDINO: A Foundation Model for GI Endoscopy | GI Endoscopy | Image-level | 10M (130,037 clips) | DINOv2 | [Link](https://arxiv.org/pdf/2501.05488) | |
| EndoMamba: An Efficient Foundation Model for Endoscopic Videos via Hierarchical Pre-training | GI + Laparoscope + Bronchoscopy | Video-level| 11M (74,828 clips) | EndoMamba | [Link](https://arxiv.org/pdf/2502.19090) | |
|Improving Foundation Model for Endoscopy Video Analysis via Representation Learning on Long Sequences| GI Endoscopy | Video-level | 13M (6469 clips) | EndoFM-VL | [Link](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10885043) | [Code](https://github.com/med-air/EndoFM-LV)|

#### Endoscopic Surgery
| Paper | Type | Level | Number | Method | Link | Code |
| :-------- | :---- | :---- | :-------- | :-------- | :-------- |:-------- |
| Dissecting Self-Supervised Learning Methods for Surgical Computer Vision | Cholec80 | Image-level | 9.8k | DINO/MoCo v2/SimCLR/SwAV | [Link](https://arxiv.org/pdf/2207.00449) | [Code](https://github.com/CAMMA-public/SelfSupSurg) | 
| EndoViT: pretraining vision transformers on a large collection of endoscopic images | Laparoscopic Procedures | Image-level | 700k | MAE | [Link](https://link.springer.com/article/10.1007/s11548-024-03091-5?utm_source=rct_congratemailt&utm_medium=email&utm_campaign=oa_20240403&utm_content=10.1007/s11548-024-03091-5) | [Code](https://github.com/DominikBatic/EndoViT/tree/main?tab=readme-ov-file) |
 | Self-Supervised Learning for Endoscopic Video Analysis | Laparoscopic Procedures | Image-level | 23M (7,877 clips) | MSN | [Link](https://arxiv.org/pdf/2308.12394) | [Code](https://github.com/RoyHirsch/endossl) |
 | General surgery vision transformer: A video pre-trained foundation model for general surgery | Endoscopic Procedures | Image-level | 2.4M (3000+ clips) | GSViT | [Link](https://arxiv.org/pdf/2403.05949) | [Code](https://github.com/SamuelSchmidgall/GSViT)|
 | Scaling up self-supervised learning for improved surgical foundation models | Endoscopic Procedures | Image-level | 4.7M | DINO | [Link](https://arxiv.org/pdf/2501.09436#page=8.75) | [Code](https://github.com/TimJaspers0801/SurgeNet) |


### Vision-Language Pretraining

| Paper | Type | Level | Number | Image | Link | Code | 
| :-------- | :---- | :---- | :---- | :-------- | :-------- | :-------- |
| OphCLIP: Hierarchical Retrieval-Augmented Learning for Ophthalmic Surgical Video-Language Pretraining | Ophthalmic Surgery | Video-level | 44,290 Clips / 960M Images / 375K Pairs | ![image](https://github.com/user-attachments/assets/bb5a9757-607b-478b-92a2-2594fb10139a)  | [Link](https://arxiv.org/pdf/2411.15421) | [Code](https://github.com/minghu0830/OphCLIP) |

### LLM-based VLM
| Paper | Type | Level| Number| Image | Link | Code |
| :-------- | :---- | :---- | :---- | :-------- | :-------- | :-------- |
| LLaVA-Surg: Towards Multimodal Surgical Assistant via Structured Surgical Video Learning | Endoscopic Surgery | ![image](https://github.com/user-attachments/assets/6cce549b-8e2f-428f-9540-5f515fa12a9a) | [Link](https://arxiv.org/pdf/2408.07981v1) | | Vision-Language |
| Surgical-LLaVA: Toward Surgical Scenario Understanding via Large Language and Vision Models | Endoscopic Surgery | ![image](https://github.com/user-attachments/assets/d934a2c6-7e8a-48f5-bc97-e251941eb543) | [Link](https://arxiv.org/pdf/2410.09750) | | Vision-Language |
| EndoChat: Grounded Multimodal Large Language Model for Endoscopic Surgery |  Endoscopic Surgery | Image-level | 41K images / 396K instruction-following annotation | <img width="728" alt="image" src="https://github.com/user-attachments/assets/6ed376d9-6027-4896-873d-a5dc64b0f5b9" /> |[Link](https://arxiv.org/pdf/2501.11347)| [Code](https://github.com/gkw0010/EndoChat)|


## Comprehensive Journals
| Paper | Journal | Image | Link | Code |
| :-------- | :---- | :---- | :-------- | :-------- |
| Surgical gestures as a method to quantify surgical performance and predict patient outcomes (Dani Kiyasseh et al.) | npj Digital Medicine 2022 | ![image](https://github.com/user-attachments/assets/143530fb-74e3-4eb2-b4ee-4941baa5da52) | [Link](https://www.nature.com/articles/s41746-022-00738-y) | [Code](https://github.com/crseusc/NS-Gestures-and-EF-outcomes)|
| A vision transformer for decoding surgeon activity from surgical videos (Dani Kiyasseh et al.) | Nature Biomedical Engineering 2023 | <img width="652" alt="image" src="https://github.com/user-attachments/assets/b1454abc-e92b-4418-be67-850c5fe50ef7"> | [Link](https://www.nature.com/articles/s41551-023-01010-8) | [Code](https://github.com/danikiyasseh/SAIS)|
| Human visual explanations mitigate bias in AI-based assessment of surgeon skills (Dani Kiyasseh et al.) | npj Digital Medicine 2023 | ![image](https://github.com/user-attachments/assets/fc872ded-3e20-47d8-b01e-cec80f232ff4) | [Link](https://www.nature.com/articles/s41746-023-00766-2) | [Code](https://github.com/danikiyasseh/TWIX)|


