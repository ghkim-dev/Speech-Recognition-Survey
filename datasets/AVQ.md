# AVQ (Audio-Visual sensing from a Quadcopter)
- **언어**: 영어 음성(사람 발화 + 사람이 들고 다니는 스피커 재생)
- **규모** (저자 IROS 2019 발표 자료 기준, 2차 자료): 시청각 시퀀스 12개, 총 약 50분. 예: 시퀀스 1~3은 음성 없는 ego-noise(120·120·40초, 드론 출력 50%), 시퀀스 4는 드론 정지 상태 음성만(797초, 화자 2명·위치 9곳). 시퀀스별 전체 표는 확인하지 못함 → 미확인
- **구성**: S1(고정 위치 음원)·S2(이동 음원) 두 부분, 시나리오는 natural(실제 녹음)·composite(ego-noise와 음성을 따로 녹음해 합성) 두 종류. 화자 위치·음성 구간(VAD) 정답 포함
- **녹음 환경**: 실외. 3DR IRIS 쿼드콥터에 원형 8채널 마이크 어레이(44.1 kHz)와 카메라(HD 30 fps) 장착. 시청각 보정으로 영상에서 화자 위치 정답을 만듦. ego-noise로 SNR이 −15 dB보다 낮아지는 구간이 많음
- **Physical AI 활용 포인트**: 공개된 드론 청각 데이터 중 드문 **실외·시청각** 녹음. 실내 정지·비행 녹음인 [DREGON](DREGON.md)/[SPCUP19](SPCup19-Drone-SSL.md)를 보완해, 카메라로 사람을 찾고 마이크로 그 방향의 음성을 향상하는 멀티모달 파이프라인 평가에 쓸 수 있음
- **라이선스/연구 이용**: 미확인 (프로젝트 페이지 직접 접속 불가)
- **접근 방식**: QMUL 프로젝트 페이지에서 공개된 것으로 소개됨. 단, [DroneAudioSet](DroneAudioSet.md) 논문(2025)은 AVQ를 "공개되지 않음"으로 서술해 서로 엇갈림 → 현재 다운로드 가능 여부 미확인
- **주요 사용 논문**: [Wang, Sanchez-Matilla, Cavallaro, IROS 2019](../papers/2019-AVQ-Audio-Visual-Quadcopter.md)
- **출처**: https://cis.eecs.qmul.ac.uk/projects/avq/ , https://webspace.eecs.qmul.ac.uk/lin.wang/demo/avq.html , https://risama.github.io/files/2019_IROS/paper.pdf , https://risama.github.io/files/2019_IROS/presentation.pdf , https://arxiv.org/html/2510.15383v1 (모두 웹 검색 결과로 확인, 직접 접속 불가)
