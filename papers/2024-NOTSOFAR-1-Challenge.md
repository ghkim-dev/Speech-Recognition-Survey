# NOTSOFAR-1 Challenge: New Datasets, Baseline, and Tasks for Distant Meeting Transcription
- **저자**: Alon Vinnikov, Amir Ivry, Aviv Hurvitz, Igor Abramovski 외 (Microsoft) / Interspeech 2024, pp. 5003–5007, DOI 10.21437/Interspeech.2024-1788
- **문제**: 회의실 탁자 위 단일 장치로 여러 화자의 대화를 원거리에서 화자별로 전사하는 문제. 기존 회의 코퍼스(AMI 등)는 규모·조건 다양성·실측 음향 기반 학습 데이터가 부족함
- **방법**: (1) 회의실 30곳에서 수록한 실녹음 회의 237개와 조건 메타데이터 공개, (2) 실측 음향 전달함수 15,000개로 만든 약 1,000시간 시뮬레이션 학습셋 공개, (3) 단일 채널/다채널 두 트랙의 화자 귀속 전사 과제 정의(지표 tcpWER). CSS → Whisper → 화자 분할 베이스라인 제공
- **데이터셋/벤치마크**: [NOTSOFAR-1](../datasets/NOTSOFAR-1.md)
- **결과**: 베이스라인 Dev-set-1 tcpWER 단일 채널 46.8%, 다채널 32.4% (GitHub README). 챌린지에는 5개 팀 참가(Blue Sky Wave Riders, BUT JHU, NAIST, NPU, USTC-NERCSLIP). USTC-NERCSLIP는 Dev-set-2에서 다채널 14.3%, 단일 채널 23.0% tcpWER 보고(arXiv 2409.02041). 공식 최고 평가셋 수치는 미확인(요약 논문 arXiv 2501.17304 참고 필요)
- **Physical AI 시사점**: 고정 단일 기기의 원거리 다화자 인식 성능이 거리(화이트보드)·겹침·순간 잡음에 크게 좌우된다는 조건별 분석을 제공. 다채널이 단일 채널보다 tcpWER 약 14%p 낮아, 로봇·스마트 기기에 마이크 어레이를 넣는 근거가 됨. 실측 전달함수 기반 대규모 시뮬레이션은 로봇 장착 어레이용 학습 데이터 합성 방법의 참고 사례
- **링크**: https://www.isca-archive.org/interspeech_2024/vinnikov24_interspeech.pdf , https://github.com/microsoft/NOTSOFAR1-Challenge , https://arxiv.org/abs/2501.17304
