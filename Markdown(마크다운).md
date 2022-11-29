## 마크다운이란?
  -  Markdown은 텍스트 기반의 마크업언어로 2004년 존그루버에 의해 만들어졌으며 쉽게 쓰고 읽을 수 있으며 HTML로 변환이 가능하다.  
깃헙의 저장소에 관한 정보를 기록하는 README.md는 github를 사용하는 사람이라면 누구나 가장 먼저 접하게 되는 마크다운 문서다.  
마크다운을 통해서 설치방법, 소스코드 설명, 이슈 등을 간단하게 기록하고 가독성을 높일 수 있다는 강점이 부각되면서 점점 여러 곳으로 퍼져가게 된다.

## 마크다운의 장·단점
  ### 장점
    1. 간결하다.
    2. 별도의 도구없이 작성가능하다.
    3. 다양한 형태로 변환이 가능하다.
    4. 텍스트(Text)로 저장되기 때문에 용량이 적어 보관이 용이하다.
    5. 텍스트파일이기 때문에 버전관리시스템을 이용하여 변경이력을 관리할 수 있다.
    6. 지원하는 프로그램과 플랫폼이 다양하다.
   ### 단점
    1. 표준이 없다.
    2. 표준이 없기 때문에 도구에 따라서 변환방식이나 생성물이 다르다.
    3. 모든 HTML 마크업을 대신하지 못한다.
    
## 사용법
  ### 1. 헤더(머릿말)
    - 문장 앞에 `#`을 넣어서 사용하며, `#`의 갯수에 따라 글자의 크기가 달라지며, 사용시 `#` 입력 후 한칸 띄어쓰기 해야 적용된다. 6개 까지 지원한다.  
# 1개
## 2개
### 3개
#### 4개
##### 5개
###### 6개
####### 7개
  ### 2. Block Quote
    - 이메일에서 사용하는 > 블럭인용문자를 이용한다.
> 인용문자 1개
>	> 인용문자 2개
>	>	> 인용문자 3개

## 2. 목록
  ### 순서O
    - 순서가 있는 목록은 숫자와 점을 사용한다.
1. 첫번째
2. 두번째
3. 세번째
  ### 순서X
    - 순서가 없는 목록은 '+', '-', '*' 를 이용한다. 세 기호 모두 결과는 같다. 혼합해서 사용도 가능하다.
* `*`사용
  + 들여쓰기 후 `+`사용
    - 두 번 들여쓰기 후 `-`사용  
## 3. 코드
4개의 공백 또는 하나의 탭으로 들여쓰기를 만나면 변환되기 시작하여 들여쓰지 않은 행을 만날때까지 변환이 계속된다.

### 들여쓰기
```
This is a normal paragraph:

    This is a code block.
    
end code block.
```

실제로 적용해보면,

적용예:

*****
This is a normal paragraph:

    This is a code block.

end code block.
*****

> 한줄 띄어쓰지 않으면 인식이 제대로 안되는 문제가 발생한다.

```
This is a normal paragraph:
    This is a code block.
end code block.
```

적용예:

*****
This is a normal paragraph:
    This is a code block.
end code block.
*****

## 3.1 코드블럭
코드블럭은 다음과 같이 2가지 방식을 사용할 수 있다:

* `<pre><code> {code} </code></pre>` 이용방식

```
<pre>
<code>
public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, Honeymon");
  }

}
</code>
</pre>
```

<pre>
<code>
public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, Honeymon");
  }
}
</code>
</pre>

* 코드블럭코드("\```") 을 이용하는 방법

<pre>
<code>
```
public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, Honeymon");
  }
}
```
</code>
</pre>

```
public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, Honeymon");
  }
}
```

**Github**에서는 코드블럭코드("\```") 시작점에 사용하는 언어를 선언하여 [문법강조(Syntax highlighting)](https://docs.github.com/en/github/writing-on-github/creating-and-highlighting-code-blocks#syntax-highlighting)이 가능하다.

<pre>
<code>
```java
public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, Honeymon");
  }
}
```
</code>
</pre>

```java
public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, Honeymon");
  }
}
```


## 2.5. 수평선 ```<hr/>```
아래 줄은 모두 수평선을 만든다. 마크다운 문서를 미리보기로 출력할 때 *페이지 나누기* 용도로 많이 사용한다.
