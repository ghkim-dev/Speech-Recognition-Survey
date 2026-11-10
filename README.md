# Speech-Recognition-Survey

Physical AI(로봇, 체화 에이전트, 휴머노이드, 자율주행·차량, 스마트/엣지 디바이스)에서 활용 가능한 음성인식(ASR, KWS, 원거리·다채널, 잡음·잔향, 음성 명령 로봇 제어, 음성-언어-행동 모델)용 **공개 데이터셋**과 **관련 논문**을 매일 조사해 정리합니다.

## 조사 기준
1. 연구 목적 이용 가능 여부 우선 확인(상업적 이용은 참고). 라이선스와 접근 방식(공개/신청/LDC 유료) 명시
2. 영어 데이터셋 우선, IEEE 계열(ICASSP, ASRU, SLT, TASLP, ICRA, IROS, RA-L) 우선. Interspeech·CoRL·arXiv는 보조
3. 데이터셋과 대표 논문 연결
4. 확인하지 못한 수치·라이선스는 "미확인"으로 표기하고 출처 URL 기재

## 데이터셋 요약
| 이름 | 언어 | 규모 | 녹음 환경/특징 | Physical AI 활용 포인트 | 라이선스·연구 이용 | 접근 방식 | 주요 사용 논문/학회 | 링크 |
|---|---|---|---|---|---|---|---|---|
| CHiME-6 | 영어 | 20 세션 (학습/검증/평가 약 34/2/5시간) | 가정 저녁 식사, Kinect 6대 | 가정 내 다화자 원거리 | 비상업 연구 라이선스(CC BY-SA 여부 미확인) | 신청 | CHiME-6 Challenge (arXiv) | [상세](datasets/CHiME-6.md) |
| LibriCSS | 영어 | 미확인 | LibriSpeech 재녹음, 겹침 비율 다양 | 연속 음성 분리 | 미확인 | 공개 (GitHub) | ICASSP 2020 | [상세](datasets/LibriCSS.md) |
| Speech Commands | 영어 | 미확인 (35 클래스, 2차 자료) | 1초 단어, 크라우드소싱 | 엣지 KWS | CC BY 4.0 | 공개 | Warden 2018 (arXiv) | [상세](datasets/Speech-Commands.md) |
| VOiCES | 영어 | 미확인 | 실제 방 재생·재녹음, 잡음 동시 재생 | 원거리·잡음·잔향 | CC BY 4.0 | 공개 | VOiCES Challenge 2019 (Interspeech) | [상세](datasets/VOiCES.md) |
| REVERB | 영어 | 미확인 | 시뮬레이션+실녹음(MC-WSJ-AV) | 잔향 강건 ASR | LDC 챌린지 라이선스(일반 조건 미확인) | LDC | EURASIP JASP 2016 | [상세](datasets/REVERB.md) |
| DiPCo | 영어 | 10 세션(15~45분) | 식탁 대화, 7마이크 어레이 5대 | 스마트 스피커·가정 로봇 | CDLA-Permissive(미러 기준, 미확인) | 공개 (Zenodo) | arXiv 2019 | [상세](datasets/DiPCo.md) |
| DIRHA-English | 영어 | LDC2018S01 약 85시간 | 다실 아파트, 다수 마이크 | 홈 음성 상호작용 | LDC 조건 미확인 | LDC | ASRU 2015 | [상세](datasets/DIRHA-English.md) |
| AMI | 영어 | 약 100시간 | 회의, 근접+원거리 마이크 | 다화자 회의·diarization | CC BY 4.0 | 공개 | Carletta et al. 2005 | [상세](datasets/AMI.md) |
| MChRSR | 영어 | 미확인 | PR2 이동 중 다채널 녹음 | 로봇 ego-noise ASR | 미확인 | 미확인 | 2017 | [상세](datasets/MChRSR.md) |
| CHiME-3/4 | 영어 | 미확인 | 6채널 태블릿, 카페·거리·버스·보행구역 | 모바일 다채널 잡음 ASR | 미확인(WSJ0 기반) | 미확인 | ASRU 2015 | [상세](datasets/CHiME-3-4.md) |
| CHiME-4 | 영어 | 학습 약 20시간(실+시뮬), dev/test 각 1,640/1,320 문장 | 태블릿 6채널, 버스·카페·거리 | 모바일 다채널 잡음 ASR | 미확인 | 미확인 | CHiME-4 Challenge | [상세](datasets/CHiME-4.md) |
| VoiceBank+DEMAND | 영어 | 학습 11,572 발화/28 화자(2차 자료) | VCTK+DEMAND 잡음 병렬 48kHz | 음성 향상 전처리 | 구 레코드 CC BY 4.0, 현행 미확인 | 공개 (Edinburgh) | 미확인 | [상세](datasets/VoiceBank-DEMAND.md) |
| DEMAND | 비음성(잡음) | 미확인 (16채널, 6개 환경 범주) | 16마이크 어레이 실환경 잡음 | 잡음 강건 ASR·음성 향상 잡음원 | CC BY-SA 3.0 (Zenodo 원본) | 공개 (Zenodo) | Thiemann 외 2013 | [상세](datasets/DEMAND.md) |
| OmniAction | 영어 추정 | 140k 에피소드, 5k+ 화자 | 맥락적 음성 지시 로봇 조작 | 음성-VLA | 미확인 | 공개 (HF) | RoboOmni (ICLR 2026) | [상세](datasets/OmniAction.md) |
| MIVIA Speech Command | 미확인 | 미확인 | 로봇 마이크+산업 잡음 증강 | 로봇 음성 명령 | 미확인 | 공개 (Zenodo) | 미확인 | [상세](datasets/MIVIA-Speech-Command.md) |
| VoCub | 영어 | 103 명령/29화자 | iCub 명령 | 휴머노이드 명령 인식 | 미확인 | 공개 | 미확인 | [상세](datasets/VoCub.md) |

## 논문 요약
| 제목 | 저자 | 학회/연도 | 사용 데이터셋 | 핵심 내용 | 링크 |
|---|---|---|---|---|---|
| CHiME-6 Challenge | Watanabe 외 | arXiv 2020 | CHiME-6 | 비분할 다화자 인식 챌린지 | [요약](papers/2020-CHiME-6-Challenge.md) |
| Continuous Speech Separation: Dataset and Analysis | Chen, Yoshioka 외 | ICASSP 2020 | LibriCSS | 연속 음성 분리 평가 | [요약](papers/2020-LibriCSS-Continuous-Speech-Separation.md) |
| The VOiCES from a Distance Challenge 2019 Evaluation Plan | Nandwana 외 | arXiv 2019 | VOiCES | 원거리 화자·ASR 챌린지 | [요약](papers/2019-VOiCES-Challenge-Evaluation-Plan.md) |
| A summary of the REVERB challenge | Kinoshita 외 | EURASIP JASP 2016 | REVERB | 잔향 SE/ASR 결과 정리 | [요약](papers/2016-REVERB-Challenge-Summary.md) |
| VLAS | Zhao, Ding 외 | ICLR 2025 | CALVIN, SQA, CSI | 음성 직접 입력 VLA | [요약](papers/2025-VLAS.md) |
| DiPCo – Dinner Party Corpus | Amazon | arXiv 2019 | DiPCo | 원거리 대화 코퍼스 | [요약](papers/2019-DiPCo.md) |
| The DIRHA-English corpus | Ravanelli 외 | ASRU 2015 | DIRHA-English | 가정 원거리 인식 | [요약](papers/2015-DIRHA-English.md) |
| Single-Channel Robot Ego-Speech Filtering | Li, Hindriks, Kunneman | arXiv 2024 | 자체(Pepper) | 로봇 자기 발화 제거 | [요약](papers/2024-Pepper-Ego-Speech-Filtering.md) |
| MChRSR | 미확인 | 2017 | MChRSR | 로봇 이동 잡음 ASR | [요약](papers/2017-MChRSR.md) |
| The third CHiME Challenge | Barker 외 | ASRU 2015 | CHiME-3/4 | 태블릿 다채널 잡음 ASR 챌린지 | [요약](papers/2015-CHiME-3-Challenge.md) |
| An analysis of environment, microphone and data simulation mismatches in robust speech recognition | 미확인 | CSL 2017 | CHiME-4 | 불일치가 강건 ASR에 미치는 영향 분석 | [요약](papers/2017-CHiME-4-Mismatch-Analysis.md) |
| DEMAND database | Thiemann, Ito, Vincent | ICA 2013 | DEMAND | 다양한 환경 다채널 잡음 DB | [요약](papers/2013-DEMAND.md) |
| RoboOmni | 미확인 | arXiv 2025 | OmniAction | 맥락적 음성 지시 omni-modal 로봇 | [요약](papers/2025-RoboOmni.md) |
| HEAR | 미확인 | arXiv 2026 | 미확인 | 스트리밍 오디오 sound-centric 조작, Blind Execution Interval | [요약](papers/2026-HEAR.md) |
| From Instruction to Event: Sound-Triggered Mobile Manipulation | 미확인 | arXiv 2026 | 미확인 | 소리 이벤트 트리거 이동 조작 | [요약](papers/2026-Sound-Triggered-Mobile-Manipulation.md) |
| Speech enhancement for noise-robust TTS using deep RNNs | Valentini-Botinhao 외 | Interspeech 2016 | VoiceBank-DEMAND(미확인) | RNN 기반 향상 음성으로 TTS 학습 | [요약](papers/2016-VoiceBank-DEMAND-Valentini.md) |

## Daily 로그
- [2026-10-29](daily/2026-10-29.md)
- [2026-10-30](daily/2026-10-30.md)
- [2026-10-31](daily/2026-10-31.md)
- [2026-11-01](daily/2026-11-01.md)
- [2026-11-02](daily/2026-11-02.md)
- [2026-11-03](daily/2026-11-03.md)
- [2026-11-04](daily/2026-11-04.md)
- [2026-11-05](daily/2026-11-05.md)
- [2026-11-06](daily/2026-11-06.md)
- [2026-11-07](daily/2026-11-07.md)
- [2026-11-08](daily/2026-11-08.md)
- [2026-11-09](daily/2026-11-09.md)
- [2026-11-10](daily/2026-11-10.md)
