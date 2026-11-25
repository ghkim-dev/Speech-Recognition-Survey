# Enhancing drone audition with rotor-conditioned deep models
- **저자**: Andrea Gulli, Federico Fontana, Carlo Drioli, Daniele Salvati, Giovanni Ferrin (소속은 Univ. of Udine 추정, 미확인) / **EURASIP Journal on Audio, Speech, and Music Processing 2025, article 35** (2025-10-24 게재, DOI 10.1186/s13636-025-00425-2, 오픈 액세스)
- **문제**: 드론 탑재 마이크는 모터·프로펠러·기류 잡음으로 SNR이 매우 낮아 음성 향상이 어려움. 로터 속도는 고장 진단·ego-noise 합성 등 다른 UAV 과제에는 쓰였지만 딥러닝 음성 향상의 조건 신호로는 쓰이지 않았음
- **방법**: 로터 속도 시계열을 구조적 조건 입력으로 신경망 음성 향상 모델에 주입. 시간-주파수 기반과 파형 기반 아키텍처 모두에 적용(검색 요약상 Wave-U-Net, DCCRN, Deep Complex U-Net — 원문 대조 미확인). 조건화 방식(FiLM 등) 세부는 미확인
- **데이터셋/벤치마크**: [DREGON](../datasets/DREGON.md) (로터 속도가 함께 기록된 유일한 공개 드론 데이터로 보임), SI-SDR·STOI·PESQ 평가
- **결과**: 지표×SNR 16개 구성 중 **13개에서 최고 모델이 로터 조건화 모델**. 전체 용량 베이스라인과의 80개 비교 중 55개에서 통계적으로 유의한 향상(검색 요약 기준). 파라미터 **25%**만 쓰는 경량 로터 조건화 변형(DCCRN 계열로 보고)이 최고 또는 그에 근접한 성능
- **공개 여부**: 논문 오픈 액세스. 코드 공개 여부 미확인
- **Physical AI 시사점**: "로봇 자신의 상태(모터 속도)를 잡음 제거 모델의 입력으로 쓰는" 접근을 정량 검증. 휴머노이드·이동 로봇에서도 관절 모터 전류·속도 같은 고유수용 신호를 ego-noise 조건으로 쓰는 방향(Pepper ego-speech, MChRSR 이동 잡음)으로 일반화 가능하며, 경량 모델로도 이득이 유지돼 온보드 실시간 처리에 유리. 반대로 DroneAudioSet처럼 로터 속도가 없는 데이터에서는 바로 쓸 수 없어, 향후 데이터셋 설계에 로봇 상태 로그 동시 기록이 중요함을 보여줌
- **링크**: https://link.springer.com/article/10.1186/s13636-025-00425-2 , https://www.researchgate.net/publication/396869552_Enhancing_drone_audition_with_rotor-conditioned_deep_models
