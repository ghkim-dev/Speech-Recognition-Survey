# The CHiME-8 DASR Challenge for Generalizable and Array Agnostic Distant Automatic Speech Recognition and Diarization
- **저자**: Samuele Cornell 외 / CHiME 2024 Workshop (ISCA), arXiv 2407.16447
- **문제**: CHiME-7 DASR의 세 시나리오에 사무실 회의를 더해 일반화 범위를 넓히고, 평가 지표를 시간 제약을 두는 tcpWER로 바꿔 실제 전사 품질에 가깝게 평가
- **방법**: CHiME-6·DiPCo·Mixer 6·NOTSOFAR-1 네 시나리오, tcpWER(collar 5초) macro 평균으로 순위. ESPnet(CHiME-7 베이스라인 계승)과 NeMo 두 베이스라인 제공. 데이터 준비·채점 도구 `chime-utils` 공개
- **데이터셋/벤치마크**: [CHiME-7/8 DASR](../datasets/CHiME-7-8-DASR.md), [NOTSOFAR-1](../datasets/NOTSOFAR-1.md), [Mixer 6](../datasets/Mixer-6.md)
- **결과**: NeMo 베이스라인은 ESPnet보다 CHiME-6에서 크게 낫고 NOTSOFAR-1에서는 크게 나쁨(2차 자료). NTT 논문이 인용한 NeMo 베이스라인 dev macro tcpWER 약 50.0%, NTT 시스템 dev 21.3%(약 57% 상대 개선, arXiv 2409.05554). 상위 팀은 STCON·NTT이며 평가셋 최고 macro tcpWER는 STCON sys2의 19.6%(MOVER 논문 arXiv 2508.05055 인용값). 공식 표(Table 4)는 직접 확인하지 못함
- **Physical AI 시사점**: 가정·인터뷰·회의 등 성격이 다른 실내 환경을 한 시스템이 처리해야 한다는 조건은, 다양한 집과 사무실에 놓일 로봇·스마트 기기의 요구와 같음. DiPCo(dev 약 79%)처럼 소수 기기·강한 겹침 조건이 여전히 가장 어려움
- **링크**: https://arxiv.org/abs/2407.16447 , https://www.isca-archive.org/chime_2024/cornell24_chime.pdf , https://arxiv.org/abs/2507.18161
