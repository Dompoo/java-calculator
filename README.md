# 문자열 덧셈 계산기

### 목표 시간
- 기능 구현 목록 작성 1시간
- 기능 구현 3시간
- 도메인 단위테스트 작성, 기본 테스트 추가 작성 1시간

### 실제 시간

# 기능 구현 목록

## 입력
- [x] 사용자로부터 덧셈할 문자열을 입력받는다.
  - [x] 구분자는 한개씩만 존재해야 한다. (1::3은 예외가 발생한다.)
  - [x] 커스텀 구분자가 지정되어 있다면 이를 포함하여 입력받는다.
  - [x] 공백이 있다면 모두 삭제한다.

## 출력
- [x] 처음에 입력을 받기 위한 메시지를 출력한다.
- [x] 계산이 종료된 후, 결과값을 출력한다.

## 도메인

### 기본 구분자
- [x] :와 ,로 생성된다.

### 커스텀 구분자
- [x] 문자열을 통해 커스텀 구분자를 추출하여 생성된다.
  - [x] //과 \n 사이의 문자들이 모두 생성된다.
  - [x] 숫자가 포함되어 있으면 예외를 발생시킨다.

### 구분자들
- [x] 구분자를 등록하여 들고 있는다.
  - [x] 기본 구분자와 커스텀 구분자를 등록한다.
- [x] 문자열을 통해 숫자 값들을 추출한다.
  - [x] 등록되지 않은 구분자 발견시 예외가 발생한다.

### 계산기
- [x] 숫자 값들을 모두 더하여 반환한다.
- [x] 숫자 값들에 음수가 포함되어 있으면 예외가 발생한다.

## 프로그램 흐름
- [x] 사용자가 잘못된 값을 입력한 경우 예외 메시지를 출력하고 애플리케이션을 종료시킨다.