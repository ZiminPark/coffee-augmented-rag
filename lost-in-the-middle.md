# Summary
QA Task와 Retrieval Task(key-val)에서 정답 문서가 맨 앞이나 맨 뒤에 있는 경우의 성능보다 중간 부분에서 성능이 떨어짐을 관찰함.  
떨어지는 이유를 알기 위해
  
  1. Model 구조 (Encoder-Decoder vs Decoder Only)
  2. Query Aware Contextualziation (Query를 문서 앞 뒤에 다둠)
  3. Instruction Fine-Tuning  

의 영향을 확인해봄.
decoder only와 다르게 encoder-decoder는 U-Shaped이 덜함. bidirectional encoder 영향인듯?
QA Contextualziation Retrieve Task에서는 효과가 좋았지만 QA Task에선 별로였음
Instruction Fine-Tuning 전의 Base 모델에서부터 이런 현상이 나타났으므로 Instruction Tuning으로 인한 현상은 아님.


# 생각
Attention이 어떻게 들어가는지 고려가 생각보다 필요함.
후속 연구/ 벤치마크들이 궁금.
1. Lost in the middle을 어떻게 해결했나? 최근 모델들 성적은 어떤가?
2. Lost in the middle을 고려한 벤치마크?
3. Lost in the middle이 두드러지는 Downstream Task와 아닌 Task?
