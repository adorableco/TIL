<!-- @format -->

# public 폴더 내의 이미지가 뜨지 않을 때

```css
<img src ='원래 경로'>
```

src 자리에 원래 경로 대신
<br/>

```css
<img src =src={process.env.PUBLIC_URL + "원래 경로"}>
```

를 사용한다.
