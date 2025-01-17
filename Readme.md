![header](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=1&height=250&section=header&text=어떤%20이모지를%20갖고%20싶어?%20Text-to-Emoji!&fontSize=40)

<img src="https://img.shields.io/badge/python-3776AB?style=flat&logo=python&logoColor=white"/> <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat&logo=PyTorch&logoColor=white"/>    
<img src="https://img.shields.io/badge/streamlit-FF4B4B?style=flat&logo=streamlit&logoColor=white"/> <img src="https://img.shields.io/badge/FastAPI-009688?style=flat&logo=FastAPI&logoColor=white"/> <img src="https://img.shields.io/badge/BentoML-E9568E?style=flat&logo=BentoML&logoColor=white"/> <img src="https://img.shields.io/badge/HAProxy-02458D?style=flat&logo=HAProxy&logoColor=white"/>


## Service URL

[Service Link](https://text-to-emoji.streamlit.app/)

## 시연 영상

<img src="https://user-images.githubusercontent.com/43758562/218053996-35bd2ae8-200d-4348-be7f-c8541db73cfa.gif" width="80%" height="80%"/>

<br>

## Introduction

### Background

- **Unicode**에 따르면, 전 세계 인구의 92%가 이모지를 사용합니다. ([링크](https://pumble.com/learn/communication/emoji-statistics-internal-communication/))
- **2018년 기준**, **페이스북**에서 하루에 쓰이는 이모지의 갯수는 **50억개**에 달합니다. ([링크](https://blog.emojipedia.org/5-billion-emojis-sent-daily-on-messenger/))
- **다섯개 중 하나** 이상의 **트윗**이 이모지를 포함하고 있고, 이 비율은 **점점 높아지고 있습니다.** ([링크](https://blog.emojipedia.org/top-emoji-trends-of-2021/))
- **인스타그램** **댓글**의 **50%이상**이 이모지를 포함하고 있습니다.
- 이 외에도 수많은 기사와 리서치가 이모지가 가진 영향력을 보여주고 있습니다.

### 하지만, 단 3633개만 존재하는 표준 emoji

Unicode상에 등재된 emoji는 3633개입니다.

- 다양성과 개인화가 점점 더 중요해짐에 따라, 기존**🧑** yellow skin tone 뿐이던 emoji에도 **🧑🏿🧑🏾🧑🏽🧑🏼🧑🏻** 다양한 skin tone의 추가나, 👨‍❤️‍👨 나 ⚧️와 같은 다양성과 관련 된 emoji의 추가로 이런 변화에 맞추어가는 모습을 보였습니다.
- 그럼에도 불구하고 표준 emoji는 원하는 것을 전부 표현할 수 없으며, 추가도 거의 한계에 도달한 모습을 보여주고 있습니다.
- 따라서 저희 팀은 생성 모델을 통하여 개인이 직접 emoji를 만들어 이용할 수 있게 하는 프로젝트를 고안하게 되었습니다.

### Emoji Samples

<img src="https://user-images.githubusercontent.com/43758562/217686443-6c25df44-ea48-44d9-b30a-7224c1390748.png" width="70%" height="70%"/>

<br>

## Dataset

### Openmoji

- **Openmoji**는 **CC BY-SA 4.0** 라이센스 하에 자유롭게 사용할 수 있는 **오픈 소스** 이모지 플랫폼 입니다.
- Unicode에 등재된 **3633**개의 이모지를 포함하여 총 **4083**개의 이모지를 제공합니다.
- 해당 플랫폼에서 제공하는 데이터를 활용하여 이미지-텍스트 쌍을 만들어 허깅페이스 허브에 배포하여 사용하였습니다.
- HuggingFace 에 [Openmoji dataset](https://openmoji.org/)을 업로드하였습니다.([링크](https://huggingface.co/datasets/soypablo/Emoji_Dataset-Openmoji))

### noto-emoji

- **Noto emoji**는 구글이 제작한 **Open Font License 1.1** 하에 자유롭게 사용할 수 있는 **오픈소스 이모지 라이브러리** 입니다.
- Unicode에 등재된 3,633개의 이모지 png파일을 제공합니다.
- 해당 플랫폼에서 제공하는 데이터를 활용하여 이미지-텍스트 쌍을 만들어 허깅페이스 허브에 배포하여 사용하였습니다.
- HuggingFace 에 [noto-emoji dataset](https://github.com/googlefonts/noto-emoji)을 업로드하였습니다.([링크](https://huggingface.co/datasets/kuotient/noto-emoji-dataset))

## FlowChart

### Model FlowChart

<img src="https://user-images.githubusercontent.com/43758562/217688705-3740b46c-dfe9-4b38-ae76-daf0e9237474.png" width="70%" height="70%"/>

### Server FlowChart

<img src="https://user-images.githubusercontent.com/43758562/217688927-0febeae5-61b8-4014-be4a-0d7aaa3a2a1b.png" width="49%" height="49%"/> <img src="https://user-images.githubusercontent.com/43758562/217688936-e44c35de-574f-4880-8be1-15b1412bf396.png" width="49%" height="49%"/>

<br>

## Team

<img src="https://user-images.githubusercontent.com/43758562/217689917-80c307d7-512b-451f-a0ac-4992cb234dff.png" width="70%" height="70%"/>

- **서로 다른 조**에서 **multimodal**에 관심 있는 **우리**들이 모여서, **(FUSION)**
- 각자 아는 지식들을 **공유하고 융합**하여, **(FUSION)**
- **diffusion**을 활용해 **text-to-emoji** 문제를 풀어보자! **(FUSION)**

**We, Fusion!!**

|                     김지수                     |                 김현수                 |                지상수                 |                 최석훈                 |                   최혜원                   |
| :--------------------------------------------: | :------------------------------------: | :-----------------------------------: | :------------------------------------: | :----------------------------------------: |
|                    Modeling                    |                Modeling                |               Modeling                |                Modeling                |                  Modeling                  |
|                 Serving(HAProxy)                  |       Metric 및 이론, 논문 조사        |           Front(Streamlit)            |            Serving(BENTOML)            |         Multi Encoder(AltCLIP-m9)          |
|              데이터 제작 및 가공               |         프로젝트 기획 및 발표          |              Code Review              |          데이터 제작 및 가공           |           프로젝트 기획 및 발표            |
| [GitHub](https://github.com/kuotient/kuotient) | [GitHub](https://github.com/gustn9609) | [GitHub](https://github.com/ggb04110) | [GitHub](https://github.com/soypabloo) | [GitHub](https://github.com/soohi0/soohi0) |

## Project Directories
```
Relation_Extraction
 ┣ bentoml
 ┃ ┣ eng_serve
 ┃ ┃ ┣ bentofile_eng_model.yaml
 ┃ ┃ ┣ configuration.yaml
 ┃ ┃ ┣ requirements.txt
 ┃ ┃ ┗ service.py
 ┃ ┣ kor_serve
 ┃ ┃ ┣ bentofile_kor_model.yaml
 ┃ ┃ ┣ configuration.yaml
 ┃ ┃ ┣ requirements.txt
 ┃ ┃ ┗ service.py
 ┃ ┣ readme.md
 ┣ frontend
 ┃ ┣ frontend.py
 ┃ ┣ main.py
 ┃ ┗ utils.py
 ┣ train
 ┃ ┣ dataset_utils
 ┃ ┃ ┣ make_korean_datasets.py
 ┃ ┃ ┗ save_dataset.py
 ┃ ┣ dreambooth
 ┃ ┃ ┣ dreambooth-lora.py
 ┃ ┃ ┣ dreambooth-lora.sh
 ┃ ┃ ┣ dreambooth.py
 ┃ ┃ ┗ dreambooth.sh
 ┃ ┣ examples
 ┃ ┃ ┣ AltCLIP
 ┃ ┃ ┗ AltDiffusion
 ┃ ┣ inference
 ┃ ┃ ┣ inference-lora-fid.py
 ┃ ┃ ┣ inference-lora.py
 ┃ ┃ ┗ inference_lora_altdiffusion.py
 ┃ ┣ utils
 ┃ ┃ ┣ blacklist.py
 ┃ ┃ ┣ .
 ┃ ┃ ┣ .
 ┃ ┃ ┗ white_bg.py
 ┃ ┣ train_lora.py
 ┃ ┗ train_lora.sh
 ┣ .gitignore
 ┣ README.md
 ┗ requirements.txt
```

<br>

## More Information

### Document & Demo

| Type          | Link                                                                                           |
| ------------- | ---------------------------------------------------------------------------------------------- |
| WrapUp Report | [>> Notion](https://ebony-dime-3e7.notion.site/Text-to-Emoji-d248a750462447689fb6765335d829f8) |
| Presentation  | [>> Youtube](https://youtu.be/87ppOPYoRxY)                                                     |

<br>

## Reference

### Paper

- Denoising Diffusion Probabilistic Models [[PAPER]](https://arxiv.org/abs/2006.11239)
- AltCLIP: Altering the Language Encoder in CLIP for Extended Language Capabilities [[PAPER]](https://arxiv.org/pdf/2211.06679v2.pdf) [[CODE]](https://github.com/flagai-open/flagai)
- LoRA: Low-Rank Adaptation of Large Language Models [[PAPER]](https://arxiv.org/abs/2106.09685)
- BLIP: Bootstrapping Language-Image Pre-training for Unified
  Vision-Language Understanding and Generation [[PAPER]](https://arxiv.org/abs/2201.12086)

### Open Source

- huggingface/diffusers [[CODE]](https://github.com/huggingface/diffusers)
- AltCLIP [[CODE]](https://github.com/flagai-open/flagai)

![Footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=1&height=200&section=footer)
