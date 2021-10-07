# SQL Study
업무에 바로 쓰는 SQL 튜닝 스터디 


# MySql 
1. 주로 중첩 루프 조인 알고리즘으로 해결 
2. 필요한 DBMS를 설정해 사용 가능
3. 상대적으로 낮은 메모리 사용으로 저사양 PC에서도 손쉽게 설치 및 개발 가능  

# MySql, Oracle 구문 차이 

1. 값이 NULL인 경우 대쳇값 출력 

    MySql: IFNULL(열명, '대쳇값')
    Oracle: NVL(열명, '대쳇값')

2. 일부 분량만 제한적으로 출력  

    MySql: LIMIT 숫자

    ```sql
    SELECT col1
      FROM tab
     WHERE LIMIT 5;
    ```

    Oracle: ROWNUM <= 숫자 

    ```sql
    SELECT col1
      FROM tab
     WHERE ROWNUM <= 5;
    ```

3. 현재 날짜 

