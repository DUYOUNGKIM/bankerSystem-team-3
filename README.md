# bankerSystem-team-3
설계
 
< 1일차 은행 관리프로그램 > < 필수사항 >
1.화면구상

1-1시작
  1. 관리자 2. 고객 3. 종료

1-2은행
  1.계좌등록 2. 계좌관리(수정) 3. 계좌관리(삭제) 4. 계좌검색(소유자명) 5. 모든 계좌 조회 6.종료

1-3고객
  1.입금 2.출금 3.잔고확인 4. 종료 
  
2. 시작: 관리자와 고객인지 구분한다. 관리자 선택시 비번입력을 통과해야 이동한다. 고객일 경우 계좌번호와 비밀번호를 입력하여 통과한다.

3.계좌등록 : 이름, 비밀번호, 계좌번호를 스캐너를 통해 입력. 1건의 글 생성 및 뱅크 리스트에 저장/계좌번호는 중복성 검사를 통해서 없을때는 바로 저장 /있다면 다시 계좌번호 작성란으로 돌아가며 중복된 계좌번호 입니다를 띄워준다.
          
4.계좌관리(수정) : 수정할 계좌번호 입력받기or받기/ 수정할 계좌번호의 비밀번호 입력받기 / 비밀번호 일치 : 비밀번호 수정 / 일치하지 않음:  일치 하지 않는다는 메시지 출력

5.계좌관리(삭제) : 삭제할 계좌번호 입력받기or받기/ 삭제할 계좌번호의 비밀번호 입력/ 비밀번호 일치 : 계좌번호 삭제/ 일치하지 않음 : 일치 하지 않는다는 메시지 출력

6. 입금 : 입금할 계좌번호 입력받기or받기/ 계좌번호가 있음: 입금 -> 잔고 변경/계좌번호가 없음 :계좌번호가 없다는 메시지 출력

7. 출금 : 출금할 계좌번호 입력받기or받기/ 
계좌번호가 있음 : 출금할 계좌번호의 비밀번호 입력받기 -> 비밀번호 일치 :  출금->잔고변경  /비밀번호 일치하지 않음: 일치 하지 않는다는 메시지 출력
계좌번호가 없음 : 계좌번호가 없다는 메시지 출력

8.은행(bank) 고객 한명에 대한 정보를 가진 은행 클래스는 (생성 번호,) 작성자이름, 비밀번호, 계좌번호, 계좌생성일(컴퓨터 시스템의 날짜와 시간을 자동저장) 계좌 비밀번호 수정 시 수정시간으로 시간이 변경된다.
생성번호와, 잔고는 넣을지 말지 회의하고 진행

9.뱅크리스트(bankList) 여러건의 은행에 계좌를 만들 사람들의 정보를 저장하는 클래스이다. getter, setter가 있다.
만들면서 계좌에 고객 리스트를 같이 만들지 회의 하면서 결정

10.고객(customer) 고객의 한 줄에 대한 정보를 가진 고객 클래스는 (생성번호,) 거래 일자, 거래 시간, 계좌번호, 입금/출금 여부, 거래 금액, 은행명이다.

11.고객리스트(costomerList) 고객의 입, 출금 잔고 정보를 저장하는 리스트 이다. getter, setter가 있다.

12.메인(main) 회의 후 완성후 분리 할 것인지 처음부터 분리 할 것인지 그냥 메인에 입출력 조건을 다 적어둘지 결정

13. 여러 인터페이스 다 넣을지 이런식으로 다나눌것인지 내일 다 있을 때 결정

get으로 했다가 빨리 끝나 시간이 남는다면 바이너리 서치 검색으로 바꿔서 비교해보기
