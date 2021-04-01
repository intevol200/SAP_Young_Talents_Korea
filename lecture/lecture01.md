__개발 과정__
1. DEV
2. QA
3. PRD

- CTS(Change Transport System): 프로그램을 개발할 때 통합하기 위해 다음 단계로 넘기는 것
- 패키지: 의미있는 기능을 가진 단위
- 프로그램

---
- 네이밍 규칙
  - X-: 공식적인 개발
  - Y-: 비공식적 개발(테스트 등)
  - 기타의 경우는 자신만의 네이밍 규칙을 만들어 개발

---
__CTS(SE09) 작성법__
1. TRANSPORT ORGANIZER
2. WORKBENCH REQUEST
3. CREATE
4. SHORT DESCRIPTION 입력

---
__PACKAGE(SE80) 작성법__
1. SELECT CATEGORY (PACKAGE)
2. ENTER PACKAGE NAME
3. ENTER

---
__PROGRAM 작성법__
1. CREATE PROGRAM
2. ENTER PROGRAM NAME
3. SELECT TYPE
4. SAVE

>REPORT ZBC100_27_TEST.  
>WRITE 'HELLO WORLD'.  
>WRITE 'TEST'.

>WRITE: 'HELLO WORLD',  
>       'TEST'.

| 단축키 | 기능 |
|---|---|
| CTRL + S | SAVE |
| CTRL + F2 | SYNTAX CHECK |
| CTRL + F3 | ACTIVATE |
| F8 | DIRECT PROCESSING |

---
__주석__
- 주석: "
- 한줄 주석: *
- 전체 주석: CTRL + <
- 주석 해제: CTRL + >

>REPORT zbc100_27_test.  
>  
>PARAMETERS pa_name TYPE string.  
>  
>WRITE: 'HELLO WORLD',/ "안녕하세요  
>       'BYE', pa_name,/  
>\*       'TEST',/  
>       'TEST'.  

---
- SHIFT + F1: 대소문자 자동 변환

---
__TEXT ELEMENT 입력__
1. GOTO
2. TEXT ELEMENTS
3. SELECT TEXTS

- 시스템 언어별 번역
1. GOTO
2. TRANSLATION
3. SELECT TARGET LANGUAGE
4. ENTER TRANSLATED LANGUAGE 

---
__데이터 타입__
| TYPE | 의미 | 사용 |
|---|---|---|
| string | 가변 문자열 | 어떤 문자도 입력 가능 |
| c | 고정 문자열 | 정해진 길이만큼 입력 가능 |
| d | 날짜 | YYYYMMDD |
| t | 시간 | HHMMSS |
| i | 정수 | 정수만 입력 가능 |
| p | 실수 | 소숫점자리 표현 가능 |


>REPORT zbc100_27_hello.  
>  
>PARAMETERS: pa_num1 TYPE i,  
>            pa_num2 TYPE i.  
>  
>DATA gv_result TYPE p LENGTH 16 DECIMALS 2.  
>  
>gv_result = pa_num1 * pa_num2.  
>  
>WRITE: 'result: ', gv_result.  

---
__전역 변수__
- PARAMETERS pa_mat TYPE mara-matnr.  
MARA 테이블에 있는 MATNR 변수를 불러와 pa_mat이라는 이름의 변수로 사용함

- DATA gv_var2 LIKE gv_var1.  
다른 변수에서 사용된 type 형태를 불러와 다른 변수의 type으로 사용

__변수 선언__
- DATA gv_text TYPE string VALUE 'ABC'.  
기본값으로 "ABC"를 입력

