# CHiME-9 ECHI (Enhancing Conversations to address Hearing Impairment)
- **언어**: 영어 (화자 억양 다양)
- **규모**: 세션 49개, 화자 196명, 세션당 30분 이상 (공식 baseline README). Hugging Face 데이터 카드 기준(웹 검색 요약): train 30세션·118화자·18.0시간, dev 약 6.0시간, eval 약 5.4시간. 깨끗한 화자 음성(speaker ID 등록용)은 LibriSpeech·EARS 문장 낭독으로 수록된 것으로 보이나 정확한 구성은 미확인
- **녹음 환경**: 카페테리아처럼 꾸민 시끄러운 공간에서 최대 4인 자연 대화. 다른 화자의 방해 발화와 효과음을 크기를 바꿔 가며 재생. 한 참여자는 Project Aria 안경(7채널), 다른 참여자는 귀마다 마이크 2개인 보청기(4채널)를 착용. 모든 참여자의 근접 마이크 기준 신호와 머리 움직임 추적 데이터 포함
- **Physical AI 활용 포인트**: 움직이는 머리 장착 어레이로 "알고 있는 대화 상대"의 음성만 낮은 지연으로 뽑아내는 과제. 사람 곁에서 대화하는 로봇·착용형 기기에서 대상 화자 추출(TSE) 전처리, 겹침이 많은 다자 대화 처리에 바로 연결됨
- **라이선스/연구 이용**: 서명한 Data Use Agreement 제출 후 주최측 승인 필요. 학술·벤치마크 용도로 제한(상업 이용 불가로 보이나 원문 미확인)
- **접근 방식**: 신청 (Hugging Face gated, `CHiME9-ECHI/CHiME9-ECHI`)
- **주요 사용 논문**: [CHiME-9 ECHI Challenge](../papers/2026-CHiME-9-ECHI.md) (arXiv 2609.26306), IEEE Data Descriptions vol. 3 데이터 기술 논문(서지 세부 미확인)
- **출처**: https://github.com/CHiME9-ECHI/CHiME9-ECHI , https://huggingface.co/datasets/CHiME9-ECHI/CHiME9-ECHI , https://www.chimechallenge.org/current/task2/index , https://eprints.whiterose.ac.uk/id/eprint/241320/
