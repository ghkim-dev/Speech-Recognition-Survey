# Audio-visual sensing from a quadcopter: dataset and baselines for source localization and sound enhancement
- **저자**: Lin Wang, Ricardo Sanchez-Matilla, Andrea Cavallaro (Queen Mary University of London, Centre for Intelligent Sensing) / IEEE/RSJ IROS 2019 (Macau), pp. 5320–5325
- **문제**: 드론 탑재 마이크는 로터 ego-noise 때문에 SNR이 −15 dB 이하로 떨어지는데, 실외에서 영상과 소리를 함께 정답과 함께 녹음한 공개 데이터가 없었음
- **방법**: 3DR IRIS 쿼드콥터에 원형 8채널 마이크 어레이와 카메라를 달아 고정 음원(S1)·이동 음원(S2) 시퀀스를 녹음. 시청각 보정으로 영상에서 화자 위치 정답을 만들고, 음원 위치 추정·음성 향상 기준(baseline) 결과를 제시 (구체 알고리즘·수치는 직접 확인 못 함 → 미확인)
- **데이터셋**: [AVQ](../datasets/AVQ.md) (12개 시퀀스, 약 50분)
- **Physical AI 시사점**: 드론 청각을 "소리만"에서 "영상+소리"로 넓힌 초기 데이터. 같은 그룹의 후속 연구(Multi-modal localization and enhancement of multiple sound sources from a micro aerial vehicle)로 이어짐. 카메라로 사람을 찾고 그 방향을 마이크 빔포밍에 주는 구조는 최근 로봇 상태·외부 정보를 음성 처리 조건으로 쓰는 흐름(rotor-conditioned SE, UAV KWS 조건화)의 시각 버전
- **링크**: https://risama.github.io/publication/2019_IROS , https://cis.eecs.qmul.ac.uk/projects/avq/
