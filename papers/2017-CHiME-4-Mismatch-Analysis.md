# An analysis of environment, microphone and data simulation mismatches in robust speech recognition
- **저자**: Emmanuel Vincent, Shinji Watanabe, Aditya Arie Nugraha, Jon Barker, Ricard Marxer / Computer Speech & Language 46, pp. 535–557, 2017 (MERL TR2016-172 프리프린트)
- **문제**: 잡음 환경, 마이크 수·위치, 데이터 시뮬레이션 방식의 학습/테스트 불일치가 강건 ASR 성능에 주는 영향
- **방법**: CHiME-3 데이터(6채널 태블릿 어레이)로 환경·마이크·실녹음/시뮬레이션 불일치 조건을 나누어 비교 분석
- **데이터셋/벤치마크**: [CHiME-3/4](../datasets/CHiME-3-4.md)
- **결과**: MVDR 빔포밍을 제외한 대부분의 기법은 실녹음과 시뮬레이션 데이터에서 성능이 비슷함. 학습 시 잡음 환경·마이크 차이는 정확도에 영향이 작고, 테스트 시 마이크 수가 가장 중요함. 이 결과가 CHiME-4에서 테스트 마이크 수를 줄인 근거가 됨 (2차 자료 기준, 정량 수치는 미확인)
- **Physical AI 시사점**: 로봇·엣지 기기에서는 마이크 개수가 성능을 좌우하므로 하드웨어 설계 단계에서 고려해야 함. 시뮬레이션 학습 데이터는 대체로 유효하지만 MVDR 계열 front-end는 실녹음 검증이 필요
- **링크**: https://merl.com/publications/TR2016-172 , https://eprints.whiterose.ac.uk/111196/ , https://doi.org/10.1016/j.csl.2016.11.005
