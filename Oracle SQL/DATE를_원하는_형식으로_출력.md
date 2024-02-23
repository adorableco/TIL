<!-- @format -->

# DATE를 원하는 형식으로 출력하기

```sql
SELECT book_id, to_char(published_date,'yyyy-mm-dd')
from book
where to_char(published_date,'yyyy-mm-dd') like '2021-%' and category = '인문'
order by published_date asc;
```

`TO_CHAR(속성,'yyyy-mm-dd')` -> 날짜를 문자열로 변환해서 포맷을 지정함

- 조건에 부합하는 날짜를 찾을 때도 이렇게 변환을 해서 `LIKE` 로 비교해야 함!
