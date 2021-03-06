# 람다함수 (lambda)

한 줄로 함수를 표현. 구성이 단순해 간단한 연산을 하는 데 사용됨.

- 기본구조 : lambda<인자>:<인자 활용 수행 코드>
- 람다 함수 전체를 소괄호로 감싸서 활용

``` )python
(lambda x,y : x*y*2)
```

- 람다 함수를 다른 변수에 할당하고, 이 변수를 함수명처럼 이용해 람다함수를 호출함
- 변수에 할당할 때에는 람다 함수 전체를 소괄호로 감싸지 않아도 됨. 

```python
lambda_function(변수명)=lambda<인자>:<인사 활용 수행 코드>(정의)
lambda_fuction(<인자>)(호출)
```

- ex.람다함수를 이용해 입력된 수의 제곱을 반환하는 코드 

```python
(lambda x:x**2)(3)
--> 9
```

- 여러 개의 인자를 입력 받아 연산 결과를 반환하는 함수 

```python
#x,y,z 라는 세 개의 인자를 받아, '2x+3y+z'연산의 결과를 반환 

mySimpleFunc = lambda x,y,z : 2*x + 3*y +z
mySimpleFunc(1,2,3)
----
11
```



# 내장함수

### 형변환함수

- 데이터의 형태(type)을 변환해야 하는 경우, 파이썬의 내장함수 활용 
- int() : 실수나, 문자열을 정수로 변환, 숫자 외의 문자가 포함되어있는 경우 오류가 발생.
- float() : 정수나, 문자열을 실수로 변환. 소수점 0.1의 자리로 변환됨
- str() : 정수나 실수를 문자열로 변환 
- type을 변경하는 함수 : list(), tuple(), set()
- bool() : True 혹은 False의 결과를 반환
  - 숫자를 인자로 bool함수 호출 : 0이면 False, 그 외에 숫자면 True
  - 문자열을 인자로 bool함수 호출 : 문자열이 있으면 True, 없으면 False
  - 파이썬에서 None, Null은 아무것도 없는 것으로 간주(False)
  - list, tuple, set 를 bool 함수로 호출, 항목이 있으면 True, 없으면 False
- 최소값과 최대값을 구하는 함수  min(), max()
  - list, tuple, set 의 항목이나 문자열에서 각각 최소값과 최대값을 반환 
  - 문자열비교 : 1st letter --> 2nd letter -->... 대문자가 소문자보다 큼. 문자열이 숫자보다 큼
- 절대값과 전체 핪을 구하는 함수 abs()
- 항목의 갯수를 구하는 함수 len()

