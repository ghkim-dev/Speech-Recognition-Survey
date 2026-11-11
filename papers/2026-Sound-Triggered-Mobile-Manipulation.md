# From Instruction to Event: Sound-Triggered Mobile Manipulation
- **저자**: Hao Ju, Shaofei Huang, Hongyu Li, Zihan Ding, Si Liu, Meng Wang, Zhedong Zheng (마카오대, 베이항대, 허페이공대) / arXiv 2026-01 (v2 2026-04)
- **문제**: 사람이 쓴 명령 없이 로봇이 소리 이벤트(이중 음원 포함)를 듣고 음원 물체를 찾아 조작하는 과제
- **방법**: RIR 기반 음향 렌더링 시뮬레이터 Habitat-Echo와 베이스라인. v1 과제명 SonicStow / Bi-Sonic Manipulation, v2에서는 벤치마크 STMM-1.9K(단일·다중 이벤트)로 명명
- **데이터셋/벤치마크**: Habitat-Echo, STMM-1.9K (공개 여부·라이선스 미확인, 논문 자체는 CC BY 4.0)
- **결과**: 전반적으로 성공률 낮음 — 3차 요약 기준 Oracle 1차 음원 4.23%/2차 0.56%, 이중 음원 과제 계획 정확도 최고 51.83%(Qwen3-Omni-30B). 원문 미확인
- **Physical AI 시사점**: 음성 명령을 넘어 환경음 트리거 기반 이동 조작으로 과제 확장, 겹친 음원 분리가 핵심 병목
- **링크**: https://arxiv.org/abs/2601.21667 , https://arxiv.org/html/2601.21667v2
