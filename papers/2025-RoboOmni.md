# RoboOmni: Proactive Robot Manipulation in Omni-modal Context
- **저자**: Siyin Wang, Jinlan Fu 외 (Fudan/OpenMOSS, NUS 등, 14명) / ICLR 2026 (arXiv 2510.23763, 2025-10)
- **문제**: 기존 VLA는 명시적 텍스트 명령에 의존하고, 음성은 ASR/TTS 캐스케이드로 처리해 맥락 단서(감정, 화자, 환경음)를 잃음
- **방법**: 음성·환경음·시각을 함께 받는 omni-modal LLM 기반 Perceiver-Thinker-Talker-Executor 구조(구성 명칭은 2차 자료로 미확인). 사용자 의도를 먼저 추론하고 행동 전에 확인 질문을 함
- **데이터셋/벤치마크**: [OmniAction](../datasets/OmniAction.md) (약 14만 에피소드), 시뮬레이션 및 실제 로봇 평가(세부 수치 미확인)
- **Physical AI 시사점**: 명령어 인식을 넘어 대화·환경음 맥락에서 의도를 추론하는 능동형 음성 로봇 조작
- **링크**: https://arxiv.org/abs/2510.23763 , https://openmoss.github.io/RoboOmni , https://proceedings.iclr.cc/paper_files/paper/2026/hash/33610fba262d7b6fed0810b89f55e147-Abstract-Conference.html
