# Speech Model Pre-training for End-to-End Spoken Language Understanding
- **저자**: Loren Lugosch, Mirco Ravanelli, Patrick Ignoto, Vikrant Singh Tomar, Yoshua Bengio / Interspeech 2019
- **문제**: end-to-end SLU는 레이블된 음성-의도 데이터가 많이 필요
- **방법**: 음소·단어 예측으로 음향 모델을 사전학습(LibriSpeech 강제정렬)한 뒤 의도 분류로 미세조정. 미관측 문구 일반화 예비 실험
- **데이터셋/벤치마크**: Fluent Speech Commands(본 논문에서 공개), LibriSpeech(사전학습)
- **결과**: FSC 정확도 98.8%(Papers with Code 수록치, 검증 미완), 소량 학습 데이터에서도 개선
- **Physical AI 시사점**: ASR 전사 없이 명령→의도를 직접 매핑하는 경량 SLU, 엣지 기기 음성 제어
- **링크**: https://www.isca-archive.org/interspeech_2019/lugosch19_interspeech.html , https://arxiv.org/abs/1904.03670 , 코드 https://github.com/lorenlugosch/end-to-end-SLU
