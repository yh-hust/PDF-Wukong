# PDF-Wukong
A Large Multimodal Model for Efficient Long PDF Reading with End-to-End Sparse Sampling
<h3 align="center"> <a href="https://arxiv.org/abs/2410.05970">PDF-WuKong: A Large Multimodal Model for Efficient Long PDF Reading with End-to-End Sparse Sampling</a></h3>
<h2></h2>

<h5 align="center"> Please give us a star ⭐ for the latest update.  </h5>

<h5 align="center">

<h5 align="center">

 
<!--[![arXiv](https://img.shields.io/badge/Arxiv-2311.06607-b31b1b.svg?logo=arXiv)](https://arxiv.org/abs/2311.06607) -->
<!--[![License](https://img.shields.io/badge/License-Apache%202.0-yellow)](https://github.com/Yuliang-Liu/Monkey/blob/main/LICENSE) -->
<!--[![GitHub issues](https://img.shields.io/github/issues/Yuliang-Liu/Monkey?color=critical&label=Issues)](https://github.com/Yuliang-Liu/Monkey/issues?q=is%3Aopen+is%3Aissue)-->
<!--[![GitHub closed issues](https://img.shields.io/github/issues-closed/Yuliang-Liu/Monkey?color=success&label=Issues)](https://github.com/Yuliang-Liu/Monkey/issues?q=is%3Aissue+is%3Aclosed)  --><br>
</h5>

>[ArXiv] [**PDF-Wukong: A Large Multimodal Model for Efficient Long PDF Reading with End-to-End Sparse Sampling**](https://arxiv.org/abs/2410.05970)<br>
> Xudong Xie*, Liang Yin*, Hao Yan*, Yang Liu*, Jing Ding, Minghui Liao, Yuliang Liu, Wei Chen，Xiang Bai <br>

<details open><summary>💡 Monkey series projects:✨. </summary><p>
<!--  may -->

>[CVPR'24] [**Monkey: Image Resolution and Text Label Are Important Things for Large Multi-modal Models**](https://arxiv.org/abs/2311.06607)<br>
> Zhang Li, Biao Yang, Qiang Liu, Zhiyin Ma, Shuo Zhang, Jingxu Yang, Yabo Sun, Yuliang Liu, Xiang Bai <br>
[![arXiv](https://img.shields.io/badge/Arxiv-2311.06607-b31b1b.svg?logo=arXiv)](https://arxiv.org/abs/2311.06607)
[![Source_code](https://img.shields.io/badge/Code-Available-white)](https://github.com/Yuliang-Liu/Monkey)
[![Demo](https://img.shields.io/badge/Demo-blue)](http://vlrlab-monkey.xyz:7681/)
[![Detailed Caption](https://img.shields.io/badge/Detailed_Caption-yellow)](http://huggingface.co/datasets/echo840/Detailed_Caption)
[![Model Weight](https://img.shields.io/badge/Model_Weight-gray)](http://huggingface.co/echo840/Monkey)
[![Model Weight in Wisemodel](https://img.shields.io/badge/Model_Weight_in_Wisemodel-gray)](https://www.wisemodel.cn/models/HUST-VLRLab/Monkey/)
[![Demo in Wisemodel](https://img.shields.io/badge/Demo_in_Wisemodel-blue)](https://wisemodel.cn/space/gradio/huakeMonkey)



> [**TextMonkey: An OCR-Free Large Multimodal Model for Understanding Document**](https://arxiv.org/abs/2403.04473)<br>
> Yuliang Liu, Biao Yang, Qiang Liu, Zhang Li, Zhiyin Ma, Shuo Zhang, Xiang Bai <br>
[![arXiv](https://img.shields.io/badge/Arxiv-2403.04473-b31b1b.svg?logo=arXiv)](https://arxiv.org/abs/2403.04473) 
[![Source_code](https://img.shields.io/badge/Code-Available-white)](https://github.com/Yuliang-Liu/Monkey/blob/main/monkey_model/text_monkey/README.md)
[![Data](https://img.shields.io/badge/Data-yellow)](https://huggingface.co/datasets/MelosY/TextMonkey_Data/tree/main)
[![Model Weight](https://img.shields.io/badge/Model_Weight-gray)](https://www.modelscope.cn/models/lvskiller/TextMonkey)

> [**Mini-Monkey: Multi-Scale Adaptive Cropping for Multimodal Large Language Models**](https://arxiv.org/pdf/2408.02034)<br>
> Mingxin Huang, Yuliang Liu, Dingkang Liang, Lianwen Jin, Xiang Bai <br>
[![arXiv](https://img.shields.io/badge/Arxiv-2408.02034-b31b1b.svg?logo=arXiv)](https://arxiv.org/abs/2408.02034)
[![Source_code](https://img.shields.io/badge/Code-Available-white)](https://github.com/Yuliang-Liu/Monkey/tree/main/project/mini_monkey)
[![Demo](https://img.shields.io/badge/Demo-blue)](http://vlrlab-monkey.xyz:7685)
[![Model Weight](https://img.shields.io/badge/Model_Weight-gray)](https://huggingface.co/mx262/MiniMokney)
[![Model Weight in Wisemodel](https://img.shields.io/badge/Model_Weight_in_Wisemodel-gray)](https://www.wisemodel.cn/models/HUST-VLRLab/Mini-Monkey)

## News
* ```2024.10.10``` 🚀 We release the paper [PDF-Wukong](https://arxiv.org/abs/2410.05970).

## Methodology
### The overall structure of PDF-WuKong.
<p align="center">
    <img src="assets/overall structure of PDF-WuKong.png" width="1000"/>
</p>

### Compared with closed-source APIs and previous SOTAs on Video and Structural High-resolution images.
<p align="center">
    <img src="assets/dataset construction.png" width="1000"/>
</p>

In Progress...

## Dataset
### The statistic of PaperPDF.
Text-only and Image-only indicate that the QA pairs are generated based on either a single text paragraph or an image extracted from the PDF. Meanwhile, Image-text, Section, and Cross-paragraph denote that the QA pairs are generated from a paragraph and its corresponding references, an entire section, or non-contiguous paragraphs, respectively.
<p align="center">
    <img src="assets/The statistic of PaperPDF.png" width="500"/>
</p>
In Progress...

## Evaluate
### Performance comparison with other commercial products on PaperPDF.
<p align="center">
    <img src="assets/comparision on PaperPDF.png" width="500"/>
</p>

### Performance comparison with other DocVLMs on single-page document understanding.
<p align="center">
    <img src="assets/single page evaluation.png" width="500"/>
</p>

### Performance comparison with other DocVLMs on multi-page document understanding.
<p align="center">
    <img src="assets/MP evaluation.png" width="500"/>
</p>
Please refer to Technical Report for more details.

## Environment
In Progress...

## Train
In Progress...

## Inference
In Progress...

## Checkpoint
will be released soon

## Demo
In Progress...

## Citing PDF-Wukong
## Copyright
<!-- If you wish to refer to the baseline results published here, please use the following BibTeX entries: -->
In Progress...

PDF-Wukong project is intended for non-commercial use only. For commercial inquiries, please contact haoyan at haoyan@hust.edu.cn. 
