# AISHELL-5: The First Open-Source In-Car Multi-Channel Multi-Speaker Speech Dataset for Automatic Speech Diarization and Recognition
- **저자**: Yuhang Dai, He Wang, Xingchen Li, Zihan Zhang, Shuiyuan Wang, Lei Xie, Xin Xu, Hongxiao Guo, Shaoji Zhang, Hui Bu 외 (NWPU ASLP, AISHELL, Li Auto) / Interspeech 2025 (arXiv 2505.23036)
- **문제**: 차량 내 음성 인식은 좁은 공간 잔향, 주행·바람·에어컨·음악 잡음, 운전자-동승자 겹침 발화가 동시에 존재하지만 공개된 실차 다채널 다화자 데이터가 없었음(이전 ICMC-ASR 챌린지 데이터는 공개 범위 제한)
- **방법**: 실제 전기차에서 60개 이상 주행 조건으로 원거리 4채널+근접 헤드셋 동시 녹음한 100시간+ 코퍼스와 40시간 차량 잡음을 공개. 베이스라인은 프런트엔드(AEC+IVA 또는 SpatialNet 분리) → VAD(pyannote/Silero) → WeNet ASR 구조, 두 트랙(Eval1: 정답 구간 ASR, Eval2: 화자 분할+ASR, cpCER)
- **데이터셋**: [AISHELL-5](../datasets/AISHELL-5.md)
- **결과**: Eval1 CER 자체 학습 E-Branchformer 26.05%, Paraformer(6만 시간) 미세조정 16.65%. 대규모 범용 모델도 그대로는 약함(Whisper-Small 50.69%, Qwen2-Audio 29.92%). Eval2는 최고 47.18%(SpatialNet+Paraformer 미세조정)로, 분리 프런트엔드 선택이 20포인트 가까이 차이를 만듦 (GitHub README 수치)
- **Physical AI 시사점**: 차량(이동 플랫폼) 음성 인터페이스에서 병목은 ASR 모델 자체보다 다채널 분리·AEC 프런트엔드라는 점을 정량으로 보여줌. 범용 대형 음성 모델의 실환경 도메인 격차가 커서 소량 도메인 데이터 미세조정이 필수. 영어 실차 다화자 공개 데이터 공백은 여전함
- **링크**: https://arxiv.org/abs/2505.23036 , https://github.com/DaiYvhang/AISHELL-5 , https://openslr.org/159/
