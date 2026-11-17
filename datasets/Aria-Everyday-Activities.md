# Aria Everyday Activities (AEA)
- **언어**: 영어로 추정 (명시 확인 못함, 미확인)
- **규모**: 녹화 143개, 누적 7.5시간 이상, 실내 장소 5곳 (Project Aria 문서·논문 초록, 웹 검색 요약)
- **녹음 환경**: Project Aria 안경(1세대)을 쓴 여러 착용자가 집 안에서 요리·식사·대화 같은 일상 활동을 수행. 7채널 48kHz 마이크 배열(앞 테 5개, 다리 쪽 2개, 2차 자료 SAVVY 논문 부록 기준), RGB·SLAM 카메라, 시선, IMU, 기압계·자력계 동시 기록. 다수 착용자가 같은 공간에서 동기화 녹화
- **주석**: 시간 정렬된 음성 전사(Aria Pilot Dataset에서 ASR로 생성한 전사를 그대로 사용, 2차 자료), 3D 궤적, 장면 포인트 클라우드, 프레임별 3D 시선
- **Physical AI 활용 포인트**: 1인칭 다채널 음성과 착용자 위치·시선·장면 3D 정보가 함께 있어, "누가 어디서 말했는지"를 공간적으로 다루는 체화 에이전트·로봇 음성 연구(음원 위치 추정, 시청각 화자 귀속, 공간 인식 음성 LLM 평가)에 쓸 수 있음. 다만 음성 전사는 ASR 자동 생성이라 ASR 평가용 정답으로는 품질 확인 필요
- **라이선스/연구 이용**: Meta가 발행한 Aria Everyday Activities 데이터셋 라이선스 계약. 재배포·공개 전시·개인 정보 추론 금지, 출판 시 "Aria Everyday Activities Dataset, Meta Reality Labs-R" 표기 의무, 상업 이용은 projectaria@meta.com 별도 문의(라이선스 페이지 검색 요약). 권리 부여 조항 원문은 직접 확인 못함(미확인)
- **접근 방식**: 공개 (projectaria.com에서 라이선스 동의 후 다운로드, projectaria_tools(Apache 2.0)로 로딩)
- **주요 사용 논문**: [Aria Everyday Activities Dataset](../papers/2024-Aria-Everyday-Activities.md) (arXiv 2402.13349), SAVVY(arXiv 2506.05414, 공간 인식 시청각 LLM 벤치마크에 활용)
- **출처**: https://www.projectaria.com/datasets/aea/ , https://www.projectaria.com/datasets/aea/license/ , https://github.com/facebookresearch/projectaria_tools , https://arxiv.org/abs/2402.13349
