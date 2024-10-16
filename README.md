<div align="center">

# PDF-WuKong <img src="assets/logo.png" width="50"/> : A Large Multimodal Model for Efficient Long PDF Reading with End-to-End Sparse Sampling

[\[📜 Paper\]](https://arxiv.org/abs/2410.05970) [\[🚀 Code\]](https://github.com/yh-hust/PDF-Wukong) [\[🤗 HF Dataset\]](https://huggingface.co/datasets/yh0075/PaperPDF) [\[📖 Project Page\]](https://willpat1213.github.io/PDF-Wukong/)

</div>

<h2></h2>


<h5 align="center"> Please give us a star ⭐ for the latest update.  </h5>

<h5 align="center"> </h5>

<h5 align="center"> </h5>

 
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

</details>

## News
* ```2024.10.10``` 🚀 We release the paper [PDF-Wukong](https://arxiv.org/abs/2410.05970).

## Methodology
### The overall structure of PDF-WuKong
<p align="center">
    <img src="assets/overall structure of PDF-WuKong.png" width="1000"/>
</p>

### The construction process of PaperPDF
<p align="center">
    <img src="assets/dataset construction.png" width="1000"/>
</p>

## Dataset
### The statistic of PaperPDF.
Text-only and Image-only indicate that the QA pairs are generated based on either a single text paragraph or an image extracted from the PDF. Meanwhile, Image-text, Section, and Cross-paragraph denote that the QA pairs are generated from a paragraph and its corresponding references, an entire section, or non-contiguous paragraphs, respectively.
<p align="center">
    <img src="assets/The statistic of PaperPDF.png" width="500"/>
</p>

**PaperPDF** is publicly available on Hugging Face Datasets: [PaperPDF](https://huggingface.co/datasets/yh0075/PaperPDF).

### Repository Structure
The structure of this repository is shown as follows.
```
PaperPDF
│
├── Original PDFs               # Original PDF documents
│
├── Parsed Data
│   ├── PaperPDF.py              # Code for extracting text and image information from XML documents
│   ├── pdf_xml                  # XML files generated by Grobid from the PDF documents   
│   └── pdf_figure              
│       ├── figure               # Extracted images from the PDF documents
│       └── data                 # Metadate of the images
│
├── Train  
│   ├── train_100w.jsonl         # The complete 1 million training data 
│   ├── train_50w.jsonl          # 500,000 training data for ablation studies
│   └── train_10w.jsonl          # 100,000 training data for ablation studies
│ 
└── Test
    └── test.jsonl               # The test set
      
```

### Data Instances
For each instance in the dataset, the following fields are provided:
```
json
{
  {
  "PDF name": "1507.04291v1",
  "Category": "single-text_img",
  "Query": "According to Table 1, which sections discuss TCB-included Chebyshev kernels for both position and velocity?",
  "Answer": ["Sections 5.3.3 and 5.3.4 discuss TCB-included Chebyshev kernels for both position and velocity.", "Sections 5.3.3."],
  "Evidence": {
    "Texts": [{"idx": 11, "Text": "The six SPK data types, listed in Table 1, for ephemerides of natural solar system bodies..."}],
    "Figures": [{"idx": 220, "Caption": "Table 1: Double precision kernel data types of interest.", "Figure": "1507.04291v1-Table1-1.png"}]
    }
  }
  ...
}

```
### Data Fields
- `PDF name`: a string containing the name of the PDF document.
- `Category`: a string representing the category of the query, which can be one of the following: `single-text_only`, `single-image_only`, `multi-text_image`, `multi-section`, `multi-cross_paragraph`.
- `Query`: a string containing the question posed to the PDF
- `Answer`: an array of the two answers generated, the training set and test set has different prompt for the answers (see [title](### Dataset Creation) below for more details)
- `Evidence`: an object containing supporting texts and figures (if provided) from the PDF document


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
Please refer to our paper for more details.

## Training/evaluation code, checkpoint, demo will be released soon.

## Citing PDF-Wukong
If you wish to refer to the baseline results published here, please use the following BibTeX entries:

```BibTeX
@article{xie2024pdfwukong,
        title={PDF-WuKong: A Large Multimodal Model for Efficient Long PDF Reading with End-to-End Sparse Sampling}, 
        author={Xie, Xudong and Yin, Liang and Yan, Hao and Liu, Yang and Ding, Jing and Liao, Minghui and Liu, Yuliang and Chen, Wei and Bai, Xiang},
        year={2024},
        journal={arXiv preprint arXiv:2410.05970},
        url={https://arxiv.org/abs/2410.05970},
      }
```
## Copyright
<!-- If you wish to refer to the baseline results published here, please use the following BibTeX entries: -->

PDF-Wukong project is intended for non-commercial use only. For commercial inquiries, please contact haoyan at haoyan@hust.edu.cn. 
