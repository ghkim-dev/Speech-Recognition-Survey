# NatSGD: A Dataset with Speech, Gestures, and Demonstrations for Robot Learning in Natural Human-Robot Interaction
- **저자**: Snehesh Shrestha 외 공저자 5명(Yiannis Aloimonos, Cornelia Fermüller 포함, University of Maryland; 나머지 저자명은 원문 미확인) / arXiv 2403.02274 (2024-03). 학회 게재 여부 미확인(검색 결과에서 확인되지 않음)
- **문제**: 기존 HRI 데이터는 음성 또는 제스처 한쪽이거나 단순 과제 위주이며, 자연스러운 다중 모달 명령과 로봇 행동 시연이 동기화된 자원이 부족
- **방법**: WoZ로 18명이 시뮬레이션 주방 로봇에게 음성·제스처로 지시한 1,143개 명령을 수집하고 전문가 시연 궤적과 짝지음. 음성·제스처 조건 모방학습과, BART/T5를 미세조정해 명령을 LTL로 바꾸는 Comm2LTL 벤치마크 제시
- **데이터셋**: [NatSGD](../datasets/NatSGD.md)
- **결과**: Comm2LTL(GitHub README) — BART: 음성만 Spot Score 0.434, 제스처만 0.299, 음성+제스처 0.588 / T5: 0.299, 0.244, 0.507. Jaccard 유사도는 0.92~0.96으로 모두 높아 변별력이 약하고, 정확 일치에 가까운 Spot Score에서 모달 결합 이득이 뚜렷함. 논문 본문의 모방학습 성공률 수치는 원문 접속 불가로 미확인
- **Physical AI 시사점**: 텍스트(전사)만으로는 지시 대상이 모호한 명령이 많아, 음성 인식 결과에 제스처를 더해야 과제 해석이 크게 좋아짐. 로봇 음성 명령 시스템 평가 시 ASR WER뿐 아니라 "해석 정확도(Spot Score류)"를 함께 볼 필요. 후속 [NatSGLD](2025-NatSGLD.md)(HRI 2025)의 전 단계
- **링크**: https://arxiv.org/abs/2403.02274 , https://github.com/sneheshs/NATSGD_Comm2LTL , https://www.snehesh.com/natsgd
