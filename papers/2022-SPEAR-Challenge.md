# An Introduction to the Speech Enhancement for Augmented Reality (SPEAR) Challenge
- **저자**: Pierre Guiraud, Sina Hafezi, Patrick A. Naylor, Alastair H. Moore, Jacob Donley, Vladimir Tourbabin, Thomas Lunner / IWAENC 2022
- **문제**: 머리 장착 마이크 어레이로 대상 화자를 향상하는 알고리즘을 공통 조건에서 비교할 벤치마크가 없었음. 실녹음(EasyCom)만으로는 깨끗한 기준 신호가 없어 intrusive 지표를 계산하기 어려움
- **방법**: EasyCom을 TASCAR로 디지털 재현·확장해 시뮬레이션 데이터 3종(D2~D4)을 만들고 실녹음 D1과 함께 제공. 알고리즘은 머리 자세 등 위치 정보를 쓸 수 있음. IEEE SPS 데이터 챌린지로 운영
- **데이터셋/벤치마크**: [SPEAR](../datasets/SPEAR.md) (기반: [EasyCom](../datasets/EasyCom.md))
- **결과**: MVDR 베이스라인과 평가 도구(spear-tools, 지표 12종) 공개. 참가 팀 결과는 후속 논문 "The SPEAR Challenge – Review of Results"(Tourbabin 외, Forum Acusticum 2023)에 정리. 구체 수치는 미확인(원문 PDF 접속 불가)
- **Physical AI 시사점**: 같은 장면의 실측·시뮬레이션 쌍으로 이동 어레이 향상 기법의 sim-to-real 차이를 측정할 수 있음. 로봇 머리 어레이 데이터를 시뮬레이션으로 늘리는 방식의 참고 사례
- **링크**: https://research.facebook.com/file/620127746171784/An-Introduction-to-the-Speech-Enhancement-for-Augmented-Reality-(Spear)-Challenge.pdf , https://cris.bgu.ac.il/en/publications/an-introduction-to-the-speech-enhancement-for-augmented-reality-s/
