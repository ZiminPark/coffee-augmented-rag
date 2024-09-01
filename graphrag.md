1. 일반적인 RAG는 Corpora에 대한 Global한 질문을 처리할 수 없는 구조임. 예) “What are the main themes in the dataset?”

```
this is inherently a queryfocused summarization (QFS) task, rather than an explicit retrieval task.
```

2. 이전의 QFS는 Scale적으로 확장이 어려움.

3. Scale있게 QFS를 처리하는 방식 제안 -> GraphRAG
   <img width="716" alt="image" src="https://github.com/user-attachments/assets/fa52e51e-8b06-47cc-a17d-9fdb8033dfca">
