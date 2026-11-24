# DREGON: Dataset and Methods for UAV-Embedded Sound Source Localization
- **저자**: Martin Strauss(Strauß), Pol Mordel, Victor Miguet, Antoine Deleforge (Inria Rennes / Univ. Rennes 계열, 1저자는 FAU Erlangen 기록도 존재 — 소속 세부 미확인) / **IEEE/RSJ IROS 2018**, Madrid, pp. 5735-5742 (IEEE Xplore 8593581, HAL hal-01854878)
- **문제**: 드론 탑재 마이크는 로터·프로펠러 ego-noise가 매우 크고 비정상적이라 음원(특히 음성) 위치 추정이 어려움. 공개된 실측·정답 주석 데이터가 부족
- **방법**: 쿼드로터 탑재 정육면체 8채널 어레이로 정지·비행 녹음을 수집하고 Vicon 정답 궤적, 로터 속도, IMU를 함께 공개. 베이스라인으로 GCC-PHAT 계열과 MUSIC 계열의 여러 변형(각도 스펙트럼 기반 SSL)을 비교
- **데이터셋/벤치마크**: [DREGON](../datasets/DREGON.md) (자체 공개)
- **결과**: 큰 잡음 하에서도 광대역 음원(백색잡음)은 잘 찾았지만 **비행 중 음성 위치 추정은 여전히 어려움**(논문 결론 요약 기준, 정량 수치는 미확인). 후속 IEEE SP Cup 2019(20개 팀)에서도 정지 음성·비행 광대역 과제는 상위 팀이 95% 이상 정답이었던 반면, SAR 시나리오에 가장 가까운 비행 중 음성 과제는 9개 팀만 5%를 넘겼고 우승 팀이 65%(SP Magazine 2019 보고치)
- **공개 여부**: 데이터·MATLAB 베이스라인 공개 (http://dregon.inria.fr), 학술·교육 목적 무료
- **Physical AI 시사점**: "로봇이 움직이는 순간 음성 인터페이스가 무너지는" ego-noise 문제를 정량화한 대표 공개 벤치마크. 로터 속도·IMU 같은 **로봇 내부 상태를 잡음 모델의 입력으로 활용**할 수 있게 한 점이 지상 로봇(Pepper ego-speech, MChRSR 이동 잡음)과 차별점이며, 11-23 LOCATA(이동 어레이)·ODAS(저전력 SSL)와 같은 앞단 파이프라인을 극한 잡음 조건으로 확장하는 데이터로 볼 수 있음
- **링크**: https://hal.inria.fr/hal-01854878 , https://ieeexplore.ieee.org/document/8593581/ , https://dregon.inria.fr/ , https://arxiv.org/abs/1907.04655
