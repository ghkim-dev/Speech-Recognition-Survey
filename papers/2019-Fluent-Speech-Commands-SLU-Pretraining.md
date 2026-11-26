# Speech Model Pre-training for End-to-End Spoken Language Understanding
- **저자**: Loren Lugosch, Mirco Ravanelli, Patrick Ignoto, Vikrant Singh Tomar, Yoshua Bengio / Interspeech 2019
- **문제**: 음성 → 텍스트 → 의도 파이프라인 없이 음성에서 의도를 바로 예측할 때 학습 데이터가 부족함
- **방법**: ASR 목표(음소·단어)로 하위 층을 사전학습한 뒤 의도 분류로 미세조정
- **데이터셋**: [Fluent Speech Commands](../datasets/Fluent-Speech-Commands.md) (이 논문에서 공개)
- **Physical AI 시사점**: 로봇·스마트홈 명령을 텍스트 변환 없이 바로 행동 의도로 연결하는 초기 기준선
- **링크**: https://arxiv.org/abs/1904.03670
