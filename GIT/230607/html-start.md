# html01 - start

## Code

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <h1>block_inline</h1>
    <h2>블록 요소</h2>
    <p style="background-color: beige;">줄바꿈</p>
    <div>
        블록 요소 안에 텍스트, <strong>인라인 요소</strong> 포함 가능
        <p>블록 요소 안에 블록 요소 포함 가능</p>
    </div>

    <hr>
    
    <a href="">줄바꿈X</a>
    <q style="background-color: black; color:white">인라인 요소 안에 텍스트와 <b>인라인 요소</b> 포함가능</q><br>
    <span>인라인 요소 안에 <p>블록요소</p> 포함 불가</span>
</body>
</html>
```
---
## Homepage

http://127.0.0.1:5500/web01-html/index.html
- 127.0.0.1:5500 -> ip:port
- 127.0.0.1 이라는 ip는 localhost(내컴퓨터, 나자신)라고 한다.
- http -> 요청하고 응답받기위한 통신 규약
- 127.0.0.1:5500 -> 나 자신에게 5500번 포트로 요청
- /(slash)는 하위 목록을 의미하고 하위 목록으로 요청한다는 의미
---

## ; (Semicolon)
- html에서 ; (Semicolon)는 다음 코드를 이어서 작성할 때 사용한다.
- 코드 마지막엔 당연히 안적어주어도 된다.
---

## ` <h1>&<br> `

```html
- <hr>은 한줄 그어지는 기능, <br>은 줄바꿈(enter)의 기능
- <hr>, <br>은 시작태그만 있고 끝 태그가 없다.
    - 시작태그와 끝태그가 하나로 합쳐져 있기 때문. 
    - 끝태그가 있었지만 html 5버전부터 끝태그(/)를 생략해도 되도록 바뀌었다.