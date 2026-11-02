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
| CHiME-4 | 영어 | 실녹음 약 3h + 시뮬 약 15h(학습) | 6마이크 태블릿, 버스·카페 등 | 이동 디바이스 다채널 ASR | 미확인 | 미확인 | Computer Speech & Language 2017 | [상세](datasets/CHiME-4.md) |
| VoiceBank-DEMAND | 영어 | 미확인 (30명) | 깨끗한 음성+DEMAND 잡음 시뮬 | 음성 향상 front-end | CC BY 4.0(2차 자료) | 공개 (DataShare) | SpeechBrain 등 | [상세](datasets/VoiceBank-DEMAND.md) |

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
| Environment, microphone and data simulation mismatches in robust ASR | Vincent 외 | CSL 2017 | CHiME-4 | 불일치 분석(세부 미확인) | [요약](papers/2017-CHiME-4-Mismatch-Analysis.md) |

## Daily 로그
- [2026-10-29](daily/2026-10-29.md)
- [2026-11-02](daily/2026-11-02.md)
