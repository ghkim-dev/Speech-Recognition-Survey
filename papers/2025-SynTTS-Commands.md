# SynTTS-Commands: A Public Dataset for On-Device KWS via TTS-Synthesized Multilingual Speech
- **저자**: Lu Gan, Xi Li / arXiv 2511.07821 (2025-11 제출, v2 2025-11-24), 게재 학회 미확인(README상 이중 맹검 심사 중)
- **문제**: TinyML·엣지 KWS는 명령어마다 수천 명 규모 실녹음이 필요해 새 명령·새 언어 추가 비용이 큼
- **방법**: CosyVoice 2 TTS에 VoxCeleb·Free ST 화자 음색을 프롬프트로 넣어 영어 23·중국어 25개 미디어 제어 명령을 대량 합성(38만여 샘플, 111시간). 4.2K~4.7M 파라미터의 6개 KWS 모델로 벤치마크하고, 실녹음 테스트셋으로 sim-to-real 평가
- **데이터셋**: [SynTTS-Commands](../datasets/SynTTS-Commands.md), 실녹음 평가에 Google Speech Commands(영어)·MobvoiHotwords(중국어)
- **결과**: 합성 테스트 영어 최고 99.50%(CRNN, MobileNet-V1), 중국어 97.93%. 실녹음 GSC에서 BCResNet zero-shot 88.0% → 실녹음 50개 추가 93.0%. MobvoiHotwords는 zero-shot 재현율 0.44로 낮다가 50-shot에서 0.96 (GitHub README 수치)
- **Physical AI 시사점**: 로봇·차량·가전에 맞춤 명령어를 붙일 때 "합성으로 대량 사전학습 + 실녹음 수십 개 적응"이 현실적인 비용 구조임을 보여줌. 다만 원거리·잡음·잔향 조건 평가는 없어 실제 로봇 마이크 환경 성능은 별도 검증 필요
- **링크**: https://arxiv.org/abs/2511.07821 , https://github.com/lugan113/SynTTS-Commands-Official
