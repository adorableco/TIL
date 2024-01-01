<!-- @format -->

### `sorted()` 와 `sort()` 의 주요 차이점

- `sorted()` 는 정렬 결과를 별도로 리턴하고 `sort()` 는 리턴 값이 없으며 입력을 정렬 결과로 덮어 쓴다.

</br>

### `sorted()` 의 key 옵션

- key = 옵션을 지정해 정렬을 위한 키 또는 함수를 별도로 지정할 수 있음

ex)

```python
c = ['ccc','aaaa','d','bb']
print(sorted(c, key=len))

# ['d','bb','ccc','aaaa']
```

- 길이 순으로 정렬됨
