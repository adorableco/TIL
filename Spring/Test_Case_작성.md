<!-- @format -->

```java
    @Test
    public void save(){
        Member member = new Member();
        member.setName("Spring");

        repository.save(member);

        Member result = repository.findById(member.getId()).get();
        Assertions.assertThat(member).isEqualTo(result);
    }
```

- Test 메서드 위에는 `@Test` 어노테이션 표기

</br>

### Assertions

- 내가 가정하고 있는 사실이 실제와 같은지 명시할 수 있는 도구

```java
Assertion.assertThat(expected,actual)
```

➡️ **JUnit** 메서드로, expected 와 actual 가 같은지 비교
✅ 순서 유의해야 함 !!!!
</br>

```java
Assertion.assertThat(actual).isEqualTo(expected)
```

➡️ **AssertJ** 메서드로, 마찬가지로 expected 와 actual이 같은지 비교 ( _실제값_ 이 내가 생각한 _예상값_ 과 같은가? ➡️ 이 순서로 변수 입력)

</br></br>

### ✅ 테스트 클래스를 전체 실행할 때, 메서드가 내가 작성한 순서대로 돌아가는 것이 아님!!!

</br></br>

```java
    @AfterEach
    public void afterEach(){
        repository.clearStore();
    }
```

➡️`@AfterEach` 어노테이션을 붙여서 각 메서드가 실행되고 난 후 바로 실행될 메서드를 작성해서 오류 해결!
