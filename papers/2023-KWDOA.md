# KWDOA: Adapted Dataset for Detection of the Direction of Arrival of the Keyword
- **저자**: David Beneš, Luboš Šmídl (University of West Bohemia) / CAINE 2023 (36th International Conference on Computer Applications in Industry and Engineering), EPiC Series in Computing vol. 97 (2024), pp. 30–37, DOI 10.29007/5k86
- **문제**: 마이크 어레이 기반 KWS를 학습·평가할 공개 다채널 키워드 데이터가 부족하고, 키워드 검출과 화자 방향 추정을 함께 다루는 과제 정의가 없음
- **방법**: Speech Commands를 PyroomAcoustics로 원형 4채널(57 mm 간격) 어레이 수음처럼 시뮬레이션하고 DOA 정답을 붙여 KWDOA 과제(키워드 검출 + 방향 추정)를 제안. 기준 모델·성능 수치는 확인 못 함 → 미확인
- **데이터셋**: [KWDOA](../datasets/KWDOA.md) (CC BY 4.0, LINDAT)
- **Physical AI 시사점**: 저가 어레이 기반 "명령어 듣고 돌아보기" 기능의 공개 학습 자원. 학회 등급은 낮지만 [Direction-Aware KWS(2026)](2026-Direction-Aware-KWS-Spatial-Priors.md) 같은 최근 연구의 공개 비교 기준 후보
- **링크**: https://easychair.org/publications/paper/vsB3p , https://lindat.mff.cuni.cz/repository/xmlui/handle/11234/1-5140
