# CAVEMOVE: An Acoustic Database for the Study of Voice-enabled Technologies inside Moving Vehicles
- **저자**: Nikolaos Stefanakis, Andreas Symiakakis 외 (FORTH-ICS) / arXiv 2508.19691 (2025). 학회 게재 여부 미확인
- **문제**: 차량 음성 비서 연구에는 주행 조건별 실내 잡음과 승객 위치별 음향 경로가 필요하지만, 공개 차량 음성 DB(AVICAR, SpeechDat-Car, CU-Move 등)는 오래됐거나 유료·제한 라이선스인 경우가 많음
- **방법**: 실제 승용차에서 (i) 승객 위치별 실측 임펄스 응답(정지 상태), (ii) 속도·창문 개방 조건별 정지/주행 잡음을 소형 원형 8마이크 어레이와 분산 마이크 두 구성으로 수록. 수록 과정을 7번 반복해 여러 차량을 포함(차량 수 3대/4대 출처 불일치). Python/MATLAB API로 사용자 음성과 잡음·차량 오디오 간섭을 섞어 다채널 신호 합성
- **데이터셋/벤치마크**: [CAVEMOVE](../datasets/CAVEMOVE.md)
- **결과**: 데이터·도구 공개 논문. 속도별 잡음 특성 분석이나 ASR/향상 평가 수치는 미확인(arxiv.org 접속 불가로 본문 미확인)
- **Physical AI 시사점**: 자율주행·차량 축에서 바로 쓸 수 있는 최신 공개 실측 음향 DB. 음성 대신 임펄스 응답과 잡음을 주므로 LibriSpeech 등 어떤 음성이든 차량 원거리 조건으로 바꿀 수 있고, 운전자/동승자 위치별 신호로 화자 위치 추정·대상 화자 추출 연구도 가능
- **링크**: https://arxiv.org/abs/2508.19691 , https://github.com/SPL-FORTH-ICS/CAVEMOVE , https://zenodo.org/records/17404917
