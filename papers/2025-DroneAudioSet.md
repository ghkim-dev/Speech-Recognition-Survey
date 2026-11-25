# DroneAudioset: An Audio Dataset for Drone-based Search and Rescue
- **저자**: Chitralekha Gupta*, Soundarya Ramesh*, Praveen Sasikumar, Kian Peen Yeo, Suranga Nanayakkara (*공동 1저자, Augmented Human Lab, National University of Singapore) / **NeurIPS 2025 Datasets and Benchmarks Track** (arXiv 2510.15383, 2025-10-17)
- **문제**: 수색·구조 드론은 주로 시각에 의존해 저시정·가림 상황에서 실패. 음향 감지는 대안이지만 모터·프로펠러·바람 ego-noise가 사람 소리를 가림. 기존 데이터는 다양성이 부족하거나(DREGON 등) 잡음과 음원을 따로 녹음해 합성한 것이라 실제 음향 상호작용이 빠져 있고, 표준 실험 설정이 없음
- **방법**: 프레임에 고정한 드론 2종을 실제로 돌리며 3개 방·스로틀·스피커 거리/음량·마이크 위치(위 8ch/아래 8ch/단일)를 바꿔 동시 녹음. 베이스라인 파이프라인: (1) 전통적 MVDR 빔포밍 + 스펙트럴 게이팅, (2) 신경망 잡음 억제 MP-SENet, (3) 혼합(MVDR+MP-SENet) → SSLAM(AudioSet 사전학습 분류기)으로 HV/HNV/NH 3범주 사람 존재 분류
- **데이터셋/벤치마크**: [DroneAudioSet](../datasets/DroneAudioSet.md) (자체 공개, 23.5시간, MIT)
- **결과**: 정량 수치(SNR 구간별 분류 정확도, 억제 기법별 비교)는 **미확인**(arxiv.org·NeurIPS 프록시 차단으로 본문 접근 불가). 초록 기준으로 마이크 배치 트레이드오프와 드론 잡음 인지형 처리 필요성을 설계 지침으로 제시
- **공개 여부**: 데이터(Hugging Face, MIT)·코드(GitHub) 공개
- **Physical AI 시사점**: 11-24 DREGON(실내 합성·위치 추정 중심)에서 한 단계 나아가 "로봇이 내는 잡음 + 실제 음원"을 같은 공간에서 동시 녹음한 대규모 벤치마크. 음성(HV)과 비음성 사람 소리(HNV)를 구분하는 분류 과제는 로봇의 "사람 감지 → 음성 명령 인식" 앞단에 해당. 다만 프레임 고정(비행 없음)이라 기체 움직임·바람 조건은 남은 과제
- **링크**: https://arxiv.org/abs/2510.15383 , https://neurips.cc/virtual/2025/poster/121409 , https://apps.ahlab.org/DroneAudioSet-code/ , https://github.com/augmented-human-lab/DroneAudioSet-code
