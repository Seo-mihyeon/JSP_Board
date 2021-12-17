# JSP_Board

### 기능구현
1. 회원가입
2. 로그인
3. 게시판 글 작성
4. 게시판 글 수정
5. 게시판 글 삭제

#### DB 생성하기
create database (테이블명);
= create database bbs;

#### DB 사용하기
use (테이블명);
use bbs;

#### 테이블정의
1. user
```sql
CREATE TABLE USER (
    userID VARCHAR(20),
    userPassword varchar(20),
    userName varchar(20),
    userGender varchar(20),
    userEmail varchar(50),
    primary key (userID)
    );
```
2. board
```sql
 create table bbs (
    bbsID INT,
    bbsTitle VARCHAR(50),
    userID VARCHAR(20),
    bbsDate DATETIME,
    bbsContent VARCHAR(2048),
    bbsAvailable INT,
    bbsReDate DATETIME,
    PRIMARY KEY (bbsID)
    )DEFAULT CHARSET=utf8;
```
