# EasyCom: An Augmented Reality Dataset to Support Algorithms for Easy Communication in Noisy Environments
- **저자**: Jacob Donley, Vladimir Tourbabin, Jung-Suk Lee, Mark Broyles, Hao Jiang, Jie Shen, Maja Pantic, Vamsi Krishna Ithapu, Ravish Mehra (Facebook Reality Labs) / arXiv 2021 (2107.04174). 학회 게재 여부 미확인
- **문제**: AR 안경 착용자가 시끄러운 곳에서 대화를 잘 듣도록 돕는 알고리즘을 개발·평가할 실제 1인칭 다채널 데이터가 없었음. 착용형 기기는 머리 움직임 때문에 고정 어레이와 조건이 다름
- **방법**: 레스토랑 잡음 속 자연 대화를 AR 안경 6채널 어레이, 1인칭 영상, 헤드셋 근접 마이크, 머리 자세 추적으로 동시에 수록. 대상 화자 음성을 향상해 SNR·음질·명료도를 높이는 벤치마크 과제 정의
- **데이터셋/벤치마크**: [EasyCom](../datasets/EasyCom.md)
- **결과**: 베이스라인 방법이 명료도·음질·SNR 지표 모두에서 개선됨(논문 초록 기준). 구체 수치와 WER은 미확인(arXiv 직접 접속 불가)
- **Physical AI 시사점**: 머리에 장착한 움직이는 마이크 어레이로 원거리·잡음 음성을 다루는 몇 안 되는 공개 실측 데이터. 휴머노이드 머리 마이크나 스마트 안경용 빔포밍·대상 화자 추출·ASR 연구의 출발점
- **링크**: https://arxiv.org/abs/2107.04174 , https://github.com/facebookresearch/EasyComDataset
