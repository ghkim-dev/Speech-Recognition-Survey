# The CHiME-7 DASR Challenge: Distant Meeting Transcription with Multiple Devices in Diverse Scenarios
- **저자**: Samuele Cornell 외 10명 / CHiME 2023 Workshop (ISCA), arXiv 2306.13734
- **문제**: 기존 CHiME-5/6는 단일 시나리오(가정 저녁 식사)·고정 장치 구성만 다뤄, 장치 수와 배열 구조가 다른 환경으로의 일반화를 평가하지 못함
- **방법**: CHiME-6·DiPCo·Mixer 6 세 시나리오를 공통 형식으로 통합하고, 한 시스템으로 세 시나리오를 모두 처리하는 화자 분할+ASR 과제 정의. 이전 CHiME과 달리 공개 사전학습 모델·외부 공개 데이터 사용 허용. 배열 구조 무관 베이스라인(다채널 화자 분할 → 채널 선택 → GSS → SSL 표현 기반 ASR) 제공. 오라클 분할을 주는 sub-track과 전체를 수행하는 main track으로 구분
- **데이터셋/벤치마크**: [CHiME-7/8 DASR](../datasets/CHiME-7-8-DASR.md), [CHiME-6](../datasets/CHiME-6.md), [DiPCo](../datasets/DiPCo.md), [Mixer 6](../datasets/Mixer-6.md)
- **결과**: 베이스라인 macro DA-WER main track dev 47.2% / eval 55.3%, sub-track dev 28.8% / eval 33.4%. Whisper large도 비슷한 수준이며 오라클 분할에서도 실사용 수준에 못 미친다고 보고 (2차 자료). 참가 팀 중 USTC-NERCSLIP가 eval macro DA-WER 21.01%(베이스라인 대비 약 62% 상대 개선)로 1위를 주장(arXiv 2308.14638, 공식 순위표는 미확인)
- **Physical AI 시사점**: 기기마다 다른 마이크 배치에서도 쓸 수 있는 "배열 무관" 원거리 다화자 인식을 정식 과제로 만든 첫 CHiME. 대형 사전학습 모델을 허용하면서 GSS 같은 다채널 전처리와 대형 ASR 모델의 결합이 표준 구성이 됨
- **링크**: https://arxiv.org/abs/2306.13734 , https://www.isca-archive.org/chime_2023/cornell23_chime.html
