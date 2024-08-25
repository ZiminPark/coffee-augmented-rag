Spreadsheet의 데이터 구조는 독특하다. 2차원 grid인데 Layout이 자유롭다. Cell정보, 하이라이팅, 헤더 정보 등 담아야할것도 많다.
때문에 Spreadsheet 데이터를 LLM Task를 수행할 때 input으로 정제하기가 쉽지않다. 토큰수 제한도 있다.
이런 문제 때문에 Encoding 방법을 연구한다. 크게는 세 가지 모듈이 있다.
1. Structural-anchor based compression: 같은 테이블이라면 homogeneous할 것이다. 이를 기반으로 나눈다.
2. inverse index tranlation: value를 key로 key를 value로 바꾼다.
3. data format aware aggregation: 2의 key를 data format 기반으로 변환한다.

Encoding 방식이 효과적인지 확인하기 위해 1. Table Detection Task와 2. Spreadsheet QA로 확인해본다.
