
## 1-1 Big Query 기초 지식 ~ 2-2 저장된 데이터 활용하기

### 데이터 베이스 저장 장소
- MYSQL, Oracle, PostgreSQL, AWS AUrora 등 회사마다 상이
  - 단, 이들은 모두 OLTP (거래를 하기 위한 데이터베이스)
  - 분석 속도 느릴 수 있음

- Big Query
  - OLAP(분석 기능 제공)이기에 추출과 분석 속도 빠르지만 비쌈
  - Firebase(웹 개발 시 사용), Google analytics4 사용하는 기업이 주로 사용. 해당 데이터 쉽게 추출 가능함
  - 클라우드 기반이기에 1) 쿼리비용 2) 저장 비용 존재
 
#### Big Qurey 구성요소

1. 프로젝트 2. 데이터셋 3. 테이블
   
---

### SQL로 데이터 다루는 파트
![image](https://github.com/user-attachments/assets/91b5c125-bed0-4a35-90aa-8a1f9d8c0f8b)


### SQL 쿼리 작성 전 생각할 것
1. 데이터가 어떻게 저장되어 있는가?
2. 어떤 데이터가 저장되어 있는가?
3. 컬럼의 의미는 무엇인가?


---
### ERD를 보면 데이터의 구조를 알 수 있음 (회사에 요청해보기)
![image](https://github.com/user-attachments/assets/d84f169b-cfe5-427f-9281-78f7f8d62d13)

 

> :bulb: 질문: 깃허브 파일명에 꼭 read.md를 붙여야 하는가

> :rocket: 느낀 점: 데이터베이스 관리론에서 학습한 개념들을 업무에서 어떻게 활용하는지, 그리고 **ERD(Entity-Relationship Diagram)**의 실무적 활용과 그 의미를 이해하게 되었다.


---
#### 학습 인증
![image](https://github.com/user-attachments/assets/a40c6eab-8e84-4303-8f7c-a9824a220b8b)


