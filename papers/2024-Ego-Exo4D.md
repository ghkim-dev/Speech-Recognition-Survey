# Ego-Exo4D: Understanding Skilled Human Activity from First- and Third-Person Perspectives
- **저자**: Kristen Grauman 외 (Meta FAIR + 대학 컨소시엄) / CVPR 2024 (arXiv 2311.18259)
- **문제**: 숙련 활동을 1인칭·3인칭에서 동시에 이해하기 위한 대규모 다시점·다중 모달 데이터 부재
- **방법**: 13개 도시 800명 이상이 Aria 안경(7채널 오디오·시선·SLAM·IMU)과 GoPro 4~5대로 동기 녹화. 언어 자원으로 착용자 1인칭 내레이션(Narrate & Act), 3인칭 원자 행동 기술(V2 432,467건), 전문가 음성 해설(V2 117,812개 녹음) 제공. V2(2024-03)에서 전 테이크 Aria 오디오 추출본과 Whisper large-v3 전사 추가
- **데이터셋/벤치마크**: [Ego-Exo4D 오디오·음성 자원](../datasets/Ego-Exo4D-Audio.md). 벤치마크 7종(키스텝, 숙련도 추정, 자세, 관계 등) — 음성 인식 전용 벤치마크는 없음
- **결과**: 데이터셋 논문으로 ASR 수치는 없음. 오디오는 주로 키스텝·숙련도 등 비디오 과제의 보조 모달로 사용
- **Physical AI 시사점**: 작업 잡음 속 1인칭 다채널 음성 + 손·몸 3D 자세 + 시선이 정렬된 드문 자원. 로봇이 사람의 작업 중 설명/지시를 듣고 행동 단계와 매칭하거나, 전문가 음성 피드백을 학습 신호로 쓰는 연구의 데이터 기반. 기계 전사만 있어 ASR 평가용으로는 별도 정답 전사 필요
- **링크**: https://arxiv.org/abs/2311.18259 , https://docs.ego-exo4d-data.org/
