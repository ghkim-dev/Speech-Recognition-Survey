# CHiME-3 / CHiME-4
> 2026-11-12: 기존 `CHiME-3-4.md`와 `CHiME-4.md`를 이 문서로 통합함. CHiME-4는 CHiME-3 데이터를 그대로 쓰고 테스트 시 사용 마이크 수만 제한한 후속 챌린지.

- **언어**: 영어 (WSJ0 5k 문장 낭독)
- **규모**: 학습 실녹음 1,600 + 시뮬레이션 7,138 문장(약 20시간), dev 1,640 / test 1,320 문장(실·시뮬 각각). 총 시간(전 세트 합계)은 미확인
- **녹음 환경**: 태블릿 프레임에 장착한 6채널 마이크 어레이로 버스·카페·길거리 교차로·보행자 구역 4개 환경에서 실녹음 + 시뮬레이션. 학습 실녹음에는 close-talk 마이크 1채널 추가
- **트랙**: CHiME-3는 6채널. CHiME-4는 같은 데이터로 6채널·2채널·1채널 트랙을 운영
- **Physical AI 활용 포인트**: 모바일/엣지 디바이스와 소형 로봇의 다채널 잡음 ASR, 빔포밍 front-end 평가, 실녹음과 시뮬레이션 사이 격차 분석
- **라이선스/연구 이용**: 미확인 (공식 사이트 약관 확인 필요. 원천 WSJ0는 LDC 코퍼스여서 LDC 라이선스가 필요할 수 있음)
- **접근 방식**: 미확인 (챌린지 사이트 신청 또는 LDC로 추정)
- **주요 사용 논문**:
  - [The third CHiME challenge (Barker 외, ASRU 2015)](../papers/2015-CHiME-3-Challenge.md)
  - [An analysis of environment, microphone and data simulation mismatches (Vincent 외, CSL 2017)](../papers/2017-CHiME-4-Mismatch-Analysis.md)
- **출처**: https://hal.archives-ouvertes.fr/hal-01211376 , https://signalprocessingsociety.org/publications-resources/data-challenges/chime-2016-4th-chime-speech-separation-and-recognition , https://merl.com/publications/TR2016-172
