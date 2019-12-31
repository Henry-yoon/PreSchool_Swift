# PreSchool_Swift_STEP.1 : 구구단
## 1. 개발환경 경험하기

### Xcode 설치
- 스위프트(Swift)란? Apple에서 개발한 iOS용 개발 언어
- 소프트웨어 개발 도구(Software Development Kit, 이하 SDK)란? 소프트웨어 개발 도구 (Swift: Xcode / Java: Eclipse..)
- Xcode란? Playground란? Swift용 개발 도구, Xcode의 기능 중 하나가 Playground(간편 개발 도구)
- 운영체제(Operating System, 이하 OS)란? 메모리 & 비메모리 하드웨어를 제어하는 소프트웨어

### Hello World 소스 코드 구현 및 실행
소스 코드는? 기계어를 프로그래밍 언어로 작성한 코드
컴파일이란? 실행이란? 작성한 프로그래밍 언어는 컴파일러를 통해 어셈블리어(기계어)로 번역된다.
입력이란? 출력이란? Data Input Output

### github 저장소
github이란? 개발자들을 위한 원격 저장소, 협업을 가능하게 하여 오픈소스를 만들도록 하는 서비스 플랫폼(서버)
git이란? 프로그램 등의 소스 코드 관리를 위한 버전 관리 프로그램
commit이란? 프로그래밍 파일 등에 대한 추가/변경 사항을 저장소에 기록
push란? 컴퓨터 저장소와 원격 저장소(github) 연결

### 기타
위키란? 프로젝트의 매뉴얼 등이 저장 되어 있는 곳
markdown의 용도는? 문법과 관리가 쉬워 매뉴얼 등 작성에 용의
read.md 파일은? 해당 프로젝트에 대한 기본적인 매뉴얼이 담기는 곳

## 2. 2,3단 계산과 출력
### 요구사항
구구단 중에서 2단과 3단 값을 한 줄씩 직접 계산해서 화면에 출력한다.
예를 들어 2단은 2 곱하기(x) 1 계산후 계산 값을 출력하고, 다음 줄에서 2 곱하기 2 계산 하고 계산 값을 출력한다.
이렇게 2 곱하기 9까지 반복한다.
3단은 혼자서 위와 같은 과정을 직접 입력해서 출력한다.

```
import Foundation

print("2단")
print("2 * 1 =",2*1)
print("2 * 2 =",2*2)
print("2 * 3 =",2*3)
print("2 * 4 =",2*4)
print("2 * 5 =",2*5)
print("2 * 6 =",2*6)
print("2 * 7 =",2*7)
print("2 * 8 =",2*8)
print("2 * 9 =",2*9)

print("3단")
print("3 * 1 =",3*1)
print("3 * 2 =",3*2)
print("3 * 3 =",3*3)
print("3 * 4 =",3*4)
print("3 * 5 =",3*5)
print("3 * 6 =",3*6)
print("3 * 7 =",3*7)
print("3 * 8 =",3*8)
print("3 * 9 =",3*9)
```
## 3. 4,5단 입력과 변수
### 요구사항
구구단에서 4단과 5단을 계산한 결과 값을 변수에 저장한 후 저장한 변수 값을 출력한다.
4단, 5단에서 4와 5 값은 한 번 결정하면 출력하는 동안 바뀌지 않고 반복되는 값이다. 따라서 4단과 5단에 해당하는 상수값으로 만든 후 프로그램을 구현한다.
예를 들어 4단은 4 곱하기 1 계산 결과 값을 i라는 변수에 저장하고, i라는 변수에 저장한 결과 값을 출력한다.
4단을 위해서 한 번 선언한 변수에 값을, 5단에서 바꾸고 5단을 출력한다.

```
import Foundation

var number = 4
var result = number * 1

print("4단")
print("4 * 1 =",result)
result = number * 2
print("4 * 2 =",result)
result = number * 3
print("4 * 3 =",result)
result = number * 4
print("4 * 4 =",result)
result = number * 5
print("4 * 5 =",result)
result = number * 6
print("4 * 6 =",result)
result = number * 7
print("4 * 7 =",result)
result = number * 8
print("4 * 8 =",result)
result = number * 9
print("4 * 9 =",result)

print("5단")
number = 5
result = number * 1
print("5 * 1 =",result)
result = number * 2
print("5 * 2 =",result)
result = number * 3
print("5 * 3 =",result)
result = number * 4
print("5 * 4 =",result)
result = number * 5
print("5 * 5 =",result)
result = number * 6
print("5 * 6 =",result)
result = number * 7
print("5 * 7 =",result)
result = number * 8
print("5 * 8 =",result)
result = number * 9
print("5 * 9 =",result)
```

## 4. 6,7단 반복문
### 요구사항
지금까지 2 ~ 5단까지 구현하기 위해 단순, 반복적인 작업이 많았다.
이 같은 단순, 반복적인 작업을 변수와 반복문을 활용해 제거하면서 6단과 7단을 구현한다.

```
import Foundation

var number = 6
var i = 1
var result = number * i

print("6단")
while(i<10){
    result = number * i
    print(number, "*", i, "=", result)
    i=i+1
}

print("7단")
number = 7
for i in 1..<10{
    result = number * i
    print(number, "*", i, "=", result)
}
```

## 5. 8,9단 조건문과 2중 반복문
### 요구사항
반복문을 사용해 2단과 9단에 대한 중복을 제거한다.
구구단 중에서 홀수단(1,3,5,7,9단)만 출력하도록 개선한다.

```
import Foundation

var number = 1
var result = number * 1

for i in 1..<10 {
    number = i
    if(number%2==1){
        print(number,"단")
    }
    for j in 1..<10{
        if(number%2==1){
            result = number * j  
            print(number, "*", j, "=", result)
        }
    }
}
```
## 6. 배열과 서브루틴
### 요구사항
구구단 2단 결과를 배열에 저장하고, 배열의 결과를 출력한다.
반복되는 코드를 서브루틴으로 만들어서 함수 단위로 호출하도록 개선한다.
서브루틴을 활용해서 구구단 1단부터 9단까지 전체를 출력한다.

```
import Foundation

var number = 2
var result = number * 1
var gugudan = [Int].init(repeating: 0, count: 9)
//var gugudan : Array<Int> = Array<Int>()
//var gugudan = [Int]()

for i in 1..<10 {
    result = number * i     
    gugudan[i-1] = result
}

print(gugudan)
```

```
import Foundation

var number = 2
var result = number * 1
var gugudan = [Int].init(repeating: 0, count: 9)
//var gugudan : Array<Int> = Array<Int>()
//var gugudan = [Int]()

func gugu(number1 : Int, number2 : Int){
    result = number1 * number2     
    gugudan[number2-1] = result
    print(number1, "*", number2, "=", gugudan[number2-1])
}

for i in 1..<10 {
    print(i,"단")
    for j in 1..<10{   
        gugu(number1: i, number2: j)
    }
}
```
