# STOP (Spoken Task Oriented Parsing)
- **언어**: 영어
- **규모**: 오디오 236,477개, 약 218시간, 화자 885명(논문 비교표 기준. 공식 문서는 "20만 개 이상, 800명 이상"으로 표기)
- **녹음 환경**: TOPv2 텍스트 질의를 크라우드 화자가 낭독. train은 발화당 1회, valid/test는 2회 녹음. 화자는 한 split에만 배정(화자 중복 없음). 녹음 기기·거리는 미확인
- **도메인/주석**: TOPv2 계층형 의도·슬롯 파스(알람·리마인더·날씨·타이머·음악·내비게이션·메시징·이벤트 등 8개 도메인으로 알려짐, 원문 미확인). reminder·weather 도메인은 저자원 split(25 SPIS) 별도 제공
- **Physical AI 활용 포인트**: 음성 명령을 계층형 의미 파스로 바로 바꾸는 end-to-end SLU. 다단계 로봇·가전 명령("10분 뒤 알람 맞추고 날씨 알려줘")의 구조적 이해 평가
- **라이선스/연구 이용**: 미확인 (공식 문서가 `dl.fbaipublicfiles.com/stop/LICENSE.txt`를 링크하지만 이번 세션에서 접속 불가)
- **접근 방식**: 공개 다운로드 (Meta, 공식 문서 기준)
- **주요 사용 논문**: [STOP (Tomasello 외, IEEE SLT 2022)](../papers/2022-STOP.md)
- **출처**: https://arxiv.org/abs/2207.10643 , https://facebookresearch.github.io/spoken_task_oriented_parsing/
