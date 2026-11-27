# End-to-end Listen, Look, Speak and Act (ELLSA)
- **저자**: Siyin Wang, Wenyi Yu, Xianzhao Chen, Xiaohai Tian, Jun Zhang, Lu Lu, Chao Zhang 외 (Tsinghua·ByteDance) / ICLR 2026 (arXiv 2510.16756, 2025-10)
- **문제**: 음성 대화와 로봇 행동을 별도 모델로 처리하면 실시간 끼어들기·동시 대화·행동이 어려움
- **방법**: 시각·텍스트·음성·행동을 하나의 구조에서 동시에 인지·생성하는 full-duplex end-to-end 모델. 모달리티별 전문가를 공용 어텐션으로 묶는 SA-MoE(Self-Attention Mixture-of-Experts)
- **데이터셋/벤치마크**: 음성 상호작용(Llama Questions, Web Questions, TriviaQA, AlpacaEval의 턴테이킹), 조작(SPATIAL/OBJECT/GOAL/LONG 스위트. LIBERO 계열로 보이나 미확인), 결함 있는 지시 거부 테스트
- **결과**: 조작 스위트 100.0/99.6/100.0/96.4%(2차 자료 기준). 음성·조작 모두에서 전용 모델과 비슷한 성능이라고 보고
- **Physical AI 시사점**: 음성 대화와 행동을 동시에 처리하는 휴머노이드형 상호작용의 방향. 후속작 ELLSA 2(arXiv 2610.21452)는 제스처·표정까지 확장
- **링크**: https://arxiv.org/abs/2510.16756 , https://proceedings.iclr.cc/paper_files/paper/2026/hash/6d8af672c0bca7a4be6f0cd0d229c05c-Abstract-Conference.html
