## 오버로딩 vs 오버라이딩

다형성을 나타내는 대표적인 예시!

### 오버로딩 (overloading)

- 같은 이름을 가진 메서드를 여러 개 두는 것
- 컴파일 중에 발생하는 **'정적'** 다형성임

```Java
public class Calculator {
    // 정수 두 개를 더하는 메서드
    public int add(int a, int b) {
        return a + b;
    }

    // 실수 두 개를 더하는 메서드 (오버로딩)
    public double add(double a, double b) {
        return a + b;
    }

    // 정수 세 개를 더하는 메서드 (오버로딩)
    public int add(int a, int b, int c) {
        return a + b + c;
    }
}
```

### 오버라이딩 (overriding)

- 주로 메서드 오버라이딩을 말함
    - 상위클래스로부터 상속받은 메서드를 하위 클래스가 재정의하는 것
- 런타임 중에 발생하는 **'동적'** 다형성임

```Java
class Animal {
    public void sound() {
        System.out.println("동물이 소리를 냅니다.");
    }
}

class Dog extends Animal {
    @Override
    public void sound() {
        System.out.println("멍멍!");
    }
}

public class Main {
    public static void main(String[] args) {
        Animal a = new Dog();
        a.sound();  // 출력: 멍멍!
    }
}
```
