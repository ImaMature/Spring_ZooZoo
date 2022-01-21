# 주주클럽  
경기도 유기동물, 분양서비스 커뮤니티

조장 - 강보균  
조원 - 장용범, 장희동, 최병호

제20조(동물의 소유권 취득) 시ㆍ도와 시ㆍ군ㆍ구가 동물의 소유권을 취득할 수 있는 경우는 다음 각 호와 같다.  
<개정 2013. 4. 5., 2017. 3. 21.>

1. 「유실물법」 제12조 및 「민법」 제253조에도 불구하고 제17조에 따라 공고한 날부터 10일이 지나도 동물의 소유자등을 알 수 없는 경우

2. 제14조제1항제3호에 해당하는 동물의 소유자가 그 동물의 소유권을 포기한 경우

3. 제14조제1항제3호에 해당하는 동물의 소유자가 제19조제2항에 따른 보호비용의 납부기한이 종료된 날부터 10일이 지나도 보호비용을 납부하지 아니한 경우

4. 동물의 소유자를 확인한 날부터 10일이 지나도 정당한 사유 없이 동물의 소유자와 연락이 되지 아니하거나 소유자가 반환받을 의사를 표시하지 아니한 경우


파일명 : ex) NewClass (파스칼)
url 규칙 : @RequestMapping 안씀
	goToUpdate : 이동만
	UpdateController : 컨트롤러
프로젝트명 : ZooZooClub
메소드명 : 파스칼
변수명 : 카멜
디비명 : zoozooclub(mysql)
디비 테이블명 : 소문자(개별)
이외 규칙은 상의를 통해 결정

------------------------------------------
뱃지
	- 여러 카테고리
메인 공지
친구
	- 쪽지 / 대화(1:1)
헤더 브금
국세청 사업자 진위확인 조회
카드
모달
sns 연동 가입
다크모드
애드센스
후원
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
회원 
	- 일반회원
		- 번호(PK)
		- 이름
		- 아이디
		- 비번
		- 폰번호
		- 주소
		- 이메일
		- 가입일
		- 생년월일 / 주민번호
	- 기업회원
		- 번호(PK)
		- 이름
		- 아이디
		- 비번
		- 폰번호
		- 사업자등록번호
		- 상호명
		- 사업장주소
		- 사업장연락번호
		- 가입일
		- 이메일

-----------------------------------------------------
유기
	- 번호(PK)
	- 제목
	- 내용
	- 파일
	- 등록일자
	- 조회수
	- 일반회원번호 (FK - 일반회원)

-----------------------------------------------------
분양
	- 번호(PK)
	- 제목
	- 내용
	- 파일
	- 등록일자
	- 조회수
	- 기업회원번호(FK - 기업회원)

----------------------------
병원
	- 댓글 번호(pk)
	- 작성자
	- 댓글 내용
	- 댓글 등록일자
	- 번호(fk)

------------------------------
자랑
	- 번호(PK)
	- 제목
	- 내용
	- 파일
	- 조회수
	- 등록일자
	- 일반회원번호(FK)

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
1. 유기 커뮤니티 --보류-------------------------------------------------------------------------------------------------------------------------------------------------------
개인이 유기동물을 습득한 경우
10일간 메인에 공지
후 분양인 나타나면 개인간 분양
	- 분양 과정 중 현물이 오고가는 경우 범법임을 공지
	- 게시물 등록 시 현물에 대한 키워드 지정(고밥비, 책임비, 장난감비), 등록불가처리
안나타나면 보호소 연결
	- 게시글을 등록한 회원의 정보를 받아와 회원에게 쪽지나 개인적인 연락을 할 수 있는 터를 통해 보호소 연결 및 분양 의사 확인 후 연계 또는 방치
	- 보호소 리스트를 볼 수 있는 페이지 -> 보호소 정보를 볼 수 있는 상세페이지

-----------------------------------------------------------------------------------------------------------------------------------------------------------------

2. 분양 커뮤니티--보류---------------------------------------------------------------------------------------------------------------------------------------------------
	- 기업회원 / 일반회원
		- 기업회원은 분양 커뮤니티(소개글)에 글 등록 가능 / 일반회원은 불가능
		- 기업 회원가입 할 때 사업자 등록증, 신분증, 사업자 등록번호 등 판별 필요
		- 직접적인 금액은 암시 또는 명시 금지
		- 펫샾에서 따로 운영중인 웹이 있다면 링크를 걸어주기
		- 해당 업체에서 분양중인 동물 종, 사진 명시
		- 펫샾 리스트페이지 -> 펫샾 상세정보

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

3. 동물병원 커뮤니티--병호--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
	- 리뷰 / 후기
	- 회원 주소에 맞는 병원 추천?

4. 자랑(일상공유/아이들사진) 커뮤니티--희동이 회원 끝내고 투입 ------------------------------------------------------------------------------------------------------------------------------------
	- 사실상 sns

## ERD
![springdb](https://user-images.githubusercontent.com/87436495/150328430-bf0783b7-b791-406b-b0e9-879cfca1ab90.png)
