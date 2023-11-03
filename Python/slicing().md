<!-- @format -->

# Slicing, Slice()

```python
a[start : end : step]
```

- **a** : 리스트나 문자열
- **start** : 시작 인덱스
- **end** : 종료 인덱스
- **step** : 보폭

a 의 인덱스 _start_ 부터 _end -1_ 까지의 원소를 슬라이싱한다.

```python
slice(start,end,step)
a[slice(start,end,step)]
```

위와 같이 함수를 이용해 슬라이싱 할 수도 있다.
