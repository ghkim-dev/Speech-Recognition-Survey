# Audio-Based Search and Rescue with a Drone: Highlights from the IEEE Signal Processing Cup 2019 Student Competition
- **저자**: Antoine Deleforge, Diego Di Carlo, Martin Strauss, Romain Serizel, Lucio Marcenaro / **IEEE Signal Processing Magazine** 36(5):138–144, 2019 (DOI 10.1109/MSP.2019.2924687, arXiv 1907.04655)
- **문제**: 수색·구조 드론이 조난자 목소리 방향을 찾으려 해도 로터·바람 잡음이 매우 커서 기존 음원 위치 추정이 잘 안 됨
- **방법**: 6회 IEEE SP Cup(학부생 대회)으로 "드론 탑재 마이크 어레이 음원 위치 추정"을 출제. DREGON 장비로 녹음한 정지 과제(300개)와 비행 과제(36개)를 제공하고, 참가팀 접근법과 결과를 정리
- **데이터셋/벤치마크**: [SPCUP19](../datasets/SPCup19-Drone-SSL.md) (DREGON 기반)
- **결과**: 결선은 ICASSP 2019(영국 브라이턴, 5월 13일). 결선 진출팀 중 AGH University of Science and Technology, Soongsil University(Idea!_ssu) 확인. 우승팀·과제별 정확도는 **미확인**(arxiv.org·IEEE 페이지 접속 불가, 검색 스니펫에 없음)
- **Physical AI 시사점**: 로봇 ego-noise 아래 음성 위치 추정을 "공개 정답 + 표준 지표"로 묶은 초기 IEEE 벤치마크. 이후 DroneAudioSet(2025)·rotor-conditioned 모델(2025)·UAV KWS(2026)로 이어지는 드론 청각 연구의 출발점
- **링크**: https://arxiv.org/abs/1907.04655 , https://hal.archives-ouvertes.fr/hal-02161897 , https://www.semanticscholar.org/paper/ccdc288aebe5806cab113ef247902e11a3252b0a
