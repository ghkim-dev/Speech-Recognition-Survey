# AVICAR: Audio-Visual Speech Corpus in a Car Environment
- **저자**: Bowon Lee, Mark Hasegawa-Johnson 외 (UIUC) / Interspeech 2004 (ICSLP)
- **문제**: 차량 안 음성 인식은 엔진·도로·바람 잡음 때문에 성능이 크게 떨어짐. 다채널 오디오와 입술 영상을 함께 쓰는 연구에 필요한 대규모 차량 내 시청각 코퍼스가 없었음
- **방법**: 선바이저의 8마이크 선형 어레이와 대시보드 카메라 4대로 주행 중 화자 발화(숫자, 단어, 문장)를 다섯 가지 주행·잡음 조건에서 녹음. 장비 구성과 수집 절차를 기술
- **데이터셋/벤치마크**: [AVICAR](../datasets/AVICAR.md) (화자 100명, 약 59,000 발화, 2차 자료)
- **결과**: 코퍼스 기술 논문으로 인식 벤치마크 결과는 확인하지 못함(미확인). 이후 Sari 외(Interspeech 2018)가 TIMIT 서브셋에서 첫 시청각 인식 결과를 보고
- **Physical AI 시사점**: 차량 내 실제 주행 잡음 + 다채널 + 시각(입술) 정보를 함께 다루는 초기 기준점. 최신 차량 데이터(CAVEMOVE 등)는 합성용 음향 자료 중심이라, 실제 사람 발화 평가셋으로서 AVICAR의 가치가 여전히 있음. 다만 라이선스·접근 경로가 불분명해 사용 전 저자 문의 필요
- **링크**: https://www.isca-archive.org/interspeech_2004/lee04m_interspeech.html , https://www.isca-archive.org/interspeech_2018/sari18_interspeech.html
