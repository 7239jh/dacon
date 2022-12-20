# 쇼핑몰리뷰평점분류  
1. 참여인원: 개인
2. 참여기간: 3일
3. 성적: 7등
4. 코드공유: https://dacon.io/codeshare/5988  
  
# 목적
1,2,4,5점으로 분류 되어 있는 쇼핑몰 리뷰를 학습하여 정확도 높은 4분류 모델 만들기  
  
# 데이터셋  
1.train set: id, reviews, target 열로 이루어진 한글 텍스트 데이터셋 3만개  
2.test set: id, reviews열로 이루어진 한글 텍스트 데이터셋 3만개

# 전처리  
1. emoji를 활용한 불용어제거
2. train_set, valid_set을 8:2로 나눈 후 train_set에만 koEDA를 활용한 데이터 증강  

# 학습
1. "KcELECTRA", "roberta", "kobert" 및 하이퍼파라미터를 변화하여 5가지 방식으로 학습하여 모델 저장  
2. 각 5가지 모델의 soft_voting을 통한 최종 예측값 출력

