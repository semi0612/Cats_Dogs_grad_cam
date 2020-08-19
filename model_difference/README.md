## Cats_vs_Dogs

### 실험 내용
개고양이 이미지를 분류하는 코드
모델을 불러와 사용하는 것과 만들었을 때의 성능 차이가 크게 나타나는지 알아보기 위하여.

### 실험 환경
- 이 실험은 Tensorfloww Library API을 기반으로 Colab이 제공하는 GPU를 사용하였습니다. 
- 데이터는 kaggle에서 제공하는 Cats-vs-Dogs 데이터를 이용 : 2천 5백장 중 2000장을 train_data, 500장을 valid_data 으로 나누어 진행

### 실험 모델
VggNet(Layer 16, epoch 15, optimizer RMSprop(tf.keras.optimizers.RMSprop(lr=1e-4), batch_size 20

> 모델을 load해 사용한 결과

<img_s>![cat_dog_2000_load](https://user-images.githubusercontent.com/51469989/90616740-c3e04900-e248-11ea-840e-dcb4ecba5c71.JPG)



> 모델을 만들어 사용한 결과

![cat_dog_2000_made](https://user-images.githubusercontent.com/51469989/90616796-db1f3680-e248-11ea-93d0-67033d328921.JPG)

