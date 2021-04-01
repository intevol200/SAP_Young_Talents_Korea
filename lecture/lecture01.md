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

>REPORT ZBC100_27_TEST.  
>  
>PARAMETERS PA_NAME TYPE STRING.  
>  
>WRITE: 'HELLO WORLD',/ "안녕하세요  
>       'BYE', PA_NAME,/  
>\*       'TEST',/  
>       'TEST'.  

---
- SHIFT + F1: 대소문자 자동 변환
