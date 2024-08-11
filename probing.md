- RAG를 많이 하는데 LLM이 Context를 어떻게 활용하는지, 어떤 behavior를 보이는지 탐구한 연구는 아직 별로 없음.
- Causal Mediation (+IE, Inderect Effect) 방법론으로 input의 일부를 corrupt 해가면서 성능에 영향을 미치는 부분을 찾는 실험
- Attention Contribution 보면서 어느 부분을 예측할 때 가장 많이 보는지 실험
- Attention KnockOut으로 특정 부분을 Attention 날려보면서 성능 저하를 관찰함. 결론은 잘 이해하지 못함.

결론
1. rag context가 있는 경우 llm은 parametric memory대신 context에 집중한다.
