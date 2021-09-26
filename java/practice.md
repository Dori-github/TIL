# #12 객체와 프로퍼티
>## 객체 (object)
객체 : 여러가지 값을 한번에 저장하고 싶을 때 객체를 사용 

### 객체 만들기 
객체는 중괄호를 통해 만들 수 있음 { } 
```java
{   
    brandname: '김소희',
    bornYear: 1998,
    isVeryNice: true,
    woestCourse: null
}
```
여기서 값 이름은 key라고 하고, 값은 value 라고 한다.  
key와 value 를 합쳐서 **속성(property)** 라고 부른다.
그래서 값 이름을 property name , 값을 property value 라고 부르기도 한다.  

여기서 값 이름은 반드시 문자열로 작성해야 한다. ( 따옴표 생략하고 작성 가능 )

### property name 주의 사항
1. 첫 번째 글자는 반드시 문자, 밑줄(_), 달러 기호($) 중 하나로 시작 
2. 띄어쓰기 금지!
3. 하이픈(-) 금지!

이러한 것들을 어길 경우 따옴표르 감싸주어야한다.
