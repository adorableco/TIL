<!-- @format -->

## collections.Counter()의 most_common()

- 빈도수가 높은 순서대로 아이템을 추출하는 기능


### 메서드

#### `subtract()`

- 두 Counter 객체나 iterable을 비교하여 값들을 뺄셈하는 역할

> #### 주요 특징
> 1.	음수 값을 허용합니다. 뺄셈 후 결과값이 음수가 될 수 있습니다.
> 2.	원본 Counter 객체가 변경됩니다.
> 3.	기존 Counter에 없는 키도 새로 추가될 수 있습니다(결과는 음수로 나타남).