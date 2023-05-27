# svcm
ResNet34 모델을 기반으로 지하철 차량의 형상으로 차종 구분하는 모델 학습  
SVCM은 'Subway Vehicle Classification Model'의 약자입니다.

## 구성
| 파일 또는 폴더 이름                             | 설명                       |
|------------------------------------------------|---------------------------|
| [app](./app)                                   | 샘플 안드로이드 앱 소스코드 |
| [datasets](./datasets)                         | 지하철 차량 이미지 데이터셋 |
| [models](./models)                             | 학습된 모델                |
| [classification.ipynb](./classification.ipynb) | ResNet 기반 학습 코드      |

## 요구사항
학습을 하기 위해선 아래의 요구사항이 필요합니다.
1. Anaconda  
Jupyter Notebook을 통해 [classification.ipynb](./classification.ipynb)을 실행하려면 Anaconda가 필요합니다.
2. GPU  
필수는 아니지만 빠른 학습을 위해 CUDA를 지원하는 GPU가 필요합니다.
3. PyTorch  
PyTorch 2.0.0 이상의 패키지를 권장합니다.  
torchvision 패키지의 버전이 0.15.0 이상이어야 올바르게 작동하므로 아래의 명령어를 통해 최신 PyTorch를 설치합니다.
```console
conda install pytorch torchvision torchaudio pytorch-cuda=11.7 -c pytorch -c nvidia
```
CUDA 버전이 다르거나 CPU로 학습을 할 경우에는 PyTorch 설치 명령이 달라질 수 있습니다.

또한 안드로이드 앱 빌드를 위해 [Android Studio](https://developer.android.com/studio)가 필요합니다.

## demo
https://github.com/wise1ight/svcm/assets/59006393/caac1afc-d213-4dcd-bc03-dd12b474daa5

https://github.com/wise1ight/svcm/assets/59006393/b576b632-ac52-4a9c-a0d2-40f4f3e98b53

## 참고자료
[Tensorflow를 이용한 애완동물 영상 세부 분류](https://koreascience.kr/article/CFKO202023758834506.pdf)  
[Oxford-IIIT Pets-Pytorch](https://github.com/Skuldur/Oxford-IIIT-Pets-Pytorch)  
[PyTorch for Android - Image Classification App](https://www.youtube.com/watch?v=ghxLlsT7ebo)
