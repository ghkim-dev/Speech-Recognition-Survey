# Mixer 6 Speech
- **언어**: 영어(미국 필라델피아 지역 원어민)
- **규모**: LDC2013S03 기준 약 15,863시간(다채널 합산 녹음 시간), 화자 594명. CHiME-8용 전사 서브셋 LDC2025S07은 13개 마이크 합산 1,063시간 = 음성 기준 약 80시간 (LDC 카탈로그 수치, 웹 검색 요약으로 확인)
- **녹음 환경**: 2009~2010년 LDC 녹음실에서 인터뷰, 낭독, 전화 대화를 수록. 한 화자가 최대 3일, 세션당 최대 45분. 방 안 여러 위치에 놓인 13개 마이크(근접~원거리, 종류 상이)로 동시 녹음. 정확한 마이크 배치는 LDC 문서에서 직접 확인하지 못함(미확인)
- **Physical AI 활용 포인트**: 같은 발화를 근접부터 원거리까지 성질이 다른 마이크로 동시에 녹음해, 로봇·기기의 마이크 위치나 종류가 달라질 때 인식 성능이 어떻게 변하는지 볼 수 있음. 2인 인터뷰라 겹침이 적어, CHiME-7/8 DASR에서 가장 쉬운 시나리오(원거리 조건 자체의 영향을 분리해 보기 좋음)
- **라이선스/연구 이용**: LDC2013S03은 LDC 회원 전용(회원 할인가, 비회원은 회원 가입 필요). LDC2025S07(CHiME-8 전사 서브셋)은 LDC User Agreement for Non-Members. 비용·상업 이용 조건 세부는 미확인
- **접근 방식**: LDC (유료/계약)
- **주요 사용 논문**: [CHiME-7 DASR Challenge](../papers/2023-CHiME-7-DASR-Challenge.md), [CHiME-8 DASR Challenge](../papers/2024-CHiME-8-DASR-Challenge.md). 원래 NIST 화자 인식 평가(SRE)용으로 수집된 Mixer 시리즈의 6번째 단계
- **출처**: https://catalog.ldc.upenn.edu/LDC2013S03 , https://catalog.ldc.upenn.edu/LDC2025S07
