# 生物信息学Project1

---

## 第一堂课笔记
- 本节课了解了什么是生物信息学，明白了生信的重要性，从question-information-analysis-modeling四个step逐步认识生信。
  > 世上有三大哲学问题：什么是生命？什么是意识？宇宙是如何运转的？——信息的观点涵盖了以上三者

  这句话震撼了我，第一次感受到信息的浩渺、宽阔、包容，给我以新的启迪。
  
  同时 “*RNG:Robot Nanotech Genetics*” 也让我意识到基因信息的地位，而数量庞大的信息需要整理分析应用，这进一步说明了学习生信的必要性。
  
- 此外，在课上学习了github的应用、Markdown语言的编辑、云存储与备份等内容，为之后的进修奠定基础。

### 算法与模型的区别
| **特征**        | **算法 (Algorithm)**                              | **模型 (Model)**                                  |
|----------------|--------------------------------------------------|--------------------------------------------------|
| **定义**        | 解决问题的具体步骤或计算流程（如排序、搜索）。            | 对数据或现象的数学/统计抽象（如线性回归、神经网络）。     |
| **作用**        | 实现特定功能（如数据清洗、特征提取）。                  | 描述数据关系或预测结果（如基因表达预测）。              |
| **输入/输出**   | 输入数据 → 处理后输出结果（如排序后的序列）。             | 输入数据 → 输出概率分布或预测标签（如疾病分类）。        |
| **示例**        | 动态规划（序列比对）、K-means（聚类）。                 | 逻辑回归（分类）、隐马尔可夫模型（基因识别）。           |
| **依赖关系**    | 可独立实现功能（如排序算法）。                          | 通常依赖算法训练参数（如梯度下降优化模型权重）。          |
    
*算法是"怎么做"（如反向传播），模型是"用什么框架"（如神经网络层数设计）*

### 课堂案例解析
- **NGS数据分析流程**：
  - 算法：DEGseq2（差异表达分析）、TOPHAT（比对）。
  - 模型：概率模型（如RNA编辑检测中的GIREMI）。
- **建模预测**：
  - 统计模型：逻辑回归（预测基因致病性）
  - 机器学习：神经网络（蛋白质结构预测）

### NGS数据分析
- 测序+生信工具     
  分析数据+可视化展示
![图片1](https://github.com/user-attachments/assets/1f4ca33c-001b-4d34-991f-ecb39ef14731)

- **三代测序对比**：  

  | **特征**        | 第一代               | 第二代（NGS）       | 第三代            |
  |----------------|---------------------|--------------------|-------------------|
  | **代表技术**    | Sanger测序法         | Illumina           | PacBio/Nanopore   |
  | **读长**        | 长（~1000 bp）       | 短（50-300 bp）     | 超长（>10,000 bp） |
  | **通量**        | 低（单次运行1-96样本） | 高（百万级reads）    | 中等（千级reads）  |
  | **准确率**      | 高（>99.99%）        | 高（>99.9%）        | 中等（85-97%）    |
  | **典型应用**    | 小片段验证、克隆测序    | 全基因组测序、RNA-seq | 结构变异、全长转录本 |


    
---

## 本学期学习计划

### 1. 基础技能强化
- **工具掌握**：
  - GitHub：每周提交代码至个人仓库，用`README.md`记录进展。
  - Markdown：用Typora撰写实验报告。
  - Linux/Docker：完成PPT第11页的Docker实战练习（如运行Ubuntu容器）。
- **编程语言**：
  - Python/R语言：每周完成2个生信脚本（如序列处理、统计绘图）。
  - Bash脚本：整理常用命令。

### 2. 核心内容学习
- **理论重点**：
  - NGS数据分析：复现PPT第16页的RNA-seq流程（使用`HISAT2 + DESeq2`）。
  - 机器学习应用：实现PPT第21页的神经网络模型（如用Keras预测蛋白质结构）。
- **实践项目**：
  - Meta基因组分析：使用QIIME2处理环境样本数据（参考PPT第13页）。
  - 个人基因组解读：利用GATK分析自己的WES数据（模拟流程）。

