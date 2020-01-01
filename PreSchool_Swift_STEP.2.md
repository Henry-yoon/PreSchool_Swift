# PreSchool_Swift_STEP.2 : 단위변환기
## 1. 문제 설명

## 2. 길이변환 - 출력
### 요구사항
- ithub 저장소를 만들고 템플릿을 선택하고 새 프로젝트를 생성해서 저장소에 연결한다.
- 다음의 센티미터(cm) 단위 값을 미터(m) 단위로 변환해 결과 화면에 출력한다.
- 예를 들어 "120cm"을 "1.2m"로 출력한다.
- 미터(m) 단위 값을 센티미터(cm) 단위로 변환해 결과 화면에 출력한다.
- "1.86m"를 "186cm"로 출력한다.
```
import Foundation

var centimeter: Int = 120
var meter: Double = Double(centimeter)/100

print(centimeter, "cm ==", meter, "m")

meter = 1.86
centimeter = Int(meter*100)

print(centimeter, "cm ==", meter, "m")
```

## 3. 함수
### 요구사항
- 센티미터 단위 값을 변수에 저장하고 변환하는 데 사용한다.
- 센티미터 단위 값을 저장한 변수를 미터 단위 값으로 변환한 후 변수에 저장하고 저정한 변수 값을 출력한다.
- 길이 단위를 바꿀 때 곱하거나 나누는 값은 바뀌지 않는 값이다. 따라서 상수 값으로 지정해서 프로그램을 구현한다.
- 문자열로 값 뒤에 붙어있는 단위에 따라 길이를 변환해서 결과를 출력하는 함수를 만든다.
- 예를 들어 "183cm"처럼 숫자 다음에 cm가 붙어있으면 센티미터 값을 미터로 변환하고 출력한다. "3.14m"처럼 숫자 다음에 m가 붙어있으면 미터 값을 센티미터로 변환하고 출력한다.
```
import Foundation

let inputNumber = "183cm"
let inputNumber2 = "3.14m"

func meterConversion(_ inputData: String) -> String{    // FROM: CM -> TO: M 
    var convertUnit: String
    var calProcess: Double
    var result: String

    convertUnit = inputData.replacingOccurrences(of: "cm", with: "")
    calProcess = Double(convertUnit)!  // !의 의미는..? 없으면 왜 오류가 나는지..?
    calProcess = calProcess/100

    result = String(calProcess) + "m"

    return result
}

func centimeterConversion(_ inputData: String) -> String{    // FROM: M -> TO: CM 
    var convertUnit: String
    var calProcess: Double
    var calProcess2: Int
    var result: String

    convertUnit = inputData.replacingOccurrences(of: "m", with: "")
    calProcess = Double(convertUnit)!  // !의 의미는..? 없으면 왜 오류가 나는지..?
    calProcess2 = Int(calProcess*100)   // 자료형 한번 선언하면 못바꾸는지..? calProcess = Int(calProcess*100) 시 error

    result = String(calProcess2) + "cm"

    return result
}

print(meterConversion(inputNumber))
print(centimeterConversion(inputNumber2))
```

## 4. 값 입력
### 요구사항
```

```

## 5. 인치길이 변환
### 요구사항
```

```

## 6. 야드길이 변환
### 요구사항
```

```
