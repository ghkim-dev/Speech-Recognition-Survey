# End-to-End Direction-Aware Keyword Spotting with Spatial Priors in Noisy Environments
- **저자**: Rui Wang, Zhifei Zhang, Yu Gao, Xiaofeng Mou, Yi Xu (Midea Group, 2차 자료 기준) / arXiv 2603.09505 (2026-03, eess.AS, CC BY-NC-ND 4.0). 학회 채택 여부 미확인
- **문제**: 가전·로봇의 다채널 마이크로 키워드를 검출할 때, 잡음 환경에서 단일 채널 KWS는 성능이 떨어지고 별도 음성 향상 + KWS 직렬 구조는 최적화가 따로 됨
- **방법**: (1) 채널 간 특징을 학습하는 공간 인코더, (2) 목표 화자 방향(DOA) 사전 정보를 넣는 공간 임베딩, (3) 스트리밍 백본을 end-to-end로 결합. 학습·평가 때 목표 DOA를 안다고 가정하고, 실제 배치 때는 임의의 DOA 추정기가 값을 공급한다고 봄
- **데이터/벤치마크**: 여러 SNR의 시뮬레이션 잡음 조건. 사용 키워드 코퍼스·어레이 구조는 확인 못 함 → 미확인
- **결과**: 공간 모델링과 방향 사전 정보가 각각 기준 모델보다 낫고, 둘을 함께 쓸 때 가장 좋다고 보고. 구체 수치 미확인
- **관련 연구**: End-to-End Multi-Look KWS(Tencent, arXiv 2005.10386)가 다방향 음성 향상과 KWS를 함께 학습한 선행 연구. 공개 데이터 측면에서는 [KWDOA](../datasets/KWDOA.md)가 같은 "키워드+방향" 과제를 다룸
- **Physical AI 시사점**: "말한 사람 방향"을 KWS 입력으로 주는 조건화 방식. 드론 KWS의 잡음 상태 조건화, 드론 SE의 로터 상태 조건화와 같은 계열로, 로봇이 이미 아는 정보(카메라로 본 사람 위치, 로터 회전수 등)를 음성 처리에 주입하는 설계가 KWS에서도 확산 중
- **링크**: https://arxiv.org/abs/2603.09505 , https://arxiv.org/html/2603.09505v1
