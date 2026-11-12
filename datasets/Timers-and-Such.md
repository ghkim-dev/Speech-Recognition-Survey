# Timers and Such
- **언어**: 영어
- **규모**: 실녹음 + 합성(TTS) 음성, 전체 zip 약 12.9GB(v0.1 Zenodo 기준). 총 발화 수·화자 수·시간은 미확인. split: train/dev/test × real/synth
- **녹음 환경**: 자원 화자가 문법 스크립트로 생성한 문장을 낭독(원격 크라우드 녹음, 기기 다양). 숫자가 들어간 명령에 특화
- **의도**: SetTimer, SetAlarm, SimpleMath, UnitConversion 4개 + 숫자 슬롯
- **Physical AI 활용 포인트**: 오프라인 엣지 음성 비서·로봇에서 숫자(시간·수량·단위)를 정확히 인식해야 하는 명령 평가. 합성 음성만으로 학습했을 때 실음성 일반화 확인
- **라이선스/연구 이용**: CC0 (논문 기준, 상업 이용 포함 제한 없음. Zenodo 메타데이터는 직접 확인 못 함)
- **접근 방식**: 공개 (Zenodo record 4623772, SpeechBrain 레시피 `recipes/timers-and-such`)
- **주요 사용 논문**: [Timers and Such (Lugosch 외, NeurIPS 2021 Datasets & Benchmarks)](../papers/2021-Timers-and-Such.md)
- **출처**: https://arxiv.org/abs/2104.01604 , https://zenodo.org/record/4623772 , https://github.com/speechbrain/speechbrain/tree/develop/recipes/timers-and-such
