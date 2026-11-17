# Aria Everyday Activities Dataset
- **저자**: Zhaoyang Lv, Nicholas Charron, Pierre Moulon, Alexander Gamino 외 (Meta Reality Labs Research) / arXiv 2402.13349 (2024)
- **문제**: 1인칭(egocentric) 다중 센서 데이터를 공간 정보와 함께 제공하는 공개 데이터가 부족함. 기존 Aria Pilot Dataset의 Everyday Activities 부분을 최신 처리로 갱신할 필요
- **방법**: Project Aria 안경으로 여러 착용자가 실내 5곳에서 일상 활동 143개를 녹화. Machine Perception Services(MPS)로 6DoF 궤적, 반밀집 포인트 클라우드, 3D 시선 산출. 시간 정렬된 음성 전사 포함. projectaria_tools로 로딩·시각화 도구 제공
- **데이터셋/벤치마크**: [Aria Everyday Activities](../datasets/Aria-Everyday-Activities.md) (7.5시간 이상)
- **결과**: 벤치마크 수치보다는 활용 예시(신경 장면 재구성, 프롬프트 기반 분할 등)를 제시. 음성 관련 정량 평가는 없음(확인 범위 내)
- **Physical AI 시사점**: 음성 데이터셋은 아니지만, 다채널 오디오 + 착용자 3D 위치·시선 + 장면 지도가 한 번에 있는 드문 공개 자료. 체화 에이전트가 "어디서 누가 무슨 말을 했는지"를 공간적으로 이해하는 연구(예: SAVVY의 시청각 공간 추론)의 기반 데이터로 쓰임. 같은 Aria 안경 기반인 [MMCSG](../datasets/MMCSG.md), [CHiME-9 ECHI](../datasets/CHiME-9-ECHI.md)와 하드웨어가 같아 전이 연구에 유리
- **링크**: https://arxiv.org/abs/2402.13349 , https://www.projectaria.com/datasets/aea/
