# A Cocktail-Party Benchmark: Multi-Modal dataset and Comparative Evaluation Results
- **저자**: Thai-Binh Nguyen 외 (KIT, CMU, Meta AI, Interactive-AI) / arXiv 2510.23276 (2025-10 v1, 2026-02 v2), CHiME-9 Task 1
- **문제**: 한 방에서 여러 대화가 동시에 오가는 칵테일파티 상황에서 각 화자의 발화를 전사하고, 누가 누구와 대화 중인지까지 묶어야 하는 문제. 기존 다화자 ASR 벤치마크는 하나의 대화만 가정
- **방법**: [CHiME-9 MCoRec](../datasets/CHiME-9-MCoRec.md) 데이터(150세션, 중앙 360° 카메라 영상 + 단일 채널 음성) 공개. 베이스라인은 능동 화자 검출 → 얼굴 랜드마크·입 영역 크롭 → 15초 단위 AVSR 디코딩 → 발화 시간 겹침 기반 대화 클러스터링으로 구성. AVSR 모델 4종(AV-HuBERT CTC/Attention, MuAViC-EN, Auto-AVSR, MCoRec 미세조정판) 비교
- **데이터셋/벤치마크**: CHiME-9 MCoRec (train 5.6시간, dev 2.5시간, eval 6.9시간)
- **결과**: 오디오만 쓰면 WER이 100%를 넘고, 시각 정보를 넣으면 약 50% 개선(초록). 최고 베이스라인 dev Joint ASR-Clustering Error Rate 0.3548(화자 WER 0.4990, 클러스터링 F1 0.8153; 공식 baseline README)
- **Physical AI 시사점**: 단일 마이크로는 동시 대화를 사실상 분리할 수 없고 카메라의 입술 정보가 결정적이라는 점을 수치로 보여 줌. 로봇이 방 안 여러 그룹 중 자신에게 말하는 그룹을 고르고 해당 화자 발화만 인식하는 시청각 파이프라인의 기준점
- **링크**: https://arxiv.org/abs/2510.23276 , https://github.com/MCoRec/mcorec_baseline
