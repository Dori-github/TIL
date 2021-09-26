

### [변수]
: 값을 저장하는 공간

애완동물을 소개해 주세요
```python
animal="강아지"

name = "공주"

age = 14

hobby = "산책"

is_adult = age >= 3

print("우리집 " + animal + "의 이름은 " + name + "에요")

#print(name + "는 " + str(age) + "살이며," + hobby + "을 아주 좋아해요")

print(name, "는 ", age, "살이며,", hobby, "을 아주 좋아해요")

print(name + "는 어른일까요? " + str(is_adult))
```

### [숫자 처리 함수]
```python
print(abs(-5)) # 5

print(pow(4, 2)) # 4^2 = 4*4 = 16

print(max(5, 12)) # 12

print(min(5, 12)) # 5

print(round(3.14)) # 3
```
```python
from math import *

print(floor(4.99)) # 내림. 4

print(ceil(3.14)) # 올림 .4

print(sqrt(16)) # 제곱근 . 4.0
```
### [랜덤 함수]

```python
from random import *

print(random()) # 0.0 ~1.0 미만의 임의의 값 생성

print(random() * 10 ) #0.0 ~ 10.0 미만의 임의의 값 생성

print(int(random() * 10)) #0 ~ 10 미만의 임의의 값 생성

print(int(random() * 10) +1) #1~10 이하의 임의의 값 생성

print(int(random() * 10) +1) #1~10 이하의 임의의 값 생성

print(int(random() * 10) +1) #1~10 이하의 임의의 값 생성

print(int(random() * 45) +1) #1~45 이하의 임의의 값 생성

print(randrange(1,46)) #1~ 46 미만의 임의의 값 생성
print(randint(1, 45)) #1~45 이하의 임의의값 생성
```
```python
from random import *

x = randint(4,28)

print("오프라인 스터디 모임 날짜는 매월 " + str(x)+ " 일로 선정되었습니다.")
```

###  [슬라이싱]
: 필요한 정보를 잘라서 사용하는 것

```python
jumin = "990120-1234567"

print("성별 : " + jumin[7])

print("연 :" + jumin[0:2]) # 0부터 2 직전까지 (0, 1)

print("월 :" + jumin[2:4])

print("일 :" + jumin[4:6])

print("생년월일 :" + jumin[:6]) #처음부터 6 직전까지

print("뒤 7자리 : " + jumin[7:]) #7부터 끝까지

print("뒤 7자리 (뒤에부터) :" + jumin[-7:]) #맨뒤에서 7번째부터 끝까지
```

### [문자열 포맷]

#### 방법1
```python
print("나는 %d살 입니다." %20) #정수값만 넣을 수 있음

print("나는 %s를 좋아해요." %"파이썬")

print("Apple 은 %c로 시작해요" %"A") #한글자만 넣을 수 있음

# %s는 다 쓸 수 있음

print("나는 %s색과 %s색을 좋아해요." %("파란", "빨간"))
```
  
#### 방법2
```python
print("나는 {}살입니다.".format(20))

print("나는 {}색과 {}색을 좋아해요.".format("파란", "빨간"))

print("나는 {1}색과 {0}색을 좋아해요.".format("파란", "빨간"))
```
#### 방법3
```python
print("나는 {age}살이며, {color}색을 좋아해요.".format(age = 20, color = "빨간"))
```
 
#### 방법4 (v3.6이상~)
```python
age = 30

color ="빨간"

print(f"나는 {age}살이며, {color}색을 좋아해요")
```
 ```python
url ="http://naver.com"

my_str = url.replace("http://", "")

my_str = my_str[:my_str.index(".")]

password = my_str[:3] + str(len(my_str)) + str(my_str.count("e")) +"!"

print("{0}의 비밀번호는 {1} 입니다. ".format(url, password))
```
  

### [리스트]
: 순서를 가지는 객체의 집합

  
```python
# 지하철 칸 별로 10명, 20명, 30명

  

subway = [10, 20, 30]

print(subway)

  

subway = ["유재석", "조세호", "박명수"]

print(subway)

  

#조세호씨가 몇번째 칸에 타고 있는가?

print(subway.index("조세호"))

  

# 하하씨가 다음 정류장에서 다음칸에 탐

subway. append("하하")

print(subway)

  

# 정형돈씨를 유재석 / 조세호 사이에 태워봄

subway. insert(1,"정형돈")

print(subway)

  

# 지하철에 있는 사람을 한 명씩 뒤에서 꺼냄

print(subway.pop())

print(subway)

  

#같은 이름의 사람이 몇명 있는지 확인

subway.append("유재석")

print(subway)

print(subway.count("유재석"))

#정렬도 가능

num_list = [5,2,4,3,1]

num_list.sort()

print(num_list)

  

#순서 뒤집기 가능

num_list.reverse()

print(num_list)

  

#모두 지우기

num_list.clear()

print(num_list)

#다양한 자료형 함께 사용

num_list =[5,2,4,3,1]

mix_list = ["조세호", 20, True]

  

#리스트 확장

num_list.extend(mix_list)

print(num_list)
```
