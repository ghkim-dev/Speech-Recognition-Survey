# Ego4D Audio-Visual Diarization (AVD) / Social (Talking-to-Me)
- **언어**: 영어 위주 (AVD 전사 기준). Ego4D 전체는 9개국 931명 참여로 다국어 포함, AVD 클립의 언어 구성 비율은 미확인
- **규모**: Ego4D 전체 1인칭 영상 약 3,670시간. AVD는 대화 장면 750시간 이상 중 약 50시간(5분 클립 572개: train 389, val 50, 나머지 test)에 주석. 클립당 평균 화자 4.71명, 클립당 발화 시간 219.81초, 착용자 발화 77.64초 (EGO4D/audio-visual README)
- **녹음 환경**: 머리 장착 카메라(기기 다양)로 찍은 일상 대화. 영상에 내장된 오디오(단일 채널 16kHz로 추출해 사용). 4개 과제: 화자 위치 추정·추적(얼굴 bbox), 능동 화자 검출(보이지 않는 착용자 포함), 화자 분할(오디오 전용/시청각), 전사. Social 벤치마크의 Talking-to-Me(TTM)는 AVD 발화 주석 위에 "이 사람이 착용자에게 말하고 있는가" 라벨을 추가
- **Physical AI 활용 포인트**: 로봇 1인칭 시점에서 화자 검출·분할·전사, 그리고 "나에게 하는 말인가"(addressee detection) 판단. 로봇이 명령을 받을지 무시할지 정하는 단계와 직결
- **라이선스/연구 이용**: Ego4D 라이선스 동의 후 승인(약 48시간) → AWS 자격 증명 발급. 2차 자료들은 비상업 연구 전용(CC BY-NC 4.0 계열)으로 설명하나 일부 자료는 일정 상업 이용 허용으로 서술하여 상충 → 미확인. 공식 라이선스 원문 확인 필요
- **접근 방식**: 신청 (라이선스 동의 후 `ego4d` CLI로 다운로드, 주석 `av_train.json`/`av_val.json`)
- **베이스라인/결과(2차 자료)**: 전사 공식 베이스라인은 GigaSpeech 학습 ESPnet 모델에 oracle 분할 사용, 2022 test WER 112.10. 2022 우승(AVATAR) 68.40, 2023 우승(OxfordVGG, WhisperX) 56.0 — 텍스트 정규화만으로 73.3→56.0. 2022 AVD 최고 DER 65.9%(Intel Labs, 베이스라인 73.3%). TTM 최근 결과 mAP 67.39%(EgoAdapt, 2026)
- **주요 사용 논문**: [Ego4D: Around the World in 3,000 Hours of Egocentric Video](../papers/2022-Ego4D.md) (CVPR 2022)
- **출처**: https://raw.githubusercontent.com/EGO4D/audio-visual/main/README.md , https://raw.githubusercontent.com/EGO4D/audio-visual/main/transcription/README.md , https://github.com/EGO4D/social-interactions/tree/ttm , https://ego4d-data.org/docs/start-here/ , https://arxiv.org/abs/2211.09966 , https://arxiv.org/abs/2307.09006 , https://arxiv.org/abs/2210.07764
