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
| CHiME-3/4 | 영어 | 학습 약 20시간(실 1,600+시뮬 7,138 문장), dev/test 각 1,640/1,320 문장 | 태블릿 6채널, 버스·카페·거리·보행구역 (CHiME-4는 6/2/1채널 트랙) | 모바일 다채널 잡음 ASR | 미확인(WSJ0 기반) | 미확인 | ASRU 2015, CSL 2017 | [상세](datasets/CHiME-3-4.md) |
| VoiceBank+DEMAND | 영어 | 학습 11,572 발화/28 화자(2차 자료) | VCTK+DEMAND 잡음 병렬 48kHz | 음성 향상 전처리 | 구 레코드 CC BY 4.0, 현행 미확인 | 공개 (Edinburgh) | 미확인 | [상세](datasets/VoiceBank-DEMAND.md) |
| DEMAND | 비음성(잡음) | 미확인 (16채널, 6개 환경 범주) | 16마이크 어레이 실환경 잡음 | 잡음 강건 ASR·음성 향상 잡음원 | CC BY-SA 3.0 (Zenodo 원본) | 공개 (Zenodo) | Thiemann 외 2013 | [상세](datasets/DEMAND.md) |
| OmniAction | 영어 추정 | 140k 에피소드, 5k+ 화자 | 맥락적 음성 지시 로봇 조작 | 음성-VLA | 미확인 | 공개 (HF) | RoboOmni (ICLR 2026) | [상세](datasets/OmniAction.md) |
| MIVIA Speech Command | 미확인 | 미확인 | 로봇 마이크+산업 잡음 증강 | 로봇 음성 명령 | 미확인 | 공개 (Zenodo) | 미확인 | [상세](datasets/MIVIA-Speech-Command.md) |
| VoCub | 영어 | 103 명령/29화자 | iCub 명령 | 휴머노이드 명령 인식 | 미확인 | 공개 | 미확인 | [상세](datasets/VoCub.md) |
| SLURP | 영어 | 실녹음 약 72K + 합성 약 69K 발화, 18 시나리오 | 홈 로봇 비서 명령, 177 화자 | 홈 로봇 음성 명령 SLU | 텍스트 CC BY 4.0 / 오디오 CC BY-NC 4.0 | 공개 (GitHub+Zenodo) | EMNLP 2020 | [상세](datasets/SLURP.md) |
| Fluent Speech Commands | 영어 | 30,043 발화/97 화자, 약 19시간 | 스마트홈 제어 명령, 16kHz 근접 | 엣지 E2E 의도 인식 | 학술 연구 전용(미확인) | 신청 | Interspeech 2019 | [상세](datasets/Fluent-Speech-Commands.md) |
| OpenX-Sound | 비해당(오디오) | 미확인 | OXE 궤적+동기화 오디오 | 음향 큐 기반 VSLA 학습 | 미확인 | 공개 (HF) | HEAR (IJRR 2026) | [상세](datasets/OpenX-Sound.md) |
| STOP | 영어 | 236,477 오디오, 약 218시간, 885 화자 | TOPv2 질의 낭독, 계층형 의도·슬롯 파스 | 복합 음성 명령 구조적 SLU | 미확인 (LICENSE 링크 접속 불가) | 공개 (Meta) | IEEE SLT 2022 | [상세](datasets/STOP.md) |
| Timers and Such | 영어 | 실+합성, 약 12.9GB (발화 수 미확인) | 숫자 명령 4개 의도(타이머·알람·계산·단위) | 엣지 음성 비서 숫자 명령 | CC0 (논문 기준) | 공개 (Zenodo) | NeurIPS 2021 D&B | [상세](datasets/Timers-and-Such.md) |
| EasyCom | 영어 | 약 5시간 18분(오류 포함 6.6시간), 세션 12개 | AR 안경 6채널+1인칭 영상, 레스토랑 잡음, 머리 자세 | 착용형·머리 장착 이동 어레이 음성 향상/ASR | CC BY-NC 4.0 | 공개 (GitHub) | arXiv 2021 | [상세](datasets/EasyCom.md) |
| SpokenWOZ | 영어 | 5.7k 대화, 203k 턴, 약 249시간, 8 도메인 | 전화 통화 사람 간 과업 지향 대화 | 다중 턴 음성 대화 로봇·비서 | CC BY-NC 4.0 | 공개 (test 비공개) | NeurIPS 2023 D&B | [상세](datasets/SpokenWOZ.md) |

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
| An analysis of environment, microphone and data simulation mismatches in robust speech recognition | Vincent, Watanabe 외 | CSL 2017 | CHiME-3/4 | 불일치가 강건 ASR에 미치는 영향 분석 | [요약](papers/2017-CHiME-4-Mismatch-Analysis.md) |
| DEMAND database | Thiemann, Ito, Vincent | ICA 2013 | DEMAND | 다양한 환경 다채널 잡음 DB | [요약](papers/2013-DEMAND.md) |
| RoboOmni | 미확인 | arXiv 2025 | OmniAction | 맥락적 음성 지시 omni-modal 로봇 | [요약](papers/2025-RoboOmni.md) |
| HEAR (Vision-Sound-Language-Action) | Nie, Deng, Wang 외 | IJRR 2026 (arXiv) | OpenX-Sound, HEAR-Bench | 스트리밍 오디오 메모리로 Blind Execution Interval 해소 | [요약](papers/2026-HEAR.md) |
| From Instruction to Event: Sound-Triggered Mobile Manipulation | Ju, Huang 외 | arXiv 2026 | Habitat-Echo, STMM-1.9K | 소리 이벤트 트리거 이동 조작 | [요약](papers/2026-Sound-Triggered-Mobile-Manipulation.md) |
| SLURP: A Spoken Language Understanding Resource Package | Bastianelli, Vanzo, Swietojanski, Rieser | EMNLP 2020 | SLURP | 홈 로봇 비서 18도메인 SLU 벤치마크, SLU-F1 | [요약](papers/2020-SLURP.md) |
| Speech Model Pre-training for End-to-End SLU | Lugosch, Ravanelli 외 | Interspeech 2019 | Fluent Speech Commands | 음소·단어 사전학습 E2E 의도 인식 | [요약](papers/2019-Fluent-Speech-Commands-E2E-SLU.md) |
| Speech enhancement for noise-robust TTS using deep RNNs | Valentini-Botinhao 외 | Interspeech 2016 | VoiceBank-DEMAND(미확인) | RNN 기반 향상 음성으로 TTS 학습 | [요약](papers/2016-VoiceBank-DEMAND-Valentini.md) |
| STOP: A Dataset for Spoken Task Oriented Semantic Parsing | Tomasello 외 (Meta AI) | IEEE SLT 2022 | STOP | 218시간 계층형 SLU 음성 벤치마크, exact match | [요약](papers/2022-STOP.md) |
| Timers and Such: A Practical Benchmark for SLU with Numbers | Lugosch 외 | NeurIPS 2021 D&B | Timers and Such | 숫자 명령 SLU, Direct E2E가 cascade 대비 우위 | [요약](papers/2021-Timers-and-Such.md) |
| EasyCom: An Augmented Reality Dataset to Support Algorithms for Easy Communication in Noisy Environments | Donley, Tourbabin 외 | arXiv 2021 | EasyCom | AR 안경 1인칭 다채널 대화 데이터, 대상 화자 향상 벤치마크 | [요약](papers/2021-EasyCom.md) |
| SpokenWOZ | Si 외 | NeurIPS 2023 D&B | SpokenWOZ | 249시간 음성 과업 대화, cross-turn·reasoning 슬롯, JGA 25.65% | [요약](papers/2023-SpokenWOZ.md) |

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
- [2026-11-11](daily/2026-11-11.md)
- [2026-11-12](daily/2026-11-12.md)
- [2026-11-13](daily/2026-11-13.md)
