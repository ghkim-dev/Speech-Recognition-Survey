# DroFiT: A Lightweight Band-fused Frequency Attention Toward Real-time UAV Speech Enhancement
- **저자**: Jeongmin Lee, Chanhong Jeon, Hyungjoo Seo, Taewook Kang (성균관대·UIUC, 2차 자료 기준) / arXiv 2509.16945 (2025-09, v2 2026-03). 데모 페이지에 ICASSP 2026 투고로 표기, 채택 여부 미확인
- **문제**: 드론 자체 잡음이 매우 커 음성이 −5~−25 dB SNR로 들어오는데, 기존 음성 향상 모델은 기체 탑재 연산·메모리 예산에 비해 무거움
- **방법**: 단일 마이크 음성 향상. 주파수 축 Transformer + 전대역(full-band)/부대역(sub-band) 혼합 인코더-디코더, 스트리밍용 TCN 백엔드, 학습 가능한 skip-and-gate 결합, 스펙트럼-시간 결합 손실. 데모 페이지 설정: 모델 차원 32, 어텐션 헤드 16, 4층, FFN 128, TCN 커널 3
- **데이터**: [VoiceBank-DEMAND](../datasets/VoiceBank-DEMAND.md) 음성 + DJI Flip을 실제로 띄워 녹음한 드론 잡음(약 9000초) 혼합, 16 kHz, −5~−25 dB(추가로 −30 dB 실험). 드론 잡음 녹음 공개 여부 미확인
- **결과** (2차 요약 기준, 원문 표 확인 못 함): DCU-Net, SMoLnet-T 대비 비슷한 향상 성능에 연산량 약 47%, 메모리 약 53% 감소. 극저 SNR에서 PESQ 1.2 이상 개선 → 미확인
- **Physical AI 시사점**: [UAV KWS 프런트엔드 논문](2026-UAV-KWS-Noise-Floor-Front-Ends.md)·[rotor-conditioned 드론 청각](2025-Rotor-Conditioned-Drone-Audition.md)과 함께, 드론 음성 인터페이스를 기체 탑재 실시간 처리로 옮기려는 흐름. 다만 로터 상태를 입력으로 쓰지 않는 순수 신호 기반 방식이어서, 조건화 방식과 실제 비행 녹음에서 비교할 필요가 있음
- **링크**: https://arxiv.org/abs/2509.16945 , https://ml-sp.github.io/DroFiT
