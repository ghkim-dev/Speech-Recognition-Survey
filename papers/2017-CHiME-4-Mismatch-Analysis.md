# An analysis of environment, microphone and data simulation mismatches in robust speech recognition
- **저자**: Emmanuel Vincent, Shinji Watanabe, Aditya Arie Nugraha, Jon Barker, Ricard Marxer / Computer Speech & Language 46 (2017) 535–557, DOI 10.1016/j.csl.2016.11.005
- **문제**: 잡음 환경, 마이크 수·위치, 시뮬레이션과 실녹음의 불일치가 ASR 성능에 미치는 영향
- **방법**: 발표된 CHiME-3 결과를 다시 분석하고 새 실험으로 각 요인을 분리
- **데이터셋**: CHiME-3 (6채널 태블릿). 이 분석이 CHiME-4(평가 시 사용 마이크 수 축소) 설계의 근거가 됨 → [CHiME-4](../datasets/CHiME-4.md)
- **결과**: MVDR 빔포밍을 빼면 대부분 기법이 실/시뮬레이션 데이터에서 비슷하게 동작하고 시뮬레이션 학습 데이터가 도움이 됨. 학습 시 잡음 환경이나 마이크를 바꾸는 효과는 작고, 마이크 수가 가장 크게 작용
- **Physical AI 시사점**: 로봇용 데이터를 시뮬레이션으로 늘리는 전략의 근거. 마이크 수가 핵심 설계 변수
- **링크**: https://eprints.whiterose.ac.uk/111196/ , https://merl.com/publications/TR2016-172
