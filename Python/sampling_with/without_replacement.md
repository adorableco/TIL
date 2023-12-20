<!-- @format -->

# 복원/비복원 추출로 샘플링하기

sampling with replacement (복원 추출)을 하려면

```python
random.sample(range(a,b),c)
```

**random.sample()** 을 이용한다.
<br/>
sampling without replacement (비복원 추출)을 하려면

```python
random.choices(range(a,b),k=c)
```

**random.choices()** 을 이용한다.
