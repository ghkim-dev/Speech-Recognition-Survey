# KWDOA (Speech Commands Dataset Enhanced for Direction-of-Arrival Estimation)
- **언어**: 영어
- **규모**: [Speech Commands](Speech-Commands.md)를 다채널로 변환. LINDAT 기록 기준 train·validate·test·배경잡음 압축 파일 합계 약 111 GB. 발화 수·클래스 수는 원본을 따르는 것으로 보이나 직접 확인 못 함 → 미확인
- **녹음 환경**: 실녹음이 아닌 시뮬레이션. PyroomAcoustics로 방 잔향·잡음을 넣고, 인접 마이크 간격 57 mm인 원형 4채널 어레이(Seeed 계열 실제 어레이 기하 구조를 따름)로 수음한 것처럼 만듦. 발화마다 도래 방향(DOA) 정답 제공
- **과제**: KWDOA = 키워드 검출 + 말한 사람 방향 추정을 함께 수행
- **Physical AI 활용 포인트**: 저가 4채널 어레이를 단 로봇·스마트 기기가 "명령어를 듣고 그 사람 쪽으로 돌아보기"를 학습·평가하는 공개 데이터. 실제 로봇 ego-noise는 없으므로 실환경 검증은 별도로 필요
- **라이선스/연구 이용**: CC BY 4.0 (LINDAT/CLARIAH-CZ 기록 기준, 2023-04-25 공개). 원본 Speech Commands도 CC BY 4.0
- **접근 방식**: 공개 (LINDAT 저장소 handle 11234/1-5140)
- **주요 사용 논문**: [Beneš, Šmídl, CAINE 2023 (EPiC Series vol. 97, 2024)](../papers/2023-KWDOA.md)
- **출처**: https://lindat.mff.cuni.cz/repository/xmlui/handle/11234/1-5140 , https://easychair.org/publications/paper/vsB3p , https://dspace.zcu.cz/items/ae4fe200-cbdd-43d6-90d9-c4b063c9d58b/full (모두 웹 검색 결과로 확인, 직접 접속 불가)
