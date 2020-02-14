# Very Deep Convolutional Networks For Large-Scale Image Recognition(VGG)

논문 링크 : https://arxiv.org/pdf/1409.1556.pdf

## 논문 요약

> 1. ILSVRC 2014 대회에서 GoogleNet에 근소한 차이로 아쉽게 2등을 차지한 Network
> 2. VGG Net 논문은 망의 깊이가 딥러닝 결과에 어떤 영향을 미치는 지 알아보기 위하여 연구되었다
> 3. 3x3 filter size를 사용했다
> 4. VGGnet, GoogleNet 이전의 depth는 8layers 수준에서 머물렀다면 GoogleNet, VGGnet 이후 크게 깊어졌다.
> 5. 깊은 네트워크를 가지고 있지만, GoogLeNet과 비교하면, 구조가 매우 간단하다
> 6. 매우 많은 파라미터를 이용하여 연산한다는 단점이 있다.

## 특징
> 망의 깊이가 딥러닝 결과에 어떤 영향을 미치는 지 알아보기 위해 연구되었기 때문에 기존에 사용하던 것보다 작은 3x3 filter size를 사용햐여, 6개의 깊이가 다른 (layer depth ) Network를 구성하여 실험. 의도했던건지 아닌지는 모르겠지만, conv filters에 3x3 filter size를 스택구조로 쌓아 여러개 사용하면서 5x5 혹은 7x7 filter size를 사용하는 것과 비슷한 효과를 내면서도 파라미터 수는 조금 더 줄여 좋은 결과를 얻어냈다.

## 실험 내용
~~개 고양이 이미지를 분류하는 코드. vgg 모델을 사용하여 훈련
~~각각 2000장의 데이터와 20000장의 데이터를 훈련
~~훈련 데이터의 양이 정확도에 어떤 영향을 끼치는 지 알아보려 함
    
_load 파일은 vgg 모델을 불러와 사용

_made 파일은 vgg 모델을 구현 및 특징맵 출력
