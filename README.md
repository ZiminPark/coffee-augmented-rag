# coffee-augmented-rag

RAG를 개발하다 보면 엄밀하게 검증은 못 해봤지만 이렇지 않을까? 싶은 질문이 많습니다.  
이런 질문들 공유하고 Research Paper 살펴보면서 이야기 나누어 보아요.  
[Closed Issue](https://github.com/ZiminPark/coffee-augmented-rag/labels)에 Discussion과 질문들이 있습니다. 

| Topic                                            |
|------------------------------------------------|
| [RAG Evaluation을 구성할 때 어떤 점들을 고려해야할까](#rag-evaluation을-구성할-때-어떤-점들을-고려해야할까) |
| [Long Context가 LLM에 들어갈 때 성능이 어떻게 변할까](#long-context가-llm에-들어갈-때-성능이-어떻게-변할까) |
| [RAG+FT 어떻게 시너지 낼수 있을까](#ragft-어떻게-시너지-낼수-있을까)                |
| [RAG를 할때 LLM parameter에는 무슨 일이 일어날까](#rag를-할때-llm-parameter에는-무슨-일이-일어날까)   |
| [Spreadsheet 데이터는 어떻게 인덱싱하는게 좋을까](#spreadsheet-데이터는-어떻게-인덱싱하는게-좋을까)   | 
| [Graph RAG는 어떤 상황에서 효과적일까](#graph-rag는-어떤-상황에서-효과적일까)            |
| [Citation을 어떻게 하는게 제일 효과적일까 & 평가할까](#citation을-어떻게-하는게-제일-효과적일까--평가할까) |


# RAG Evaluation을 구성할 때 어떤 점들을 고려해야할까

**Reference**  
- [CRAG - Comprehensive RAG Benchmark](https://arxiv.org/html/2406.04744v1)  
- [Further Readings](https://github.com/ZiminPark/coffee-augmented-rag/issues/4)
<img width="1028" alt="image" src="https://github.com/user-attachments/assets/78c4f57f-8724-4f01-9bc1-665463d855bb">


**Question/ Discussion**  
https://github.com/ZiminPark/coffee-augmented-rag/labels/RAG%20Evaluation%EC%9D%84%20%EA%B5%AC%EC%84%B1%ED%95%A0%20%EB%95%8C%20%EC%96%B4%EB%96%A4%20%EC%A0%90%EB%93%A4%EC%9D%84%20%EA%B3%A0%EB%A0%A4%ED%95%B4%EC%95%BC%ED%95%A0%EA%B9%8C

**Summary**  
- [rag-evaluation.md](./rag-evaluation.md)


# Long Context가 LLM에 들어갈 때 성능이 어떻게 변할까

**Reference**  
- [Lost in the Middle: How Language Models Use Long Contexts](https://arxiv.org/pdf/2307.03172)
- [Further Readings](https://github.com/ZiminPark/coffee-augmented-rag/issues/8)
<img width="577" alt="image" src="https://github.com/user-attachments/assets/96f92164-595a-43fe-9a72-8cbbaff28ec3">


**Question/ Discussion**  
https://github.com/ZiminPark/coffee-augmented-rag/labels/Long%20Context%EA%B0%80%20LLM%EC%97%90%20%EB%93%A4%EC%96%B4%EA%B0%88%20%EB%95%8C%20%EC%84%B1%EB%8A%A5%EC%9D%B4%20%EC%96%B4%EB%96%BB%EA%B2%8C%20%EB%B3%80%ED%95%A0%EA%B9%8C

**Summary**  
https://github.com/ZiminPark/coffee-augmented-rag/blob/main/lost-in-the-middle.md

# RAG+FT 어떻게 시너지 낼수 있을까

**Reference**  
- [RAFT: Adapting Language Model to Domain Specific RAG](https://arxiv.org/pdf/2403.10131), [code](https://github.com/ShishirPatil/gorilla/tree/main/raft)
<img width="940" alt="image" src="https://github.com/user-attachments/assets/3eb6e91e-ebdc-49d7-9df1-9d32ad81d739">


**Question/ Discussion**  
https://github.com/ZiminPark/coffee-augmented-rag/issues?q=is:issue+is:open+label:%22RAG+FT+%EC%96%B4%EB%96%BB%EA%B2%8C+%EC%8B%9C%EB%84%88%EC%A7%80+%EB%82%BC%EC%88%98+%EC%9E%88%EC%9D%84%EA%B9%8C%22


**Summary**  
- [raft.md](./raft.md)

# RAG를 할때 LLM parameter에는 무슨 일이 일어날까

**Reference**  
- [From RAGs to rich parameters: Probing how language models utilize external knowledge over parametric information for factual queries](https://arxiv.org/pdf/2406.12824)
<img width="828" alt="image" src="https://github.com/user-attachments/assets/e9e00a7c-79df-43a1-84da-3dfa7662199a">


**Question/ Discussion**  
- https://github.com/ZiminPark/coffee-augmented-rag/issues?q=is%3Aissue+is%3Aopen+label%3A%22RAG%EB%A5%BC+%ED%95%A0%EB%95%8C+LLM+parameter%EC%97%90%EB%8A%94+%EB%AC%B4%EC%8A%A8+%EC%9D%BC%EC%9D%B4+%EC%9D%BC%EC%96%B4%EB%82%A0%EA%B9%8C%22


**Summary**  
- [probing.md](./probing.md)

# Spreadsheet 데이터는 어떻게 인덱싱하는게 좋을까

**Reference**  
- [SpreadsheetLLM: Encoding Spreadsheets for Large Language Models](https://arxiv.org/pdf/2407.09025)
<img width="497" alt="image" src="https://github.com/user-attachments/assets/74e25a54-cbd6-48e0-8767-a278a7d14afb">


**Question/ Discussion**  
- https://github.com/ZiminPark/coffee-augmented-rag/issues?q=is%3Aissue+is%3Aopen+label%3A%22Spreadsheet+%EB%8D%B0%EC%9D%B4%ED%84%B0%EB%8A%94+%EC%96%B4%EB%96%BB%EA%B2%8C+%EC%9D%B8%EB%8D%B1%EC%8B%B1%ED%95%98%EB%8A%94%EA%B2%8C+%EC%A2%8B%EC%9D%84%EA%B9%8C%22


**Summary**  
- [Spreadsheets.md](./Spreadsheets.md)

# Graph RAG는 어떤 상황에서 효과적일까

**Reference**  
- [From Local to Global: A Graph RAG Approach to Query-Focused Summarization](https://arxiv.org/pdf/2404.16130)
<img width="1010" alt="image" src="https://github.com/user-attachments/assets/933f81bb-214e-458f-aa10-0a89b0bffa86">


**Question/ Discussion**  
- https://github.com/ZiminPark/coffee-augmented-rag/labels/Graph%20RAG%EB%8A%94%20%EC%96%B4%EB%96%A4%20%EC%83%81%ED%99%A9%EC%97%90%EC%84%9C%20%ED%9A%A8%EA%B3%BC%EC%A0%81%EC%9D%BC%EA%B9%8C


**Summary**  
- [graphrag.md](./graphrag.md)

# Citation을 어떻게 하는게 제일 효과적일까 & 평가할까

**Reference**  
- [Enabling Large Language Models to Generate Text with Citations](https://arxiv.org/pdf/2305.14627)
<img width="790" alt="image" src="https://github.com/user-attachments/assets/8f427ec5-5cec-49f4-90dd-e5d4aae00af5">


**Question/ Discussion**  
- https://github.com/ZiminPark/coffee-augmented-rag/issues?q=is%3Aissue+is%3Aclosed+label%3A%22Citation%EC%9D%84+%EC%96%B4%EB%96%BB%EA%B2%8C+%ED%95%98%EB%8A%94%EA%B2%8C+%EC%A0%9C%EC%9D%BC+%ED%9A%A8%EA%B3%BC%EC%A0%81%EC%9D%BC%EA%B9%8C+%26+%ED%8F%89%EA%B0%80%ED%95%A0%EA%B9%8C%22


**Summary**  
- [citation.md](./citation.md)
