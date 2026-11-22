# Efficient Keyword Spotting Using Dilated Convolutions and Gating
- **저자**: Alice Coucke, Mohammed Chlieh, Thibault Gisselbrecht, David Leroy, Mathieu Poumeyrol, Thibaut Lavril (Snips) / **IEEE ICASSP 2019**, pp. 6351–6355 (DBLP), arXiv 1811.07684
- **문제**: 스마트 기기 웨이크워드 검출은 저전력·저지연이 필요하고, 실사용에서는 시간당 오경보(FA/h)를 낮게 고정한 채 오거부(FRR)를 줄여야 함. 또한 웨이크워드 전용 공개 데이터가 없어 재현성이 낮음
- **방법**: WaveNet 계열 dilated causal convolution + gated activation + residual/skip 연결로 긴 수용 영역을 적은 연산으로 확보하는 스트리밍 KWS 모델. 웨이크워드 끝 구간만 양성 표적으로 두는 end-of-keyword 라벨링으로 지연·오경보를 줄임. max-pooling loss 학습 LSTM과 CNN을 베이스라인으로 비교. 동시에 "Hey Snips" 데이터셋을 연구용으로 공개
- **데이터셋**: [Hey Snips](../datasets/Hey-Snips.md) (2.2K명 이상 화자 크라우드소싱)
- **평가**: 0.5 FA/h 고정 운영점에서 FRR. 깨끗한 조건과 잡음 조건(양성 샘플에 5 dB SNR 잡음 부가)
- **결과**: 파라미터 수는 세 모델이 비슷한데, WaveNet 모델이 LSTM 대비 FRR을 깨끗한 조건 약 94%, 잡음 조건 약 86% 줄임(CNN 대비 각각 약 95%, 88%, 웹 검색 2차 자료). CNN은 FLOPS가 훨씬 많음. 절대 FRR 값과 정확한 파라미터 수는 원문 Table 미확인
- **Physical AI 시사점**: 로봇·가전의 상시 청취 단계는 "FA/h 고정 후 FRR" 지표로 설계해야 한다는 기준을 제시. dilated conv 스트리밍 구조는 이후 엣지 KWS(예: TC-ResNet, BC-ResNet 계열 비교 실험)의 표준 비교 대상. 다만 원거리·로봇 ego-noise 조건 평가는 없음
- **링크**: https://arxiv.org/abs/1811.07684 , https://dblp.org/rec/conf/icassp/CouckeCGLPL19 , https://github.com/sonos/keyword-spotting-research-datasets
