# 🔥 Wildfire Smoke Detector

딥러닝을 이용한 산불 및 연기 탐지 모델입니다. Kaggle 및 AI Hub의 산불/연기 이미지 데이터를 학습시켜, 실제 CCTV 이미지나 단일 이미지에서도 연기 및 불꽃을 탐지할 수 있습니다.

## 📁 프로젝트 구성

- `train_model.ipynb`: 모델을 학습하는 Google Colab 노트북
- `test_single_image.ipynb`: 학습된 모델로 단일 이미지를 예측하는 노트북
- `fire_smoke_model.pth`: 학습된 모델 가중치 (ResNet18 기반)
- `fireandsmoke/`: 학습 및 테스트에 사용된 이미지 데이터셋
- `requirements.txt`: 필요한 라이브러리 목록
- `README.md`: 프로젝트 소개 문서

## 🧠 사용한 모델

- ResNet-18 (ImageNet 사전학습 모델 사용)
- Fine-tuning 후 최종 FC layer만 교체하여 클래스 수(예: fire, smoke, non_fire 또는 ['Smoke', 'fire'])에 맞춤

## 🧪 단일 이미지 테스트

1. `test_single_image.ipynb` 열기
2. `fire_smoke_model.pth` 로드
3. 이미지를 업로드하고 테스트 실행

## 📦 설치 환경

```bash
pip install -r requirements.txt
