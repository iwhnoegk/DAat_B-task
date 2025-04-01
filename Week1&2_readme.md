## 2-3 SQL 핵심 문법

### Select col1, col2
* col AS 별명 << 별명 붙이기 가능
* 컬럼 선택
* * 선택 시 모든 컬럼 보이기

### FROM table
* 데이터 확인할 테이블 명시
* table AS 별칭 << 별명 붙이기 가능

### WHERE 
* 조건 설정
* col = 조건 (숫자는 그대로, 문자는" " 붙여서)

> 작성 할 때는 SELECT-FROM-WHERE 순서

## 2-4,5 SELECT, 집계 및 그룹화

현업에서는 컬럼의 의미를 파악해서 요구사항에 맞춰 추출하는 역량이 필요함!

### 집계함수 기본 문법

---
SELECT
${\textsf{\color{green}col1,co2}}$

집계함수
col2 AS
${\textsf{\color{red}cnt2}}$

From 

GROUP BY
${\textsf{\color{green}col1, col2}}$

Having
${\textsf{\color{red}cnt2}}$ >3

ORDER BY col1 순서

LIMIT 숫자 

---


> 순서 = desc (내림차순) osc(오름차순, 보통 디폴트값)
>
> (집계함수) 는 꼭 (Group by)와 함께 다님!! (집계 기준 있을 때)
> 
> select와 group by 뒤에 오는 컬럼이 일반적으로 동일

![image](https://github.com/user-attachments/assets/63f258a0-8e29-4971-a6a5-b41b9a69428c)

---

### Where vs Having

Where = 원본 테이블 컬럼에 바로 조건 설정하는 경우 (컬럼 선택에 조건)

Having = Group By의 짝꿍! 컬럼 기준으로 묶은 후 (새로 생성된 집계 함수 등의 컬럼에) 조건 설정하고 싶은 경우

> 서브쿼리로 작성할 수도 있으나, 쿼리문이 늘어남

---

### 2-6 연습문제

#### NULL

NULL 이란, 0 혹은 " "(공백)과 다름. 알 수 없다는 의미.

* WHERE IS NULL  / IS NOT NULL 문법 존재
* AND는 그대로 연결 시키면 됨
* OR 조건 => ( ) OR ( )


![image](https://github.com/user-attachments/assets/a16dc4aa-2273-4039-9ee7-d650a12e2657)

> 문제 풀 때 다음과 같이 정리한 후, 쿼리 짜기

 
#### IN ("000", "xxx")

OR 조건이 너무 길 경우, IN 안의 내용에 해당할 경우 추출

#### Like "파%" "%파%"

~~로 시작하는, ~~로 끝나는 ~~들어있는 것을 찾는 문법! ~~자리에 % 붙이기

#### GROUP BY ALL

기존 GROUP BY 뒤에 컬럼 적어줘야 했는데, 얘는 알아서 묶어줌

---

## 3-1 SQL 쿼리 잘 작성하기

![image](https://github.com/user-attachments/assets/d4d1616f-818c-402f-893e-ba1aaeb8bfbd)


## 3-3 쿼리 작성 템플릿과 생산성 도구

```
# 쿼리 작성하는 목표, 확인할 지표 :
# 쿼리 계산식 : 
# 데이터 기간 : 
# 사용할 테이블 :
# Join Key :
# 데이터 특징 :

SELECT

FROM
WHERE
```

> 해당 템플릿 작성하고 쿼리 쓰면 쉬움 !!
>
> 쿼리 작성 시에는 FROM WHERE SELECT 순으로 !!
> 
> 이를 위한 생산성 도구 ? ** Espanso **
 



