# 📁Diet Helper Project

**1. 주제**

사용자의 다이어트 식단에 도움을 주고자 사용자가 섭취할 식단(일반식/샐러드)을 \
사진으로 찍어 입력하면 해당 식단의 칼로리를 제공하는 것이 목표이다.


**2. 데이터 셋**

Roblflow
- 'food korea6' (1862장)
- 'korean food_yolo5' (991장)
- 'salad' (1352장)
- 'vegetable' (2884장)

AIHub
- '한국 음식 이미지' (15만장)
- '건강관리를 위한 음식 이미지' 중 샐러드 데이터만 사용 (300만장 중 95,730장)

Kaggle
- 'Calories in Food Items (per 100 grams)' (csv/xlsx 파일)


**3. 사용 학습 모델**

YOLOV5
- https://github.com/ultralytics/yolov5.git


**4. 제약 조건**

여러가지 재료가 혼합된 음식의 경우 총합 칼로리는 구할 수 있으나 각 재료의 칼로리는 얻기가 힘들다.


**5. 개선 방안**

- 채소, 과일을 각각 학습시키는 것이 아니라 여러 종류의 샐러드를 학습시켜\
  평균 칼로리를 도출하여 오차를 줄인다.
- 사용자가 섭취하는 식단이 사용자의 건강 상태와 적합한지 판별하고\
  적합하지 않을 시 경고 문구를 출력한다.
