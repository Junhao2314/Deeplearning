# Deep Learning for Remote Sensing 🛰️

本仓库收集深度学习在遥感图像处理领域的最新研究成果。

---

## 📋 论文汇总表格

<div align="center">

| **序号** | **论文标题** | **期刊** | **年份** | **主要内容** | **DOI链接** |
|---------|-------------|---------|---------|-------------|-------------|
| **1** | Advancing Plain Vision Transformer Toward Remote Sensing Foundation Model | IEEE TGRS | 2022 | 提出约1亿参数的遥感ViT大模型，引入旋转可变窗口注意力(RVSA)机制处理遥感图像大尺寸和任意方向目标；在DOTA-V1.0检测任务达81.24% mAP，超越所有SOTA模型，展现出优异的计算效率和迁移学习能力 | [🔗](https://doi.org/10.48550/arxiv.2208.03987) |
| **2** | SkySense: A Multi-Modal Remote Sensing Foundation Model Towards Universal Interpretation for Earth Observation Imagery | CVPR | 2024 | 构建迄今最大的多模态遥感基础模型(20亿参数)，在2150万时序序列数据上预训练；提出因式分解时空编码器、多粒度对比学习和地理上下文原型学习，在16个数据集7类任务全面超越18个SOTA模型，平均领先2.5%+ | [🔗](https://doi.org/10.48550/arXiv.2312.10115) |
| **3** | GeoChat: Grounded Large Vision-Language Model for Remote Sensing | CVPR | 2024 | 首个遥感VLM对话模型，解决通用VLM在遥感场景表现不佳问题；支持图像级和区域级查询、视觉定位回答，在图像/区域描述、VQA、场景分类、定位对话和指代检测等任务展现强大零样本性能 | [🔗](https://doi.org/10.48550/arXiv.2311.15826) |
| **4** | Mobile-Seed: Joint Semantic Segmentation and Boundary Detection for Mobile Robots | IEEE RA-L | 2024 | 提出轻量化多任务学习框架Mobile-Seed，同步执行语义分割和边缘检测；采用双分支编码器、主动融合解码器(AFD)和多任务一致性约束，在Cityscapes上mIoU提升2.2%、mF-score提升4.2%，1024×2048分辨率下保持23.9 FPS实时效率 | [🔗](https://ieeexplore.ieee.org/document/10461032) |
| **5** | A semantic-enhanced multi-modal remote sensing foundation model for Earth observation | Nature MI | 2025 | SkySense++升级版，发表于Nature Machine Intelligence(IF=23.9)；基于2700万多模态图像的两阶段渐进预训练，支持In-context Learning少样本能力；在12个EO任务7个领域(农业/林业/海洋学等)超越SOTA，实现时敏场景快速响应 | [🔗](https://www.nature.com/articles/s42256-025-01078-8) |
| **6** | Domain Generalization for Semantic Segmentation of Remote Sensing Images via Vision Foundation Model Fine-tuning | ISPRS JPRS | 2025 | 系统评估多种VFM在遥感跨域分割中的泛化，确认DINO v2 ViT‑L表现领先；据此提出GeoSA（增强器‑桥接器‑提取器）与BaSA批级风格增强，在冻结/少量调参下提升域不变性，跨多数据与设置均显著优于现有DG与VFM微调方法 | [🔗](https://doi.org/10.1016/j.isprsjprs.2025.09.004) |
| **7** | Global Urban High-resolution Scene Classification via Uncertainty-aware Domain Generalization | ISPRS JPRS | 2025 | 构建DGUS数据集并提出UADG框架：以城市相关白化（CRW）缓解跨城风格差异，以不确定性引导专家分配（UAE）应对长尾；在未见域上较GAMMA的OA/AA分别提升9.79%/7.42% | [🔗](https://doi.org/10.1016/j.isprsjprs.2025.08.027) |
| **8** | REST: Holistic Learning for End-to-End Semantic Segmentation of Whole-Scene Remote Sensing Imagery | IEEE TPAMI | 2025 | 提出首个真正端到端的整幅遥感影像（WRI）分割框架REST；引入空间并行交互机制（SPIM）结合并行与分而治之以突破显存并获得全局感知，支持即插即用的编码器/解码器与基础模型；随GPU数近线性扩展并在多场景显著优于裁剪/融合范式 | [🔗](https://doi.org/10.1109/TPAMI.2025.3609767) |
| **9** | Multi-E2E: An end-to-end urban land-use mapping framework integrating high-resolution remote sensing images and multi-source geographical data | Remote Sensing of Environment | 2025 | 提出端到端城市土地利用制图框架Multi-E2E，融合高分辨率遥感图像与POIs多源地理数据；引入知识注入图卷积网络（KD-GCN）建模POI空间关系，设计自适应融合模块（AFM）实现跨模态特征融合，单模态监督模块（USM）处理POI缺失情况；在34座中国城市及跨国验证泛化性 | [🔗](https://doi.org/10.1016/j.rse.2025.114966) |
| **10** | Global high categorical resolution land cover mapping via weak supervision | ISPRS JPRS | 2025 | 提出PRE方法，首次将原型引导的伪标签校正与扩展用于弱监督领域自适应(WSDA)；联合稠密标注源域与稀疏标注目标域，实现全球尺度高分辨率细分类土地覆盖制图(24类)；跨传感器、跨类别、跨大陆适应，在10个全球城市准确率超80% | [🔗](https://doi.org/10.1016/j.isprsjprs.2024.12.017) |
| **11** | DeH4R: A Decoupled and Hybrid Method for Road Network Graph Extraction | arXiv | 2025 | 提出首个结合graph-generating高效性与graph-growing动态性的混合路网提取框架；通过解耦四阶段(候选顶点检测、相邻顶点预测、初始图构建、图扩展)实现动态顶点插入，比RNGDet++快约10倍且在CityScale上APLS提升4.62、IoU提升10.18 | [🔗](https://www.arxiv.org/abs/2508.13669) |

</div>

---

## 📊 遥感大模型对比总结

<div align="center">

| **维度** | **RSVA (2022)** | **SkySense (2024)** | **SkySense++ (2025)** | **GeoChat (2024)** |
|---------|----------|--------------|-------------|-------------|
| **模态** | 可见光 | RGB+SAR+时序 | 高分辨率光学+Sentinel-2+Sentinel-1 | RGB (+可扩展) |
| **参数量** | 1亿 | 20亿 | 未公布 | 7B LLM + ViT |
| **最强技能** | 旋转检测 | 多模态融合 | In-context Learning | 对话&定位 |
| **下游成本** | 微调1-2小时 | 零样本/微调皆可 | 几乎无标注 | 零样本对话 |
| **一句话总结** | ViT的遥感特化版 | 遥感界的GPT-4V | 语义增强的少样本学习王者 | 让卫星开口说话 |

</div>

---

## 📚 论文列表

### 1. Domain Generalization for Semantic Segmentation of Remote Sensing Images via Vision Foundation Model Fine-tuning

<div align="center">

| **属性** | **内容** |
|---------|---------|
| **期刊** | ISPRS Journal of Photogrammetry and Remote Sensing |
| **年份** | 2025 |
| **单位** | 武汉大学，墨尔本大学 |
| **论文链接** | [📄 DOI: 10.1016/j.isprsjprs.2025.09.004](https://doi.org/10.1016/j.isprsjprs.2025.09.004) |
| **代码仓库** | [💻 GitHub: GeoSA-BaSA](https://github.com/mmmll23/GeoSA-BaSA) |

</div>

#### 🔬 主要创新点

- **🎯 系统性评估**: 首次系统评估多种视觉基础模型(VFMs)在遥感跨域语义分割任务中的泛化能力，发现冻结的DINO v2 ViT-L无需微调即可显著超越传统骨干网络和专门的域泛化方法

- **🧩 地理空间语义适配器(GeoSA)**: 提出创新的适配器架构，通过以下三个协同子模块实现冻结VFM向遥感图像的高效参数化适配：
  - **增强器**: 特征增强处理
  - **桥接器**: 跨域特征连接
  - **提取器**: 关键信息提取

- **🌊 批量风格增强器(BaSA)**: 设计新颖的频域适应技术，实现在线、无参数的批级别风格混合，有效减少对特定域风格的依赖

- **📊 综合评估框架**: 构建涵盖二分类和多类别、不同地理区域和传感器平台的域泛化评估框架，为VFM在遥感领域的应用提供系统性基准

---

### 2. Global Urban High-resolution Scene Classification via Uncertainty-aware Domain Generalization

<div align="center">

| **属性** | **内容** |
|---------|---------|
| **期刊** | ISPRS Journal of Photogrammetry and Remote Sensing |
| **年份** | 2025 |
| **单位** | 武汉大学，东京大学，信息工程大学 |
| **论文链接** | [📄 DOI: 10.1016/j.isprsjprs.2025.08.027](https://doi.org/10.1016/j.isprsjprs.2025.08.027) |

</div>

#### 🔬 主要创新点

- **🏙️ 新数据集构建 - DGUS**: 
  - 提出Domain Generalized Urban Scene (DGUS)数据集，专门用于全球城市场景分类的域泛化研究
  - 包含42个城市场景类别，具有长尾分布特征和跨城市域差异

- **🎨 城市相关白化变换(CRW)**:
  - 改进传统白化变换，不是简单去除风格信息，而是选择性保留城市相关的语义信息
  - 通过风格选择机制保留有价值的城市特征，增强特征判别能力

- **🤖 不确定性感知专家(UAE)**:
  - 基于Dempster-Shafer理论估计场景不确定性
  - 根据不确定性动态分配专家数量：
    - 尾部类别(高不确定性) → 分配更多专家
    - 头部类别 → 分配较少专家

---

### 3. REST: Holistic Learning for End-to-End Semantic Segmentation of Whole-Scene Remote Sensing Imagery

<div align="center">

| **属性** | **内容** |
|---------|---------|
| **期刊** | IEEE Transactions on Pattern Analysis and Machine Intelligence (IF = 18.6，中科院一区top) |
| **年份** | 2025 |
| **单位** | 武汉大学，特伦托大学，康奈尔大学，华南理工大学等 |
| **通讯作者** | Yansheng Li |
| **论文链接** | [📄 DOI: 10.1109/TPAMI.2025.3609767](https://doi.org/10.1109/TPAMI.2025.3609767) |
| **项目主页** | [🌐 REST Project](https://weichenrs.github.io/REST) |

</div>

#### 🔬 主要创新点

- **🚀 首个真正的"端到端"全景分割框架(REST)**:
  - REST是第一个能够直接对整幅遥感影像进行整体处理和分割的端到端框架，彻底摆脱了传统方法对图像进行裁剪或融合的依赖
  - 具有"即插即用"的特性，能够无缝集成各种主流的编码器-解码器架构：
    - **Swin Transformer**: 层次化视觉Transformer
    - **ConvNeXt**: 现代化卷积网络
    - **遥感基础模型**: 最新的领域特定模型

- **⚡ 空间并行交互机制(SPIM)**:
  - SPIM是REST框架的核心，采用"分而治之"与并行计算相结合的策略，克服单块GPU的显存瓶颈
  - 能有效地在多GPU之间聚合全局上下文信息，确保模型在处理局部区域时也能拥有全局视野
  - 理论和实验均证明：随着GPU数量增加，REST的处理吞吐量（可处理的图像尺寸）能实现近乎线性的扩展

---

### 4. Multi-E2E: An end-to-end urban land-use mapping framework integrating high-resolution remote sensing images and multi-source geographical data

<div align="center">

| **属性** | **内容** |
|---------|---------|
| **期刊** | Remote Sensing of Environment |
| **年份** | 2025 |
| **单位** | 武汉大学，信息工程大学 |
| **论文链接** | [📄 DOI: 10.1016/j.rse.2025.114966](https://doi.org/10.1016/j.rse.2025.114966) |
| **代码仓库** | [💻 GitHub: Multi_E2E](https://github.com/Rayoll/Multi_E2E) |

</div>

#### 🔬 主要创新点

- **🏗️ Multi-E2E框架**: 提出端到端城市土地利用制图框架，创新性融合高分辨率遥感图像（HRS）和多源地理数据（特别是POIs），通过数据驱动方法自动建立多源数据到土地利用类别的映射关系

- **🧠 知识注入图卷积网络(KD-GCN)**: 结合POI的空间分布和语义特征进行建图，有效保留POI之间的空间关系，克服现有方法无法自动捕捉多源数据与土地利用类别复杂关系的局限

- **🔄 自适应融合模块(AFM)**: 设计跨模态注意力机制，解决HRS图像与POIs之间的显著语义差异问题，实现图像与POI特征的有效融合并提取互补信息

- **🛡️ 单模态监督模块(USM)**: 创新性地使模型能够在POI缺失情况下依然执行土地利用分类，无需重新训练，打破了现有方法对完整模态的假设依赖

- **🌏 跨域泛化验证**: 在中国34座城市以及北京、武汉、香港、澳门、芬兰赫尔辛基等多个跨国城市上验证了框架的有效性和泛化能力

---

### 8. Global high categorical resolution land cover mapping via weak supervision

<div align="center">

| **属性** | **内容** |
|---------|---------|
| **期刊** | ISPRS Journal of Photogrammetry and Remote Sensing |
| **年份** | 2025 |
| **单位** | 慕尼黑工业大学，清华大学 |
| **核心任务** | 全球高分辨率土地覆盖制图 |
| **论文链接** | [📄 DOI: 10.1016/j.isprsjprs.2024.12.017](https://doi.org/10.1016/j.isprsjprs.2024.12.017) |
| **项目主页** | [🌐 PRE Land Cover](https://zhu-xlab.github.io/PRE-land-cover.html) |
| **一句话亮点** | 首次实现基于弱监督的全球尺度高类别分辨率土地覆盖制图，24类分类准确率超80% |

</div>

#### 🔬 主要创新点

- **🔄 PRE弱监督域适应方法**: 首次将"原型引导的伪标签校正与扩展"(Prototype-based pseudo-label Rectification and Expansion, PRE)用于弱监督领域自适应(WSDA)，实现细粒度土地覆盖制图的突破性进展

- **📊 联合标注策略**: 创新性结合稠密标注源域与稀疏标注目标域，突破传统UDA(无标签目标域)和WSSS(弱标签)方法的限制，显著提升跨域适应能力和标注效率

- **🧠 原型引导机制**: 利用类别特征质心作为原型，构建稀疏标签与全局特征分布之间的桥梁；根据特征到原型的距离评估目标域未标注区域伪标签的置信度，指导动态扩展和校正

- **🌍 全球弱监督数据集**: 构建涵盖中国五个城市(C-megacities)和全球五个城市(G-cities)的挑战性数据集，实现跨传感器(PlanetScope、Gaofen-1、Sentinel-2)、跨类别、跨大陆的综合验证

- **🎯 高分辨率细分类制图**: 首次实现基于弱标注的全球尺度、高类别分辨率土地覆盖图(24类)，为联合国可持续发展目标的经济生计追踪和环境退化测量提供精确支撑

- **📈 卓越跨域性能**: 在10个全球不同区域城市实现跨传感器、跨类别、跨大陆的WSDA，总体准确率超过80%，显著减少对高质量标注的依赖，提升标注效率

- **🌱 环境监测应用**: 为全球精细土地覆盖制图奠定基础，推动地球观测为环境监测提供更精确、全面的信息支持，助力可持续发展目标实现

---

## 🌍 遥感基础大模型

### 5. RSVA: Advancing Plain Vision Transformer Toward Remote Sensing Foundation Model

<div align="center">

| **属性** | **内容** |
|---------|---------|
| **期刊** | IEEE Transactions on Geoscience and Remote Sensing |
| **年份** | 2022 |
| **参数量** | 1亿参数 |
| **核心技术** | 旋转可变窗口注意力(RVSA) |
| **论文链接** | [📄 DOI: 10.48550/arxiv.2208.03987](https://doi.org/10.48550/arxiv.2208.03987) |
| **代码仓库** | [💻 GitHub: remote-sensing-rvs](https://github.com/ViTAE-Transformer/remote-sensing-rvs) |
| **一句话亮点** | 用"旋转+变尺寸"窗口把ViT改造成遥感专用视觉引擎，DOTA检测mAP直接干到81.24% |

</div>

#### 🔬 主要创新点

- **🌀 旋转可变窗口注意力(RVSA)**: 为处理遥感图像中的大尺寸和任意方向目标，提出旋转可变尺寸窗口注意力机制，替代传统Transformer的全注意力；显著减少计算成本和内存占用，同时通过多样化窗口提取丰富上下文来学习更好的目标表示

- **📐 遥感图像适应性设计**: 专门针对遥感图像的独特挑战进行结构优化：
  - **高分辨率处理**: 有效处理大尺寸遥感图像
  - **任意方向目标**: 适应遥感图像中目标的多向性
  - **多尺度特征**: 通过变尺寸窗口捕获不同尺度的语义信息

- **� 检测性能突破**: 在DOTA-V1.0数据集上达到81.24% mAP，超越所有现有SOTA模型，验证了大规模ViT在遥感领域的有效性

- **⚡ 计算效率优化**: 在下游分类和分割任务上展现出竞争性能的同时，在计算复杂度和数据传输效率方面表现出明显优势

- **🧬 良好的可迁移性**: 实验证明模型在迁移学习场景下具有优异的数据效率和泛化能力，为遥感大模型发展奠定了重要基础

---

### 6. SkySense: A Multi-Modal Remote Sensing Foundation Model Towards Universal Interpretation for Earth Observation Imagery

<div align="center">

| **属性** | **内容** |
|---------|---------|
| **会议** | IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) |
| **年份** | 2024 |
| **参数量** | 20亿参数 |
| **支持模态** | RGB + SAR + 时序 |
| **论文链接** | [📄 DOI: 10.48550/arXiv.2312.10115](https://doi.org/10.48550/arXiv.2312.10115) |
| **代码仓库** | [💻 GitHub: SkySense](https://github.com/Jack-bo1220/SkySense) |
| **后续版本** | [🔗 SkySense++](https://github.com/kang-wu/SkySensePlusPlus) |
| **一句话亮点** | 20亿参数的"多模态地球翻译官"，多云天气也能精准识别水稻田 |

</div>

#### 🔬 主要创新点

- **🧩 因式分解的多模态时空编码器**: 在包含2150万时序序列的多模态遥感数据集上预训练，采用因式分解架构处理光学和SAR时序数据，模块化设计支持灵活组合以适应各种任务需求

- **🔄 多粒度对比学习**: 提出跨不同模态和空间粒度的多粒度对比学习方法，在像素级、目标级、图像级进行逐层对比学习，有效捕捉从细粒到粗粒的语义特征表示

- **📍 地理上下文原型学习**: 引入地理上下文原型学习机制，在RSI的多模态时空特征基础上学习区域感知原型，通过地理上下文线索进一步增强遥感图像表示能力

- **🌦️ 全天候遥感理解**: 作为迄今为止最大的多模态遥感基础模型，能够处理多云条件下的复杂场景，实现全天候、全模态的地球观测图像理解

- **📊 全面超越现有方法**: 在涵盖16个数据集、7种任务的全面评估中超越18个最新的遥感基础模型：
  - 相比GFM平均提升2.76%
  - 相比SatLas平均提升3.67% 
  - 相比Scale-MAE平均提升3.61%
  - 从单模态到多模态、静态到时序、分类到定位任务均表现卓越

---

### 6. SkySense++: A semantic-enhanced multi-modal remote sensing foundation model for Earth observation

<div align="center">

| **属性** | **内容** |
|---------|---------|
| **期刊** | Nature Machine Intelligence (IF = 23.9，计算机科学顶级期刊) |
| **年份** | 2025 |
| **数据规模** | 2700万多模态遥感图像 |
| **支持模态** | 高分辨率光学 + Sentinel-2多光谱 + Sentinel-1雷达(SAR) |
| **论文链接** | [📄 DOI: 10.1038/s42256-025-01078-8](https://www.nature.com/articles/s42256-025-01078-8) |
| **代码仓库** | [💻 GitHub: SkySensePlusPlus](https://github.com/kang-wu/SkySensePlusPlus) |
| **单位** | 武汉大学，蚂蚁集团，中国科学技术大学 |
| **一句话亮点** | Nature MI发表的语义增强遥感大模型，支持In-context Learning少样本能力，12个EO任务7个领域全面SOTA |

</div>

#### 🔬 主要创新点

- **🏗️ 多模态因式分解架构**: SkySense++采用创新的因式分解架构，无缝整合高分辨率光学、Sentinel-2多光谱和Sentinel-1雷达(SAR)三种模态的多时相图像，通过模块化设计实现多传感器数据的统一表示学习

- **🎯 两阶段渐进预训练策略**: 
  - **表示增强预训练阶段**: 利用多粒度对比学习获取通用的多模态特征表示，建立跨模态的共享语义空间
  - **语义增强预训练阶段**: 通过掩码语义学习(MSL)结合语义信息，大幅提升模型的少样本学习和快速适应能力

- **🧠 In-context Learning能力**: 借助语义池(semantic bank)实现类别提示学习，模型可在几乎无标注的情况下处理全新任务，特别适用于时间敏感场景如快速洪水制图、灾害响应等

- **📊 全领域性能突破**: 在12个地球观测任务、7个应用领域(农业、林业、海洋学、大气科学、生物学、土地测量、灾害管理)中均超越现有SOTA模型，展现出卓越的泛化性和实用性

- **⚡ 快速响应能力**: 通过语义增强预训练和上下文学习，显著减少对大规模标注数据的依赖，能够快速适应紧急任务需求，为时效性要求极高的地球观测应用提供强大支撑

---

### 7. GeoChat: Grounded Large Vision-Language Model for Remote Sensing

<div align="center">

| **属性** | **内容** |
|---------|---------|
| **会议** | IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) |
| **年份** | 2024 |
| **基础模型** | Vicuna-7B |
| **核心能力** | 视觉定位 + 多轮问答 |
| **论文链接** | [📄 DOI: 10.48550/arXiv.2311.15826](https://doi.org/10.48550/arXiv.2311.15826) |
| **代码仓库** | [💻 GitHub: GeoChat](https://github.com/mbzuai-oryx/GeoChat) |
| **一句话亮点** | 对着卫星图直接问"东北角白色建筑是什么？"GeoChat秒回"体育馆，面积约1.8万㎡" |

</div>

#### 🔬 主要创新点

- **🌍 首个遥感专用VLM**: 针对遥感领域独特挑战设计的首个通用多模态对话模型，解决了通用VLM在遥感场景下表现不佳、产生错误或虚假信息的问题

- **🎯 视觉定位对话能力**: 独创的视觉定位功能，不仅能回答图像级查询，还能接受区域输入进行特定区域对话，并在回答中通过空间坐标指向相关目标，实现真正的"所答即所指"

- **📚 遥感多模态指令数据集**: 基于现有多样化遥感数据集扩展生成新颖的遥感多模态指令跟随数据集，涵盖：
  - **高分辨率图像处理**: 处理遥感图像的大尺寸和多尺度变化
  - **小目标识别**: 针对遥感图像中众多小目标的区域级推理
  - **场景级解释**: 整体场景理解与解释能力

- **🧠 多模态架构设计**: 
  - **图像编码器**: 使用CLIP-ViT作为视觉主干提取空间特征
  - **投影模块**: 将视觉嵌入映射到语言模型的隐藏空间
  - **语言模型**: 基于Vicuna-7B的LLaMA模型，支持复杂自然语言生成

- **�️ 零样本多任务能力**: 在遥感多任务对话基准上展现出强大的零样本性能：
  - **图像和区域描述**: 准确描述遥感场景和特定区域
  - **视觉问答**: 回答关于遥感图像的复杂问题  
  - **场景分类**: 识别和分类不同的遥感场景类型
  - **视觉定位对话**: 在对话中精确定位和引用具体目标
  - **指代检测**: 根据自然语言描述定位相应的遥感目标

---

### 9. DeH4R: A Decoupled and Hybrid Method for Road Network Graph Extraction

<div align="center">

| **属性** | **内容** |
|---------|---------|
| **预印本** | arXiv |
| **年份** | 2025 |
| **单位** | 武汉大学 |
| **核心任务** | 道路网络图提取 |
| **论文链接** | [📄 arXiv: 2508.13669](https://www.arxiv.org/abs/2508.13669) |
| **代码仓库** | [💻 GitHub: DeH4R](https://github.com/7777777FAN/DeH4R) |
| **一句话亮点** | 首次融合graph-generating与graph-growing优势，比RNGDet++快10倍且精度更高 |

</div>

#### 🔬 主要创新点

- **🔄 DeH4R混合框架**: 首次将graph-generating的高效性与graph-growing的动态性相结合，通过解耦四个关键阶段实现最优性能：
  - **候选顶点检测**: 利用SAM2进行精准的顶点候选区域识别
  - **相邻顶点预测**: 采用DETR-like架构预测顶点间的邻接关系
  - **初始图构建**: 基于预测结果构建初始道路网络图
  - **图扩展**: 动态插入遗漏的顶点和边，提升拓扑完整性

- **🚀 动态顶点插入**: 突破传统graph-generating方法无法动态补充顶点的局限，实现运行时的自适应图结构优化，显著提升道路网络的拓扑完整性和空间一致性

- **🧠 先进架构融合**: 创新性结合多种前沿技术：
  - **SAM2集成**: 利用Segment Anything Model 2进行候选顶点的精确检测
  - **DETR思路**: 采用Detection Transformer的端到端预测范式进行相邻顶点预测
  - **混合推理**: 保持快速推理速度的同时实现动态结构调整

- **⚡ 显著效率提升**: 相比现有最优graph-growing方法RNGDet++实现约10倍的速度提升，同时在拓扑精度上表现更优，解决了传统方法计算开销过大的问题

- **📊 SOTA性能表现**: 在CityScale和SpaceNet基准测试中达到最先进性能：
  - **CityScale数据集**: 相比RNGDet++在APLS指标上提升4.62，IoU指标上提升10.18
  - **拓扑保真度**: 在vectorization后处理中保持更好的拓扑一致性
  - **空间一致性**: 显著提升道路网络的空间连通性和几何精度

---

### 10. Mobile-Seed: Joint Semantic Segmentation and Boundary Detection for Mobile Robots

<div align="center">

| **属性** | **内容** |
|---------|---------|
| **期刊** | IEEE Robotics and Automation Letters (RA-L) |
| **年份** | 2024 |
| **单位** | 武汉大学，慕尼黑工业大学，南洋理工大学，伦敦国王学院，新加坡科技局，国防科技大学 |
| **核心任务** | 联合语义分割和边缘检测 |
| **论文链接** | [📄 IEEE: 10461032](https://ieeexplore.ieee.org/document/10461032) |
| **代码仓库** | [💻 GitHub: Mobile-Seed](https://github.com/WHU-USI3DV/Mobile-Seed) |
| **项目主页** | [🌐 Mobile-Seed Project](https://whu-usi3dv.github.io/Mobile-Seed/) |
| **一句话亮点** | 基于轻量化框架同时执行语义分割和边缘检测任务，实时获取鲁棒语义信息和锐利边界信息 |

</div>

#### 🔬 主要创新点

- **🤖 Mobile-Seed轻量化框架**: 首个针对移动机器人设计的轻量化多任务学习框架，同步完成语义分割和边缘检测，为机器人抓取操作、实时语义建图和边缘计算传感器校准提供核心支撑

- **🔀 双分支编码器设计**: 创新的编码器架构包含两个专门分支：
  - **语义分支**: 捕获类别感知的语义信息，专注于像素级分类
  - **边界分支**: 从多尺度语义特征中提取边界信息，专注于目标轮廓检测

- **⚡ 主动融合解码器(AFD)**: 自适应学习语义特征和边界特征各个通道的权重关系，实现动态融合而非固定权重融合；通过通道注意力机制为每个特征通道分配合适的权重，显著提升特征融合效果

- **🎯 多任务一致性约束**: 引入双任务正则化损失缓解深度多样性监督(DDS)引起的任务冲突，使语义分割和边缘检测任务相互促进而非相互干扰

- **📊 优异的性能表现**: 在多个基准数据集上实现显著提升：
  - **Cityscapes**: mIoU相比SOTA基线提升2.2%，mF-score提升4.2%
  - **实时性能**: 在RTX 2080 Ti GPU上以1024×2048高分辨率输入保持23.9 FPS
  - **泛化能力**: 在CamVid和PASCAL Context数据集上验证了广泛的应用前景

- **🚀 机器人应用优化**: 专门针对移动机器人的计算资源限制和实时性要求进行优化，在边缘计算单元上实现高效推理，为自主导航和环境感知提供准确且快速的视觉理解

---

<div align="center">

**🌟 持续更新中，敬请关注！**

</div>
