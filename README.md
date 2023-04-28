# 자율주행을 위한 객체 인식(YOLOv5)
## 프로젝트 개요
- 주어진 이미지에서 신호등과 도로 표지판을 인식하는 모델을 구축
- [학습 데이터셋 (출처: ai hub)](https://drive.google.com/file/d/1iz4CQz1P6_xJBRYqJuovjFTiEQfb0XQ0/view?usp=sharing)
## 프로젝트 배경
- 자율 주행 차량이 상황에 따라 적절하게 주행하기 위해서 여러가지 객체 인식이 요구되는데 본 프로젝트에서는 그 중 신호등과 도로 표지판을 인식해내는 모델을 구축
## 프로젝트 수행과정 
![image](https://user-images.githubusercontent.com/114974542/235167176-ffc4787a-b078-4681-86f9-be5a132721d8.png)
![image](https://user-images.githubusercontent.com/114974542/235168529-9b51b11d-d0f7-4189-b842-3e7a7a1b0424.png)
![image](https://user-images.githubusercontent.com/114974542/235167562-d574d50f-6041-4df3-aabe-4bf95d225cdc.png)
![image](https://user-images.githubusercontent.com/114974542/235167685-9578be25-ed0d-4fed-b6de-5cb3d5ae0781.png)
## 한계점 및 추후 발전과제
- 많은 양의 데이터와 높은 화질의 이미지 데이터를 수집했음에도 학습시간이 길고 메모리 문제로 모델 학습에 생각보다 시간이 많이 소요되었다.
- 이로 인해 epoch 수를 충분하게 설정하지 못하여, 모델 학습이 충분히 이루어지지 않았다.
- 또한 YOLO 모델 외 다른 객체 감지 모델을 적용해보지 못한 아쉬움이 있다.
- 사진 상 신호등과 교통 표지판은 상대적으로 작은 크기이기 때문에, 작은 크기를 잘 감지하지 못하는 1 stage detector 보다 2 stage detector를 적용했을 때 성능이 더 높아질 수도 있다.
- 본 프로젝트에서는 신호등과 교통 표지판을 감지하고 둘을 분류하는 데에 마쳤지만, 실제 자율주행 기술에서는 신호등의 상태(초록불, 빨간불)와 표지판 의미를 인식할 수 있어야 하므로,
- 이러한 세부적인 상태도 분류할 수 있는 모델이 구현된다면 더 유용할 것이라 생각된다.
