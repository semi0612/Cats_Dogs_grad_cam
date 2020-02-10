# Very Deep Convolutional Networks For Large-Scale Image Recognition(VGG)

논문 링크 : https://arxiv.org/pdf/1409.1556.pdf

## 논문 요약

> 1. ILSVRC 2014 대회에서 GoogleNet에 근소한 차이로 아쉽게 2등을 차지한 Network
> 2. VGG Net 논문은 망의 깊이가 딥러닝 결과에 어떤 영향을 미치는 지 알아보기 위하여 연구되었다
> 3. 3x3 filter size를 사용했다
> 4. VGGnet, GoogleNet 이전의 depth는 8layers 수준에서 머물렀다면 GoogleNet, VGGnet 이후 크게 깊어졌다.
> 5. 깊은 네트워크를 가지고 있지만, GoogLeNet과 비교하면, 구조가 매우 간단하다
> 6. 매우 많은 파라미터를 이용하여 연산한다는 단점이 있다.

***

## 실험 내용
개 고양이 이미지를 분류하는 코드. vgg 모델을 사용하여 훈련
각각 2000장의 데이터와 20000장의 데이터를 훈련
훈련 데이터의 양이 정확도에 어떤 영향을 끼치는 지 알아보려 했다
    
_load 파일은 vgg 모델을 불러와 사용

_made 파일은 vgg 모델을 구현
