# The CHiME-8 MMCSG Challenge: Multi-modal Conversations in Smart Glasses
- **저자**: Kateřina Žmolíková 외 (Meta) / CHiME 2024 Workshop (ISCA Archive). 전체 저자 목록 미확인
- **문제**: 스마트 안경에서 착용자와 대화 상대의 발화를 실시간으로 받아 적고 누가 말했는지 구분해야 함. 지연이 짧아야 하고, 착용자 음성과 상대 음성의 음향 조건이 크게 다름
- **방법**: Aria 안경으로 수록한 양자 대화 데이터 MMCSG를 공개하고, 스트리밍 다화자 ASR 과제 정의. 오디오 외에 영상·IMU 사용 허용. 지표는 화자 귀속 포함 WER과 단어별 지연
- **데이터셋/벤치마크**: [MMCSG](../datasets/MMCSG.md) (Train 8.5h / Dev 8.4h / Eval 9.4h)
- **결과**: 베이스라인(FastConformer 스트리밍) Dev SELF/OTHER WER 14.3~17.9% / 20.3~24.4%(지연 0.62~0.15초). 참가 팀 순위와 최고 WER은 미확인
- **Physical AI 시사점**: 착용형·머리 장착 기기의 스트리밍 대화 인식 표준 벤치마크. 자기 발화/상대 발화 분리, IMU 활용(USTC 팀이 성능 개선 보고)은 로봇 ego-speech·자세 정보 활용 연구에 바로 연결됨
- **링크**: https://www.isca-archive.org/chime_2024/zmolikova24_chime.pdf , https://github.com/facebookresearch/MMCSG , https://arxiv.org/abs/2410.05986
