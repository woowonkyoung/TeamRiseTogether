**미션 2: 대출/반납 기록을 로그 파일로 저장하는 기능 구현**
- **입력:**
    - 대출 또는 반납 거래 기록을 나타내는 문자열
- **기능:**
    1. 입력받은 거래 기록을 로그 파일(예: "transaction.log")에 추가(append) 모드로 저장한다.
    2. 파일 입출력 과정에서 발생할 수 있는 예외를 처리하며, 잘못된 파일 경로 등의 예외 상황에 대해 assertThrows를 이용한 테스트를 진행한다.
- **출력 예:**
    - "transaction.log" 파일에 대출/반납 기록이 추가되어 저장됨


**미션 2 (대출/반납 로그 파일 저장):**
1. `LogManager` 클래스를 정의하여:
    - `logTransaction(String record, String filePath)` 메서드 구현
    - 파일 입출력 시 발생하는 IOException을 try-catch로 처리한다.
2. main() 메서드에서 샘플 거래 기록을 이용하여 로그 파일 저장 기능을 시연한다.

## 나의 접근 방법

2. Member 클래스를 정의 
3. memberId , member name의 속성을 갖는다.
2. Book 클래스를 정의
3. Name,Author,Price 의 속성을 갖는다
3. BookRentManager 클래스를 정의
4. - BookRentManager에서 책 대출하는 메서드 구현
- >  전에 했던 방식으로 rent(String memberId,List<Book>)으로 구현
  > 
  --- 여기까지 전에 했던거 재사용---
  >
대출할때 즉시 파일에 기록
-- 이를위해 return 값을 전에 했던 함수(rentBook)에 String으로 넣어준다.

1. LogManager 클래스를 정의 로그를 기록할 메서드 logTransaction를 갖는다.
5.
6.  반납도 마찬가지로 구현.

- 파일 입출력 시 발생하는 IOException을 try-catch로 처리한다.
- 