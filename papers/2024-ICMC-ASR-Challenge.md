# ICMC-ASR: The ICASSP 2024 In-Car Multi-Channel Automatic Speech Recognition Challenge
- **저자**: He Wang, Lei Xie 외 (ICMC-ASR 조직위: NWPU ASLP, AISHELL, Li Auto 등으로 추정 — 전체 저자·소속 원문 미확인) / IEEE ICASSP 2024 Grand Challenge (arXiv 2401.03473)
- **문제**: 차량 내 좁은 공간 잔향, 주행 잡음, 운전자·동승자 겹침 발화가 동시에 있는 실차 다채널 데이터와 공통 평가 기준이 없었음
- **방법**: 하이브리드 전기차 4개 좌석(운전석·조수석·뒷좌석 2) 화자의 표준 중국어 대화를 원거리 다채널+근접 마이크로 녹음. 트랙 I(ASR, 정답 구간 제공, CER), 트랙 II(화자 분할+인식, cpCER). 공식 베이스라인은 AEC+IVA 프런트엔드 → pyannote VAD → E-Branchformer
- **데이터셋**: 챌린지 데이터 — Train 94.75시간(568세션), Dev 3.33시간, Eval_1 3.30시간, Eval_2 3.58시간(각 18세션), 잡음 40.29시간(60세션). 이 분할 통계가 [AISHELL-5](../datasets/AISHELL-5.md)와 정확히 같아, AISHELL-5는 ICMC-ASR 데이터를 공개 배포한 것으로 판단됨(두 논문 수치 비교로 추정, 공식 명시 문구는 미확인). IEEE SPS 공지 페이지의 "1,000시간+ 음성·400시간+ 잡음"은 실제 배포 규모와 달라 사전 공지 수치로 보임
- **결과**: 98팀 참가, 유효 제출 53건. 베이스라인 트랙 I CER 26.24%, 트랙 II cpCER 72.88%. 1위 USTC-iflytek 트랙 I 13.16%, 트랙 II 21.48%. 1위 시스템은 GSS(Guided Source Separation)의 채널 선택 기준을 SNR 대신 에너지·위상 차이로 바꾸고, 비전사 데이터 반복 의사 레이블링과 억양 최적화 Accent-ASR, 다채널 TS-VAD 화자 분할을 사용 (웹 검색 결과로 확인, USTC-NERCSLIP 시스템 논문 arXiv 2407.02052)
- **Physical AI 시사점**: 차량(이동 플랫폼)에서 베이스라인 대비 cpCER를 72.9→21.5%로 줄인 핵심은 프런트엔드(GSS 채널 선택)와 화자 분할(TS-VAD)로, AISHELL-5 베이스라인의 "분리 프런트엔드가 병목" 결론과 일치. CHiME-6/7 원거리 회의 기법(GSS, TS-VAD)이 차량에도 그대로 이전됨
- **링크**: https://arxiv.org/abs/2401.03473 , https://arxiv.org/abs/2407.02052 , https://signalprocessingsociety.org/publications-resources/data-challenges/car-multi-channel-automatic-speech-recognition-challenge
