# CHiME-9 ECHI: A Machine Learning Challenge for Enhancing Conversations to Address Hearing Impairment
- **저자**: Robert Sutherland, Thomas Kuebert, Marko Lugger, Stefan Petrausch, Eline Borch Petersen, Juan Azcarreta Ortiz, Buye Xu, Stefan Goetze, Jon Barker / arXiv 2609.26306 (2026), CHiME-9 Task 2 (CHiME 2026 Workshop)
- **문제**: 시끄러운 카페테리아에서 다자 대화를 할 때, 착용형 기기(보청기·스마트 안경)가 대화 상대들의 목소리만 낮은 지연으로 분리해 들려주는 문제. 기존 향상 챌린지는 고정 마이크·시뮬레이션 위주였음
- **방법**: [CHiME-9 ECHI](../datasets/CHiME-9-ECHI.md) 데이터(4인 대화, Aria 7채널·보청기 4채널, 머리 추적, 근접 기준 신호, 참여자 깨끗한 음성) 공개. 베이스라인은 TF-GridNet 기반 대상 화자 추출(TSX) 모델을 단방향 LSTM·마스크드 self-attention으로 인과적으로 바꿔 지연 제한을 맞춤. 학습 데이터만 사용, STOI로 dev 튜닝. 평가는 참조 기반 객관 지표, 참조 없는 DNN 예측 지표, 청취 실험(명료도·음질) 세 갈래
- **데이터셋/벤치마크**: CHiME-9 ECHI (train 18시간, dev 약 6시간, eval 약 5.4시간)
- **결과**: 상위 시스템이 청취 실험의 명료도·음질 모두에서 베이스라인 대비 크게 개선. 객관 지표가 실제 청취자 평가를 잘 반영하지 못한다는 점을 주요 결론으로 보고(초록). 베이스라인 dev Aria 55.28, 보청기 43.94 등의 수치가 2차 자료에 보이나 어떤 지표인지 확인 못함(미확인)
- **Physical AI 시사점**: 착용자 머리가 움직이는 어레이, 자기 발화·방해 화자가 섞인 상황에서 "등록된 대화 상대" 음성만 추출하는 설정은 사람과 대화하는 로봇의 전처리 문제와 같음. 객관 지표와 실제 체감의 괴리는 로봇 음성 인터페이스 평가에도 경고가 됨. 참가 시스템 중에는 자기 간섭(self-interference) 억제 단계를 넣은 3단계 구조도 있어(Zhao 외, CHiME 2026), 로봇 ego-speech 제거와 연결됨
- **링크**: https://arxiv.org/abs/2609.26306 , https://www.chimechallenge.org/current/task2/index , https://github.com/CHiME9-ECHI/CHiME9-ECHI , https://www.isca-archive.org/chime_2026/index.html
