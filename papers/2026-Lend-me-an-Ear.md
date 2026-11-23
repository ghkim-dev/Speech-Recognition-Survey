# Lend me an Ear: Speech Enhancement Using a Robotic Arm with a Microphone Array
- **저자**: Zachary Turcotte, François Grondin (Université de Sherbrooke 추정, 소속 미확인) / arXiv 2602.17818 (2026-02-19, cs.RO / cs.SD), 게재 학회 미확인
- **문제**: 공장처럼 시끄러운 환경에서는 음성 향상 성능이 떨어져 음성 제어 도구 사용이 어려움. 로봇에 쓰이는 마이크 어레이는 대부분 기하 구조가 고정되어 있어 화자·잡음 배치에 맞춰 바꿀 수 없음
- **방법**: Kinova Gen3 7자유도 산업용 매니퓰레이터에 무지향 마이크 16개를 서브어레이 4개로 나눠 여러 관절에 부착(1개는 엔드이펙터 근처). (1) 화자 위치 추정 → (2) 역기구학으로 청취에 유리한 관절 각을 계산해 팔을 움직여 어레이 형상을 실시간 재구성 → (3) 어레이 구조에 무관한 DNN IRM(ideal ratio mask) 추정 + MVDR 빔포머로 향상
- **데이터셋/평가 조건**: 음성과 잡음을 입력 SNR -5, 0, 5, 10 dB로 혼합. 혼합 수는 버전마다 SNR당 1,944개 또는 10,368개로 다르게 보고(미확인). 사용한 음성·잡음 코퍼스 이름과 시뮬레이션/실녹음 여부는 미확인
- **지표·결과**: SI-SDR(개선량)과 WER. 웹 요약 기준으로 재구성 어레이가 여러 SNR에서 고정 어레이보다 우수하다고 보고되나 **구체 수치는 미확인** (arxiv.org 직접 접속 불가)
- **공개 여부**: 코드·데이터 공개 저장소는 GitHub 검색으로 찾지 못함(미확인)
- **Physical AI 시사점**: 로봇이 "귀를 화자 쪽으로 가져가는" 능동 청취(active audition)를 매니퓰레이터 기구학과 결합한 사례. 고정 어레이 가정에서 벗어나 로봇 몸체 자체를 가변 어레이로 쓰는 방향이며, 어레이 무관(array-agnostic) 향상 모델(CHiME-7/8 DASR의 배열 무관 평가 흐름)과 맞물림. 같은 연구실의 로봇 청각 도구([ODAS](2022-ODAS.md), MIT 공개, Sherbrooke IntRoLab)와 이어지는 계보로 보임(추정)
- **링크**: https://arxiv.org/abs/2602.17818 , https://arxiv.org/html/2602.17818v1
