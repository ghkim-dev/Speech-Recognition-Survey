# NatSGLD (Natural Speech, Gesture, Logic, and Demonstration)
- **언어**: 영어 (샘플 발화 기준, 예: "turn on the burner under the water")
- **규모**: 다중 모달 명령 1,143개, 참가자 18명, 활동 11종·객체 20종·객체 상태 16종 (논문 초록, 2차 자료). 공개 샘플 npz의 참가자 키도 18개. LTL 샘플 파일은 734개 명령. 총 녹음 시간은 미확인
- **녹음 환경**: Wizard-of-Oz 방식 — 참가자는 자율 로봇이라 믿고 Unity 시뮬레이터 속 Baxter 로봇(주방 요리 과제)에게 음성·제스처로 지시하고, 실제 동작은 사람이 원격 조작. 참가자 시점 영상에 44kHz 오디오 포함, 실험자 시점·다중 카메라 방 시점·로봇 1인칭(RGB·깊이·분할) 영상 제공. 명령별 시작/끝 시각(ms), 음성 유무·제스처 유무 플래그
- **주석**: 발화 전사 텍스트(FEVA 도구로 이벤트 주석), GloVe·BART 임베딩, OpenPose 25 키포인트 제스처, L2CS-Net 시선, 로봇 관절 상태·객체 bbox, 과제 정답으로 LTL(선형 시간 논리) 공식 + 정답 행동·객체
- **Physical AI 활용 포인트**: 자연스러운(대본 없는) 음성+제스처 로봇 명령을 "무엇을 해야 하는가"의 형식 표현(LTL)·시연 궤적과 직접 연결. 음성 명령 → 과제 구조 파싱, 제스처로 지시 대상 보완(deixis), 시연 기반 학습 평가에 사용. 다만 ASR 관점에서는 규모가 작고 오디오가 영상 파일 안에 포함된 형태
- **라이선스/연구 이용**: MIT License (GitHub LICENSE 확인, 데이터셋·시뮬레이터·코드에 적용된다고 README에 명시) → 상업 이용 포함 허용
- **접근 방식**: 공개 (GitHub `sneheshs/natsgld` 메타데이터·샘플, 전체 데이터는 프로젝트 사이트 snehesh.com/natsgld — 이번 세션에서 사이트 접속 불가로 전체 다운로드 조건 미확인)
- **주요 사용 논문**: [NatSGLD: A Dataset with Speech, Gesture, Logic, and Demonstration for Robot Learning in Natural Human-Robot Interaction](../papers/2025-NatSGLD.md) (ACM/IEEE HRI 2025)
- **출처**: https://raw.githubusercontent.com/sneheshs/natsgld/main/README.md , https://raw.githubusercontent.com/sneheshs/natsgld/main/LICENSE , https://www.snehesh.com/natsgld , https://arxiv.org/abs/2502.16718 , https://dl.acm.org/doi/10.5555/3721488.3721628
