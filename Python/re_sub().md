<!-- @format -->

## re.sub()

### 정규표현식을 이용할 땐 **re** 모듈 사용

```python
re.sub(pattern,replace,text)
```

➡️ `text` 중에서 `pattern` 에 해당하는 부분을 `replace`로 대체한다.

| 패턴 | 내용                      | ex                           |
| ---- | ------------------------- | ---------------------------- |
| ^    | 이 패턴으로 시작해야 함   | ^abc : 'abc'로 시작하는 패턴 |
| $    | 이 패턴으로 종료되어야 함 | $wer : 'wer'로 끝나는 패턴   |

</br>

✅ `s = re.sub('[^a-z0-9]','',s)`

❌ `s = re.sub([^a-z0-9],'',s)`

- pattern 도 문자열이니 따옴표를 잊으면 안된다.

</br></br>

참고 : https://jjuha-dev.tistory.com/entry/Python-%EC%A0%95%EA%B7%9C%ED%91%9C%ED%98%84%EC%8B%9D-resub%EC%9D%84-%EC%9D%B4%EC%9A%A9%ED%95%9C-%EB%AC%B8%EC%9E%90%EC%97%B4-%EC%B9%98%ED%99%98%ED%95%98%EA%B8%B0
