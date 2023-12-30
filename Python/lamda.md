<!-- @format -->

## 람다 표현식

### 간단한 함수를 쉽게 선언하는 방법

```python
s.sort(key = lamda x: (x.split()[1], x.split()[0]))
```

➡️ `x.split()` 의 인덱스 1 을 기준으로 정렬하고, 같을 경우 x.split()[0] 을 기준으로 정렬한다.

같은 것을 함수로 표현하면,

```python
def func(x):
    return x.split()[1], x.split()[0]

s.sort(key=func)
```
