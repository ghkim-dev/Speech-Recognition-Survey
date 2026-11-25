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
| SPEAR | 영어 | D1~D4, Core Train 압축 78 GB, 세션 15개 (총 시간 미확인) | EasyCom 실녹음(D1)+TASCAR 시뮬레이션(D2~D4) | 머리 장착 이동 어레이 향상, sim-to-real 비교 | 미확인(원본 EasyCom은 CC BY-NC 4.0) | 공개 (Eval은 요청) | IWAENC 2022 | [상세](datasets/SPEAR.md) |
| MMCSG | 영어 | 530 녹음, 약 26.3시간 | Aria 안경 7채널(48kHz)+IMU+영상, 양자 대화 | 착용형 스트리밍 다화자 ASR, 자기/상대 발화 구분 | Meta Data License(연구용, 세부 미확인) | 신청 | CHiME-8 (2024) | [상세](datasets/MMCSG.md) |
| NOTSOFAR-1 | 영어 | 실회의 237개(평균 6분, 회의실 30곳, 화자 35명) + 시뮬레이션 약 1,000시간 | 회의실 탁자 위 단일 장치(단일/다채널), 조건 해시태그 | 고정 단일 기기 원거리 다화자 화자 귀속 전사 | CC BY 4.0 (Dev-set-2 제외) | 공개 (HF) | Interspeech 2024 | [상세](datasets/NOTSOFAR-1.md) |
| CAVEMOVE | 비해당(임펄스 응답·잡음) | Zenodo 약 7.6 GB, 차량 3~4대(출처 불일치) | 승용차 실내, 8마이크 원형 어레이+분산 마이크, 속도·창문 조건별 주행 잡음, 16kHz | 자율주행·차량 음성 비서 데이터 합성 | 데이터 미확인(API 코드 MIT) | 공개 (Zenodo) | arXiv 2025 | [상세](datasets/CAVEMOVE.md) |
| CHiME-7/8 DASR | 영어 | 기존 코퍼스 3~4개 통합(CHiME-6·DiPCo·Mixer 6 + CHiME-8은 NOTSOFAR-1), 총 시간 미확인 | 시나리오마다 장치 수·배열 구조 상이, 배열 무관 단일 시스템 평가 | 다양한 실내 환경·기기 배치로의 원거리 다화자 인식 일반화 | 구성 코퍼스별(CC BY 4.0~LDC 유료) | 혼합 (chime-utils 자동 다운로드 + Mixer 6은 LDC) | CHiME 2023/2024 Workshop | [상세](datasets/CHiME-7-8-DASR.md) |
| Mixer 6 Speech | 영어 | 화자 594명, LDC2013S03 약 15,863시간(다채널 합산), CHiME-8 전사 서브셋 음성 약 80시간 | LDC 녹음실 인터뷰·낭독·통화, 13개 마이크 동시 녹음 | 마이크 위치·종류 변화에 따른 원거리 인식 | LDC 회원 전용(서브셋 LDC2025S07은 비회원 계약) | LDC | CHiME-7/8 DASR | [상세](datasets/Mixer-6.md) |
| CHiME-9 ECHI | 영어 | 49세션·196화자(세션당 30분+), train 18시간/dev 약 6시간/eval 약 5.4시간 | 카페테리아 잡음 4인 대화, Aria 안경 7채널+보청기 4채널, 머리 추적·근접 기준 신호 | 착용형·로봇의 저지연 대상 화자 추출 전처리 | DUA 서명 후 학술·벤치마크 용도 | 신청 (HF gated) | CHiME-9 (arXiv 2609.26306) | [상세](datasets/CHiME-9-ECHI.md) |
| Aria Everyday Activities | 영어 추정 | 녹화 143개, 7.5시간+, 실내 5곳 | Aria 1인칭 7채널 오디오+RGB/SLAM·시선·3D 궤적, ASR 전사 | 공간 인식 체화 에이전트 음성(누가 어디서 말했나) | Meta AEA 라이선스(재배포 금지, 상업 별도 문의) | 공개 (동의 후 다운로드) | arXiv 2402.13349 | [상세](datasets/Aria-Everyday-Activities.md) |
| AVICAR | 영어 | 화자 100명(86명 표기 불일치), 약 59,000 발화 | 주행 차량, 선바이저 8마이크 어레이+카메라 4대, 주행 조건 5종 | 차량 내 다채널 시청각 ASR | 미확인 | 요청 (추정) | Interspeech 2004 | [상세](datasets/AVICAR.md) |
| CHiME-9 MCoRec | 영어 | 150세션(train 5.6/dev 2.5/eval 6.9시간), 세션당 최대 8화자·4개 동시 대화 | 방 중앙 360° 카메라 영상+내장 마이크 1채널, 겹침 최대 100%, 학습셋만 라펠 근접 음성 | 로봇의 시청각 ASR과 대화 그룹(누가 누구와) 파악 | CHiME 연구 목적(상업은 저자 문의, 원문 미확인) | 신청 (HF gated) | CHiME-9 (arXiv 2510.23276) | [상세](datasets/CHiME-9-MCoRec.md) |
| Ego4D AVD / Talking-to-Me | 영어 위주(구성 미확인) | AVD 주석 약 50시간(5분 클립 572개), 클립당 화자 4.71명 | 1인칭 착용 카메라 일상 대화, 위치·능동 화자·분할·전사 4과제 + 청자 판단(TTM) | 로봇 1인칭 화자 분할·전사, "나에게 하는 말인가" 판단 | Ego4D 라이선스(비상업 여부 자료 상충, 미확인) | 신청 (라이선스 동의 후 CLI) | CVPR 2022 | [상세](datasets/Ego4D-AVD.md) |
| Ego-Exo4D (오디오·음성 자원) | 영어 위주(구성 미확인) | V2 테이크 5,035개·영상 1,286시간(1인칭 221시간), take_audio 약 1,057 GB, 전문가 해설 녹음 117,812개 | 숙련 활동(요리·수리·스포츠) 중 Aria 7채널 1인칭 음성, Narrate & Act 자기 설명, 전문가 음성 해설, Whisper 자동 전사 | 작업 잡음 속 음성 지시와 3D 손·몸 동작 정렬, 음성 피드백 학습 | Ego-Exo4D 라이선스(무료, 상업 범위 원문 미확인) | 신청 (lab22.ai 동의 후 CLI) | CVPR 2024 | [상세](datasets/Ego-Exo4D-Audio.md) |
| NatSGLD | 영어 | 명령 1,143개·참가자 18명, 활동 11종 | WoZ 시뮬레이션 로봇(Baxter) 주방 과제, 자연 음성+제스처, 44kHz 오디오 포함 영상, LTL 정답·시연 궤적 | 음성+제스처 로봇 명령의 형식적 과제 해석(LTL) | MIT | 공개 (GitHub+프로젝트 사이트) | ACM/IEEE HRI 2025 | [상세](datasets/NatSGLD.md) |
| NatSGD | 영어 | 명령 1,143개·참가자 18명(NatSGLD와 동일 명령) | WoZ 시뮬레이션 주방 로봇, 자연 음성+제스처, 전문가 시연 궤적 | 음성+제스처 조건 모방학습, 명령→LTL(Comm2LTL) | 코드 MIT, 데이터 미확인 | 공개 (프로젝트 사이트) | arXiv 2024 | [상세](datasets/NatSGD.md) |
| AISHELL-5 (비영어 보조) | 중국어 | 100시간+ (train 94.75h/568세션, dev·eval1·eval2 각 약 3.3~3.6h) + 차량 잡음 40시간 | 전기차 실주행 60+ 조건(속도·창문·에어컨·음악), 원거리 4채널+근접 헤드셋+AEC 참조 2채널 | 차량 음성 비서의 겹침 발화 분할·인식, AEC·분리 프런트엔드 | CC BY-SA 4.0 (코드 Apache 2.0) | 공개 (OpenSLR 159) | Interspeech 2025 | [상세](datasets/AISHELL-5.md) |
| SynTTS-Commands | 영어+중국어 | 384,621개·111.33시간(영어 23클래스 183,076개·46.5시간) | CosyVoice 2 TTS 합성, VoxCeleb·Free ST 화자 음색 복제, 미디어 제어·웨이크워드 명령 | 엣지·차량·로봇 KWS의 합성 사전학습+소량 실녹음 적응 | 코드 MIT, 데이터 미확인 | 공개 (Hugging Face) | arXiv 2025 | [상세](datasets/SynTTS-Commands.md) |
| Hey Snips | 영어 | 웨이크워드 약 11K + 음성 약 86.5K(약 96시간), 2.2K+ 화자 | 크라우드소싱 근접 녹음, 음성 샘플도 같은 화자·기기에서 수집(원거리 아님) | 스마트 기기·로봇 상시 청취 웨이크워드, FRR @ 0.5 FA/h 평가 | 비상업 연구 전용, 수정본 재배포 금지 | 신청 (Google Form) | IEEE ICASSP 2019 | [상세](datasets/Hey-Snips.md) |
| LOCATA | 영어 (VCTK 문장) | 6개 과제 개발·평가 셋, 총 시간 미확인 | 음향실, NAO 로봇 머리 12ch·Eigenmike 32ch·DICIT 평면·바이노럴 보청기 동시 녹음, 이동 화자·이동 어레이, OptiTrack 정답 궤적 | 로봇 머리 화자 위치 추정·추적, 빔포밍 조향(원거리 ASR 앞단) | Open Data Commons(세부 종류 미확인) | 공개 (Zenodo) | IEEE/ACM TASLP 2020, IEEE SAM 2018 | [상세](datasets/LOCATA.md) |
| DREGON | 영어 (TIMIT 음성 재생) | 총 시간 미확인 (정지·ego-noise 단독·비행 중 음원 녹음) | MikroKopter 쿼드로터 정육면체 8ch 어레이 44.1 kHz, 실내(RT<150 ms), Vicon 정답+로터 속도+IMU | 드론·로봇 ego-noise 하 음원 위치 추정, 로봇 상태 조건화 잡음 제거 | 학술·교육 무료(라이선스명 미확인) | 공개 (dregon.inria.fr) | IEEE/RSJ IROS 2018, IEEE SP Cup 2019 | [상세](datasets/DREGON.md) |
| DroneAudioSet | 음성 포함(HV 범주, 언어 비율 미확인) | 23.5시간 (42.6 GB), 216개 설정 | 프레임 고정 드론 2종 실제 회전+스피커 음원 동시 녹음, 방 3개, 위/아래 8ch 어레이+단일 마이크, SNR 약 -57~-3 dB | 드론·로봇 ego-noise 하 사람 존재 감지(음성/비음성/비인간), 잡음 억제·마이크 배치 비교 | MIT(HF, 검색 결과 기준) | 공개 (Hugging Face) | NeurIPS 2025 D&B | [상세](datasets/DroneAudioSet.md) |

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
| An Introduction to the Speech Enhancement for Augmented Reality (SPEAR) Challenge | Guiraud, Hafezi, Naylor 외 | IWAENC 2022 | SPEAR, EasyCom | EasyCom 시뮬레이션 확장 IEEE SPS 챌린지, MVDR 베이스라인 | [요약](papers/2022-SPEAR-Challenge.md) |
| The CHiME-8 MMCSG Challenge | Žmolíková 외 | CHiME 2024 Workshop | MMCSG | 스마트 안경 스트리밍 다화자 ASR, WER+지연 평가 | [요약](papers/2024-CHiME-8-MMCSG.md) |
| NOTSOFAR-1 Challenge: New Datasets, Baseline, and Tasks for Distant Meeting Transcription | Vinnikov, Ivry 외 (Microsoft) | Interspeech 2024 | NOTSOFAR-1 | 단일 기기 원거리 회의 화자 귀속 전사, tcpWER SC 46.8/MC 32.4% 베이스라인 | [요약](papers/2024-NOTSOFAR-1-Challenge.md) |
| CAVEMOVE: An Acoustic Database for the Study of Voice-enabled Technologies inside Moving Vehicles | Stefanakis, Symiakakis 외 (FORTH) | arXiv 2025 | CAVEMOVE | 차량 실측 임펄스 응답·주행 잡음 DB와 합성 API | [요약](papers/2025-CAVEMOVE.md) |
| The CHiME-7 DASR Challenge: Distant Meeting Transcription with Multiple Devices in Diverse Scenarios | Cornell 외 | CHiME 2023 Workshop (arXiv 2306.13734) | CHiME-6, DiPCo, Mixer 6 | 배열 무관 원거리 화자 분할+ASR, 베이스라인 main eval macro DA-WER 55.3% | [요약](papers/2023-CHiME-7-DASR-Challenge.md) |
| The CHiME-8 DASR Challenge for Generalizable and Array Agnostic Distant ASR and Diarization | Cornell 외 | CHiME 2024 Workshop (arXiv 2407.16447) | CHiME-6, DiPCo, Mixer 6, NOTSOFAR-1 | 4개 시나리오 tcpWER, 최고 eval macro 19.6%(STCON, 2차 자료) | [요약](papers/2024-CHiME-8-DASR-Challenge.md) |
| CHiME-9 ECHI: A Machine Learning Challenge for Enhancing Conversations to Address Hearing Impairment | Sutherland, Goetze, Barker 외 | arXiv 2026 (CHiME-9) | CHiME-9 ECHI | 보청기·Aria 저지연 대상 화자 추출, 인과적 TF-GridNet 베이스라인, 객관 지표와 청취 평가 괴리 | [요약](papers/2026-CHiME-9-ECHI.md) |
| Aria Everyday Activities Dataset | Lv, Charron, Moulon 외 (Meta) | arXiv 2024 | Aria Everyday Activities | 1인칭 다중 센서+3D 공간 정보+음성 전사 공개 | [요약](papers/2024-Aria-Everyday-Activities.md) |
| AVICAR: Audio-Visual Speech Corpus in a Car Environment | Lee, Hasegawa-Johnson 외 | Interspeech 2004 | AVICAR | 차량 내 8마이크+카메라 4대 시청각 코퍼스 | [요약](papers/2004-AVICAR.md) |
| A Cocktail-Party Benchmark: Multi-Modal dataset and Comparative Evaluation Results | Nguyen 외 (KIT, CMU, Meta AI) | arXiv 2025 (CHiME-9) | CHiME-9 MCoRec | 동시 다중 대화 시청각 전사+대화 클러스터링, 오디오만 WER>100%, 최고 Joint 0.3548 | [요약](papers/2025-MCoRec-Cocktail-Party-Benchmark.md) |
| Ego4D: Around the World in 3,000 Hours of Egocentric Video | Grauman 외 (Meta AI 컨소시엄) | CVPR 2022 | Ego4D AVD / Social | 1인칭 영상 3,670시간·AVD/TTM 벤치마크, 전사 WER 112→56(챌린지) | [요약](papers/2022-Ego4D.md) |
| Ego-Exo4D: Understanding Skilled Human Activity from First- and Third-Person Perspectives | Grauman 외 (Meta FAIR 컨소시엄) | CVPR 2024 | Ego-Exo4D | 1인칭+3인칭 숙련 활동, Aria 7채널 오디오·내레이션·전문가 음성 해설, ASR 벤치마크는 없음 | [요약](papers/2024-Ego-Exo4D.md) |
| NatSGLD: A Dataset with Speech, Gesture, Logic, and Demonstration for Robot Learning in Natural HRI | Shrestha, Zha 외 (UMD) | ACM/IEEE HRI 2025 | NatSGLD | WoZ 자연 음성·제스처 로봇 명령 + LTL 정답 + 시연, MIT 공개 | [요약](papers/2025-NatSGLD.md) |
| NatSGD: A Dataset with Speech, Gestures, and Demonstrations for Robot Learning in Natural HRI | Shrestha 외 (UMD) | arXiv 2024 | NatSGD | 음성+제스처 명령·시연, Comm2LTL Spot Score 음성만 0.434 → 결합 0.588(BART) | [요약](papers/2024-NatSGD.md) |
| AISHELL-5: The First Open-Source In-Car Multi-Channel Multi-Speaker Speech Dataset | Dai, Xie, Bu 외 (NWPU, AISHELL, Li Auto) | Interspeech 2025 | AISHELL-5 | 실차 다채널 다화자 공개, Eval1 CER 최저 16.65%, 분리 프런트엔드가 Eval2 cpCER 약 20포인트 좌우 | [요약](papers/2025-AISHELL-5.md) |
| ICMC-ASR: The ICASSP 2024 In-Car Multi-Channel Automatic Speech Recognition Challenge | Wang, Xie 외 | IEEE ICASSP 2024 GC | ICMC-ASR(=AISHELL-5 추정) | 실차 다화자 챌린지, 베이스라인 cpCER 72.88% → 1위 21.48%(GSS 채널 선택 개선+TS-VAD) | [요약](papers/2024-ICMC-ASR-Challenge.md) |
| SynTTS-Commands: A Public Dataset for On-Device KWS via TTS-Synthesized Multilingual Speech | Gan, Li | arXiv 2025 | SynTTS-Commands, GSC, MobvoiHotwords | TTS 합성 KWS, 실녹음 GSC zero-shot 88.0% → 50-shot 93.0% | [요약](papers/2025-SynTTS-Commands.md) |
| Efficient Keyword Spotting Using Dilated Convolutions and Gating | Coucke 외 (Snips) | IEEE ICASSP 2019 | Hey Snips | WaveNet식 dilated conv+gating 스트리밍 KWS, 0.5 FA/h에서 LSTM 대비 FRR 약 94%(잡음 86%) 감소 | [요약](papers/2019-Hey-Snips-Dilated-Conv-KWS.md) |
| Lend me an Ear: Speech Enhancement Using a Robotic Arm with a Microphone Array | Turcotte, Grondin | arXiv 2026 | 미확인(합성 혼합, -5~10 dB) | 7자유도 팔 16마이크 가변 어레이, 화자 위치→역기구학 재구성→DNN IRM+MVDR | [요약](papers/2026-Lend-me-an-Ear.md) |
| The LOCATA Challenge: Acoustic Source Localization and Tracking | Evers, Löllmann 외 | IEEE/ACM TASLP 2020 | LOCATA | 정지/이동 음원×정지/이동 어레이 6개 과제 실측 위치 추정·추적 벤치마크, MUSIC 베이스라인 | [요약](papers/2020-LOCATA-Challenge.md) |
| ODAS: Open embeddeD Audition System | Grondin, Michaud 외 (Sherbrooke) | Frontiers in Robotics and AI 2022 | 자체 실측 | C 기반 저전력 로봇 청각(SRP-PHAT-HSDA 위치 추정+M3K 추적+분리), Raspberry Pi 실시간, MIT·ROS | [요약](papers/2022-ODAS.md) |
| DREGON: Dataset and Methods for UAV-Embedded Sound Source Localization | Strauss, Mordel, Miguet, Deleforge | IEEE/RSJ IROS 2018 | DREGON | 드론 탑재 8ch 어레이 ego-noise 데이터+GCC-PHAT/MUSIC 베이스라인, 비행 중 음성 위치 추정 난제 | [요약](papers/2018-DREGON.md) |
| Development, Deployment and Applications of Robot Audition Open Source Software HARK | Nakadai, Okuno, Mizumoto | J. Robotics and Mechatronics 2017 (선행 IEEE Humanoids 2008) | 응용 사례 | 로봇 청각 오픈소스 미들웨어(위치 추정·분리·ASR 연동), HARK-Embedded/SaaS | [요약](papers/2017-HARK.md) |
| DroneAudioset: An Audio Dataset for Drone-based Search and Rescue | Gupta, Ramesh 외 (NUS) | NeurIPS 2025 D&B | DroneAudioSet | 드론 잡음+음원 실측 동시 녹음 23.5시간, MVDR/MP-SENet → SSLAM 사람 존재 3범주 분류 베이스라인 | [요약](papers/2025-DroneAudioSet.md) |
| Enhancing drone audition with rotor-conditioned deep models | Gulli, Fontana, Drioli, Salvati, Ferrin | EURASIP JASMP 2025 | DREGON | 로터 속도 시계열로 조건화한 음성 향상, 16개 구성 중 13개 최고, 25% 파라미터 경량 모델도 최고 근접 | [요약](papers/2025-Rotor-Conditioned-Drone-Audition.md) |

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
- [2026-11-14](daily/2026-11-14.md)
- [2026-11-15](daily/2026-11-15.md)
- [2026-11-16](daily/2026-11-16.md)
- [2026-11-17](daily/2026-11-17.md)
- [2026-11-18](daily/2026-11-18.md)
- [2026-11-19](daily/2026-11-19.md)
- [2026-11-20](daily/2026-11-20.md)
- [2026-11-21](daily/2026-11-21.md)
- [2026-11-22](daily/2026-11-22.md)
- [2026-11-23](daily/2026-11-23.md)
- [2026-11-24](daily/2026-11-24.md)
- [2026-11-25](daily/2026-11-25.md)
