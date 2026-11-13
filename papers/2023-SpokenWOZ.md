# SpokenWOZ: A Large-Scale Speech-Text Benchmark for Spoken Task-Oriented Dialogue Agents
- **저자**: Shuzheng Si 외 9명 (Alibaba DAMO 등) / NeurIPS 2023 Datasets and Benchmarks Track
- **문제**: 기존 과업 지향 대화 데이터(MultiWOZ 등)는 텍스트 위주라 실제 음성 대화의 ASR 잡음, 단어 단위 끊어 말하기, 구어 추론을 반영하지 못함
- **방법**: 전화 통화로 수집한 사람 간 음성 대화 249시간을 음성·텍스트 쌍으로 공개. cross-turn 슬롯과 reasoning 슬롯이라는 구어 특유의 과제를 새로 정의하고, 텍스트 모델·음성+텍스트 모델·LLM으로 대화 상태 추적(DST)과 응답 생성 베이스라인 제공
- **데이터셋/벤치마크**: [SpokenWOZ](../datasets/SpokenWOZ.md)
- **결과**: 최고 DST 모델 joint goal accuracy 25.65%, 최고 end-to-end 모델 과업 성공률 52.1%(논문 초록 기준). 텍스트 데이터 대비 큰 성능 격차
- **Physical AI 시사점**: 로봇이 음성 대화로 사용자 요구를 여러 턴에 걸쳐 파악하는 문제의 공개 기준선. 음성 직결 VLA(VLAS, RoboOmni)의 대화형 확장을 평가할 때 참고할 수 있음
- **링크**: https://arxiv.org/abs/2305.13040 , https://proceedings.neurips.cc/paper_files/paper/2023/hash/7b16688a2b053a1b01474ab5c78ce662-Abstract.html
