2021 Uni DataThon에 참가한 기록입니다.
주제는 음식사진을 분류하는 것이었습니다.

비록 좋은 성적을 거두지는 못했지만,
비전 ai에 대한 좋은 경험을 할 수 있었습니다.

제가 속한 팀의 시도를 요약하자면

1. data preprocess
  => 컴퓨팅 파워가 부족한 환경탓에 최대한 작은 데이터로 전처리 (64*64*1, grayscale)
 
2. 대분류기, 소분류기
  => 음식의 가짓수가 총 150가지로 매우 많아서 먼저 대분류로 음식을 분류한 뒤 소분류하자는 아이디어
  => 대분류 classifier 하나와, 각 소분류 classifier 27개를 훈련
  => 시간 부족 및 대분류 classifier의 낮은 성능으로 중단
  
3. 앙상블 모델 선택
  => resnet 150과 swin transformer를 선택
  => 컴퓨팅 문제 및 훈련 시간 부족으로 인해 resnet 18과 basic cnn 두 모델을 훈련
  
(후기)
이미지 데이터를 다운받고 공유하는 것에 시간을 너무 소모함. 더 체계적인 데이터 관리법이 필요
이미지 전처리에 대한 추가 지식이 필요
대회 전 충분한 성능의 개인 서버 또는 개인 컴퓨터 확보가 필요

(추가코드 / 데이터)
https://colab.research.google.com/drive/11YjARm4DkwAt5DfUaTeRkqVZZzUqfqKL?usp=sharing, https://drive.google.com/file/d/1Jpu5khn9RG0NG-xaTMTjlzfaGi6UMYBE/view?usp=sharing, https://drive.google.com/drive/folders/1Jq3LbxO4EXmEupNF1QKanluYKxfGRZY5?usp=sharing, https://drive.google.com/drive/folders/1cmlf97jNMl0BSF4d81z3xE-xgfmy6DXe?usp=sharing, https://colab.research.google.com/drive/1fLcHtdeNreI6Ur33rEw6foiqHhGuZeg_?usp=sharing
