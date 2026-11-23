# The LOCATA Challenge: Acoustic Source Localization and Tracking
- **저자**: Christine Evers, Heinrich W. Löllmann, Heinrich Mellmann, Alexander Schmidt, Hendrik Barfuss, Patrick A. Naylor, Walter Kellermann (Imperial College London / FAU Erlangen-Nürnberg / HU Berlin 등, 전체 저자 순서·소속 일부 미확인) / **IEEE/ACM TASLP vol. 28, pp. 1620-1643, 2020** (doi:10.1109/TASLP.2020.2990485), arXiv 1909.01008
- **문제**: 음원 위치 추정·추적 알고리즘은 대부분 시뮬레이션이나 자체 녹음으로 평가되어 비교가 어려움. 특히 이동 화자·이동 어레이, 로봇 머리·보청기 같은 실제 기기 조건의 공통 실측 벤치마크가 없었음
- **방법(챌린지 설계)**: 실내 음향실에서 4종 어레이(NAO 로봇 머리 12ch, Eigenmike 32ch, DICIT 평면, 바이노럴 보청기)로 동시 녹음한 6개 과제 코퍼스와 OptiTrack 정답 궤적 공개. 단일 음원 과제(Task 1·3·5)와 다중 음원 과제(Task 2·4·6)를 나눠 평가. 방위각 오차, 추적 연속성(트랙 끊김·교체), 검출 확률·오경보 등 위치 추정·추적 지표를 함께 정의
- **데이터셋/벤치마크**: [LOCATA](../datasets/LOCATA.md)
- **결과**: 과제·제출·어레이별 평균 방위각 오차를 Table III에 보고, 베이스라인은 MUSIC. 참가 보고서 예: Nakadai 외(HARK)는 로봇 머리 어레이에서 MUSIC을 20프레임마다 1회만 수행해도 성능을 유지하며 실시간 처리 달성, 바이노럴 변조 특징 기반 방법은 평균 방위각 오차 4.95°(베이스라인 MUSIC보다 4.25° 개선), NAO 머리 4채널 cascaded tracker는 개발 셋 위치 MAE 4.0°·추적 MAE 4.1°(별도 논문 보고치). **TASLP 논문 Table III의 개별 수치는 미확인** (arxiv.org 직접 접속 불가)
- **Physical AI 시사점**: 이동 어레이(Task 5·6) 조건에서 로봇 자체의 움직임이 추적 난도를 크게 높인다는 점을 공통 벤치마크로 처음 정량화한 사례. 로봇 원거리 ASR 파이프라인(위치 추정 → 빔포밍 → 인식)의 앞단 평가 기준이며, 11-22 Lend me an Ear(화자 위치 추정 후 팔로 어레이 재구성)·[ODAS](2022-ODAS.md) 같은 로봇 청각 시스템의 위치 추정 모듈 검증에 쓸 수 있음
- **링크**: https://arxiv.org/abs/1909.01008 , https://eprints.soton.ac.uk/439585/ , https://spiral.imperial.ac.uk/entities/publication/b75b8084-c574-45fa-b03f-0e1f0eef7bf4
