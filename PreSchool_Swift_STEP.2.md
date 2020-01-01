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
```

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
