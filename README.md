# 원격의료를 위한 AI 기반 의료영상 처리 연구

AI 기반 의료영상 처리 알고리즘을 원격의료에 적용하기 위한 연구를 정리한 프로젝트입니다. 의료영상의 객체 탐지·분할·분류 자동화를 통해 진단 정확도와 효율을 높이는 것을 목표로 합니다.

![IMG_5380](https://github.com/pigpgw/AI-based-medical-image-processing-algorithm-application-research-for-telemedicine/assets/133184988/306397ed-350c-44cf-aadd-664a39af3802)
그림 1. ICICT 2023 포스터상 수상

![IMG_9940](https://github.com/user-attachments/assets/793ec6f2-c662-4464-a30a-d9db26ee02ff)
그림 2. 조선대학교 총장배 모범상 수상

**수상**
- ICICT 2023 포스터상
- 조선대학교 총장배 모범상

**논문 정보**
- 제목: AI-based medical image processing algorithm application research for telemedicine
- 저자: Hee-Soo Ryoo, Woo-Young Jang, Geon-Woo Park
- 교신저자: danielh0609@chosun.ac.kr
- 소속: 조선대학교 AI 융합대학, 조선대학교 IT 융합 공학부 전자공학전공
- 수록: ICICT 2023 논문집 (PDF 58–62페이지, 인쇄 페이지 57–61)

**연구 요약**
의료영상 빅데이터와 딥러닝을 활용해 영상 판독, 질병 진단, 예후 예측이 가능한 AI 시스템의 모델 최적화 과정을 검증했습니다. 주요 하이퍼파라미터 중 `optimizer`에 집중하여 U-Net, ResNet50, U-Net+ResNet50 구조에서 뇌종양 및 폐질환 영상에 대한 학습 성능을 비교·분석했으며, Adam optimizer가 뇌와 폐 데이터에서 가장 우수한 성능과 빠른 수렴을 보였습니다.

**핵심 기여**
- 원격의료 환경에서 활용 가능한 AI 의료영상 처리 파이프라인 제안
- Optimizer(Adam, SGD, AdaGrad, RMSprop)별 성능 비교 실험
- U-Net, ResNet50, U-Net+ResNet50 기반 모델 성능 평가

**방법 개요**
- 의료영상 데이터 수집 및 전처리
- 모델 구조: U-Net, ResNet50, U-Net+ResNet50
- Optimizer 비교: Adam, SGD, AdaGrad, RMSprop
- 평가 지표: Accuracy, Loss
- 옵티마이저 특성: SGD(기본), AdaGrad(적응 학습률), RMSprop(누적 영향 완화), Adam(모멘텀+RMSprop, 빠른 수렴)

**결과 요약**
- 뇌종양: Adam optimizer가 최고 성능(정확도 약 0.97 수준)
- 폐질환: Adam optimizer가 가장 빠른 수렴 및 높은 정확도
- Adam 기반 U-Net+ResNet50에서 예측 및 UI/UX 검증 화면 제시

**결과 표 (핵심만)**  
각 모델에서 가장 좋은 성능을 보인 옵티마이저 기준 요약입니다.

| 모델 | 부위 | 최고 성능 옵티마이저 | 정확도 | 손실 |
|---|---|---|---:|---:|
| U-Net | 뇌종양 | Adam | 0.9816 | 0.072 |
| U-Net | 폐질환 | Adam | 0.3667 | 1.1731 |
| ResNet50 | 뇌종양 | Adam | 0.98 | 0.093 |
| ResNet50 | 폐질환 | Adam | 0.9726 | 0.1104 |
| U-Net+ResNet50 | 뇌종양 | Adam | 0.9816 | 0.65 |
| U-Net+ResNet50 | 폐질환 | Adam | 0.3667 | 1.1731 |

표 1. 모델별 최고 성능 요약(정확도/손실)

**의의**
AI 기반 의료영상 처리의 자동화는 원격의료에서 의료진 부담을 줄이고 진단 정확도를 개선하는 핵심 기술로 작동할 수 있으며, 신뢰성·일반화·규제 준수 측면의 추가 연구가 중요합니다.

**그림 캡션(논문)**
- 그림 1. AI 모델 생성 구조
- 그림 2. U-Net+ResNet50 기반 모델 개발 및 성능 다이어그램
- 그림 3. U-Net+ResNet50 구조 기반 검증 결과 및 실행 메뉴(UI/UX)

**감사의 글**
본 연구는 과학기술정보통신부 AI Healthcare Convergence College 프로그램(2023)의 지원을 받아 수행되었습니다.
