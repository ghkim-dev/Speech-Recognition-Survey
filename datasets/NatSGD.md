# NatSGD (Natural Speech, Gestures, and Demonstrations)
- **언어**: 영어
- **규모**: 다중 모달 명령 1,143개, 참가자 18명, 행동 11종·객체 20종·상태 16종, 명령마다 전문가 시연 궤적 1개 (arXiv 초록, 검색 결과 기준). 총 녹음 시간 미확인
- **녹음 환경**: Wizard-of-Oz — 참가자가 시뮬레이터 속 로봇에게 주방 요리·정리 과제를 자연스러운 음성과 제스처로 지시. 화자 시점 영상, 객체·로봇 상태, 사람이 주석한 발화·제스처(제스처 종류, 사용 신체 부위), 전문가 시연 로봇 궤적 포함
- **Physical AI 활용 포인트**: 음성+제스처 조건 모방학습(지시 따르기)과 명령 → LTL 변환 벤치마크(Comm2LTL)에 사용. 같은 데이터를 확장한 [NatSGLD](NatSGLD.md)가 LTL 정답을 공식 레이블로 추가했으므로, 두 버전 중 NatSGLD가 최신·상위 호환에 가까움(명령 수 1,143개 동일)
- **라이선스/연구 이용**: 벤치마크 코드 저장소(sneheshs/NATSGD_Comm2LTL)는 MIT (GitHub API 확인). 데이터 자체 라이선스는 이번 세션에서 프로젝트 사이트 접속 불가로 미확인 (후속 NatSGLD는 데이터까지 MIT로 명시)
- **접근 방식**: 공개 (프로젝트 사이트 snehesh.com/natsgd, Comm2LTL용 파일은 README의 Google Drive 링크)
- **주요 사용 논문**: [NatSGD (arXiv 2024)](../papers/2024-NatSGD.md)
- **출처**: https://arxiv.org/abs/2403.02274 , https://raw.githubusercontent.com/sneheshs/NATSGD_Comm2LTL/main/README.md , https://www.snehesh.com/natsgd
