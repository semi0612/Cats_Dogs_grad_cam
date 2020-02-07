# Very Deep Convolutional Networks For Large-Scale Image Recognition(VGG)

논문 링크 : https://arxiv.org/pdf/1409.1556.pdf

## 논문 요약

VGG Net 이라고 불리는 심층 신경망 모델은 Oxford University에서 개발되었으며, 2014년 ILSVRC에서 GoogleNet에 근소한 차이로 아쉽게 2등한 network이다. 하지만 굉장히 간단한 구조로 이루어져 있음에도 높은 성능을 내며, 구조변형이 쉬워 많이 사용되었다.

VGG Net 논문은 망의 깊이가 딥러닝 결과에 어떤 영향을 미치는 지 알아보기 위해서 연구되었다. 기존에 사용되던 것보다 작은 3x3 filter size 를 사용하여 6개의 다른 깊이의 network를 구성하여 실험, layer depth는 최대 19의 깊이로 만들었다. conv필터에 3x3 filter size를 stack 구조로 쌓아 사용하게 되면 receptive filed를 늘릴 수 있으며, 여러개 사용하면 5x5 혹은 7x7 filter size를 사용하는 것과 비슷한 효과를 낼 수 있으면서도 파라미터 수는 조금 더 줄일 수 있기 때문에 가장 작은 사이즈의 filter를 사용했다. 논문 내 표 3, 4내용을 보면 multiple test scale의 에러율이 single test scale의 에러율보다 낮게 나온것을 보면 한눈에 확인이 가능하다. dense보다는 multi-crop을 사용하는 것이 조금 더 좋지만, multi-crop과 dense를 함께 사용하는 것이 가장 에러율이 낮음을 보여준다(표 5)

하지만 파라미터의 개수가 너무 많다. 2014년 경쟁했던 GoogLeNet의 파라미터 개수가 5 millions 수준이였던 것에 비하여 VGG는 가장 단순간 구조에서조차 133 millions 인것으로 확인이 가능.

***

개 고양이 이미지를 분류하는 코드. vgg 모델을 사용하여 훈련
각각 2000장의 데이터와 20000장의 데이터를 훈련
훈련 데이터의 양이 정확도에 어떤 영향을 끼치는 지 알아보려 함
    
_load 파일은 vgg 모델을 불러와 사용했으며
_made 파일은 vgg 모델을 구현해 보고자 노력함
