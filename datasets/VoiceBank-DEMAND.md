# VoiceBank-DEMAND (Noisy speech database, Valentini-Botinhao)
- **언어**: 영어 (VCTK/Voice Bank 낭독 음성)
- **규모**: 28화자 버전 기준 학습 11,572문장(약 10시간), 테스트 824문장(화자 2명, 미등장 잡음 조건)
- **녹음 환경**: 깨끗한 낭독 음성에 DEMAND 환경 잡음 + 음성형 잡음(SSN)·babble을 인위적으로 섞음. 원본 48 kHz, 보통 16 kHz로 다운샘플링해 사용
- **Physical AI 활용 포인트**: 엣지 기기 음성 향상(SE) 전처리의 표준 벤치마크. 시뮬레이션 데이터라 실제 로봇 잡음에 대한 일반화는 따로 확인해야 함
- **라이선스/연구 이용**: CC BY 4.0 (여러 2차 자료 기준. DataShare 원문은 직접 확인 못함)
- **접근 방식**: 공개 (Edinburgh DataShare, DOI 10.7488/ds/2117)
- **주요 사용 논문**: [Valentini-Botinhao et al., SSW 2016](../papers/2016-VoiceBank-DEMAND-RNN-SE-TTS.md), SEGAN, PHASEN 등 다수 SE 논문
- **출처**: https://commons.datacite.org/doi.org/10.7488/ds/2117 , https://arxiv.org/pdf/2106.04624 , https://arxiv.org/pdf/2405.16834
