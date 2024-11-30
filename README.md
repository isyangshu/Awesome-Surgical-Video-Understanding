# Awesome-Surgical-Video-Understanding
There are compilations of surgery-related tasks, datasets, and papers.

## Contents
- [Dataset](#dataset)
  - [Endoscopic Surgery](#endoscopic-surgery)
    - [Public Dataset](#public-dataset)
    - [Private Dataset](#private-dataset)
  - [Egocentric Open Surgery](#egocentric-open-surgery)
  - [Ophthalmic Surgery](#ophthalmic-surgery)
- [Paper](#paper)
  - [Surgical Phase Recognition](#surgical-phase-recognition)
  - [Surgical Triplet Recognition](#surgical-triplet-recognition)
  - [Surgical Tool Detection](#surgical-tool-detection)
  - [Segmentation](#segmentation)
  - [Surgical Scene Reconstruction](#surgical-scene-reconstruction)
  - [Surgical Video Generation](#surgical-video-generation)
  - [Surgical VQA](#surgical_vqa)
  - [Surgical Type Recognition](#surgical_type_recognition)

## Dataset

### Endoscopic Surgery

#### Public Dataset

| Dataset| Paper | Link | Procedure | Task | Type |
| :-------- | :---- | :-------- | :-------- |  :-------- |  :-------- |
| Cholec80 | [Paper](https://arxiv.org/pdf/1602.03012)| [Link](https://camma.unistra.fr/datasets/) | Cholecystectomy Surgery | Surgical Phase Recognition | Video-level |
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


### Egocentric Open Surgery
| Dataset| Paper | Link | Type | Task |
| :-------- | :---- | :-------- | :-------- |  :-------- |
| EgoSurgery-Tool | [Paper](https://arxiv.org/pdf/2406.03095)| [Link](https://github.com/Fujiry0/EgoSurgery) | Distinct Surgical Procedures | Surgical Tool/Hand Detection |
| EgoSurgery-Phase | [Paper](https://www.arxiv.org/pdf/2405.19644) | [Link](https://github.com/Fujiry0/EgoSurgery)  | Distinct Surgical Procedures | Surgical Phase Recognition |

## Paper
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
| LoViT: Long Video Transformer for surgical phase recognition  (**MIA-25**) | Endoscopic Surgery | ![image](https://github.com/user-attachments/assets/951b8b2a-968b-435b-b650-1a2b2463f027) | [Link](https://www.sciencedirect.com/science/article/pii/S1361841524002913) | [Code](https://github.com/MRUIL/LoViT) | Vision |
| Surgical Video Workflow Analysis via Visual-Language Learning  (**npj-under review**) | Endoscopic Surgery | ![image](https://github.com/user-attachments/assets/e5407ed5-e697-4edd-89d4-4a0d0976d7c5) | [Link](https://www.researchsquare.com/article/rs-5205336/v1) | [Code](ttps://github.com/halamadrid-lpp/Surgical-video-workflow-analysis-I2TM) | Vision-Language |

### Surgical Triplet Recognition
| Paper | Surgery | Image | Link | Code | Type |
| :-------- | :---- | :---- | :-------- | :-------- | :-------- |
| Tail-Enhanced Representation Learning for Surgical Triplet Recognition | Endoscopic Surgery | ![image](https://github.com/user-attachments/assets/a43c5fed-a607-4b8f-92f1-a8d68397195b)| [Link](https://papers.miccai.org/miccai-2024/paper/0026_paper.pdf) | [Code](https://github.com/CIAM-Group/ComputerVision_Codes/tree/main/TERL) | Vision |

### Surgical Tool Detection
| Paper | Surgery | Image | Link | Code | Type |
| :-------- | :---- | :---- | :-------- | :-------- | :-------- |
| EgoSurgery-Tool: A Dataset of Surgical Tool and Hand Detection from Egocentric Open Surgery Videos | Endoscopic Surgery | ![image](https://github.com/user-attachments/assets/1519bb1a-4eb3-4246-960e-6d74c66e67bf) | [Link](https://arxiv.org/pdf/2406.03095) | [Code](https://github.com/Fujiry0/EgoSurgery) | Vision |

### Segmentation

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


