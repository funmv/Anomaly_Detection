# Anomaly Transformer 분석
(0)->(1)->(2)->(3)->(4) 순서로 호출되고, (4)->(3)->(2)->(1)->(0)순으로 실행  
입력을 임베딩해서(0), 넘기면 att layer를 호출(1)하고, att레이어에서 self att을 호출(2)하고,  
self att에서 임베딩입력을 projection후 att계산부 호출(3), 그러면 (4)에서 prior, series att계산  

(0) 임베딩  
(1) 레이어별 호출  
(2) self att 호출  
(3) projection + att 계산 호출  
(4) att 계산  

