# 🔥 Wildfire Smoke Detector

딥러닝을 이용한 산불 및 연기 탐지 모델입니다. Kaggle 및 AI Hub의 산불/연기 이미지 데이터를 학습시켜, 실제 CCTV 이미지나 단일 이미지에서도 연기 및 불꽃을 탐지할 수 있습니다.

---

## 📁 프로젝트 구성

- `train_model.ipynb`: 모델을 학습하는 Google Colab 노트북
- `test_model.ipynb`: 학습된 모델로 단일 이미지를 예측하는 노트북
- `wildfireandsmokedetector.ipynb`: 학습 및 테스트에 사용된 예측 모델 노트북
- `requirements.txt`: 필요한 라이브러리 목록
- `README.md`: 프로젝트 소개 문서

---

## 🧠 사용한 모델

- ResNet-18 (ImageNet 사전학습 모델 기반)
- Fine-tuning 후 FC layer를 클래스 수(예: `['Smoke', 'fire']`)에 맞게 교체

---

## 🔽 모델 다운로드

학습된 모델 가중치는 Google Drive에서 다운로드할 수 있습니다:

👉 [fire_smoke_model.pth 다운로드](https://drive.google.com/uc?export=download&id=1yj8STJjaObQfESdwFoZrMsSzf9Kq9NUB)

> 위 링크에서 `YOUR_FILE_ID_HERE` 부분을 실제 Google Drive 파일 ID로 바꿔주세요!

---

## 🧪 단일 이미지 테스트

1. `test_single_image.ipynb` 열기
2. 위의 링크에서 `fire_smoke_model.pth` 다운로드 후 Colab에 업로드
3. 예측하고 싶은 이미지를 업로드한 뒤 실행

---

## 📦 설치 환경

```bash
pip install -r requirements.txt
