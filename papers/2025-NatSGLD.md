# NatSGLD: A Dataset with Speech, Gesture, Logic, and Demonstration for Robot Learning in Natural Human-Robot Interaction
- **저자**: Snehesh Shrestha, Yantian Zha, Saketh Banagiri, Ge Gao, Yiannis Aloimonos, Cornelia Fermüller (University of Maryland) / ACM/IEEE HRI 2025 (arXiv 2502.16718)
- **문제**: 기존 HRI 다중 모달 데이터는 가리키기·밀기 같은 단순 과제 위주이고, 사람 명령을 로봇이 "올바르게 해석"했는지의 정답(과제 의미 표현)이 부족
- **방법**: Wizard-of-Oz로 참가자 18명이 시뮬레이터 속 로봇에게 요리 과제를 자연스러운 음성·제스처로 지시. 각 명령에 시연 궤적과 LTL 공식(과제의 정답 해석)을 짝지어 1,143개 명령 수집. 데이터·Unity/ROS 시뮬레이터·코드를 MIT 라이선스로 공개
- **데이터셋**: [NatSGLD](../datasets/NatSGLD.md)
- **결과**: 2차 자료 기준 다중 모달 지시 따르기, 계획 인식, 시연 기반 강화학습 연구용 기반 자원으로 제시. 논문 내 정량 베이스라인 수치는 이번 세션에서 원문(arxiv, ACM DL) 접속 불가로 미확인
- **Physical AI 시사점**: 음성 명령을 바로 행동으로 매핑하는 VLA와 달리, "음성+제스처 → 형식 논리(LTL) → 행동" 경로의 정답을 제공해 해석 가능성과 검증을 평가할 수 있음. 전 단계 [NatSGD](2024-NatSGD.md)(arXiv 2403.02274, 음성·제스처·시연)에 LTL 정답을 더한 확장판
- **링크**: https://arxiv.org/abs/2502.16718 , https://github.com/sneheshs/natsgld , https://www.snehesh.com/natsgld
