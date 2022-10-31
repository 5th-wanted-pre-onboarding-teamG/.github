![image](https://static.wanted.co.kr/images/events/2144/764914c4.jpg)

## 👋 Team Members
|Name|Role|Github|Email|
|-----|:--:|----|-------|
|강진희|팀장|https://github.com/wlsgml719|20wlsgml@gmail.com| 
|김용범|팀원|https://github.com/MisterRuby|rubykim0723@gmail.com| 
|이성태|팀원|https://github.com/stae1102|stae1102@gmail.com| 
|최영남|팀원|https://github.com/nuobasic|nuobasic@naver.com| 
|최은강|팀원|https://github.com/loveAlakazam|dmsrkd1216@gmail.com|

<br>

## 🗓 프리온보딩 진행 기간
```2022.10.25 ~ 2022.11.18```


## [📝 Team G Notion](https://www.notion.so/Team-G-db8f81b91e314bc49494340b6ea99bd2)

<br>

## 📕 Projects

|순서|기업과제명|참여기업|기간|사용기술|
|:--:|:-------:|:------:|:------:|:------:|
|1|회원별 게시판과 통계기능 제공 웹서버|웨인힐스벤처스|2022.10.26 ~ 2022.10.28|NestJS, NodeJS, Typescript, MySQL, AWS RDS|
|2|제품 쇼핑몰 관리 페이지|아이엠랩|2022.10.31 ~ 2022.11.02|NestJS, NodeJS, Typescript, MySQL|

<br><br>

## ✅ Git Convenvtion
### Commit message

- 제목은 명령문으로
- 제목 끝에 마침표(.) 금지
- 제목과 본문을 한 줄 띄워 분리하기
- 본문은 "어떻게" 보다 "무엇을", "왜"를 설명한다.
- 본문에 여러 줄의 메시지를 작성할 땐 "-" 혹은 "번호"로 구분


#### 1. 제목은 50자 이내로

- `<타입> <#이슈번호> <제목>`
- 예시: `docs: #1 README.md 수정`

- 주의사항
  - 하나의 커밋에는 한가지 기능만 포함합니다.

> GOOD CASE

```
(ex1) feat : 유저 모델 생성
(ex2) feat : 유저 모델 Create API 개발
(ex3) test : 유저 모델 Create API Testcase 작성
(ex4) refactor: 유저 로그인 API 리팩토링
```

<br>


> BAD CASE

```
(ex1) feat : 유저, 회사 CRUD API 개발
(ex2) refactor: 리팩토링
(ex3) 유저 모델 생성
```



#### 2. 본문 72자마다 줄 바꾸기

```
(예시)
상세설명이 필요하면 본문작성하시면 됩니다.
어떤 기능인지, api url 주소를 알려주세요.
```

<br>


#### 3. Commit Types

|타입| 리스트|
|:--:|:--:|
|   init    | 초기화|
|   feat    | 기능추가|
|   add     | 내용추가|
|   update  | 기능 보완 (업그레이드)|
|   fix     | 버그 수정|
|   refactor| 리팩토링|
|   style   | 스타일 (코드 형식, 세미콜론 추가: 비즈니스 로직에 변경 없음)|
|   docs    | 문서 (README.md, ignore파일 추가(Add), 수정, 삭제)|
|   test    | 테스트 (테스트 코드 추가, 수정, 삭제: 비즈니스 로직에 변경 없음)|
|   chore   | 기타 변경사항 (빌드 스크립트 수정, 코드컨벤션에 맞게 코드수정 등 )|
|   rename  | 이름(파일명, 폴더명, 변수명 등)을 수정하거나 옮기는 작업만인 경우|
|   remove  | 파일을 삭제하는 작업만 수행한 경우  |
|   hofix   | main 브랜치에서 버그가 발생하는가?|


### Branch Strategy

- main-feature 의 구성을 따릅니다.<br>

팀의 멤버는 각자의 작업내용에 맞는 feature 브랜치를 만들어서 작업을 진행합니다. <br>
작업이 끝나면 공용 브랜치인 main 브랜치에 작업 완료된 내용을 병합시키겠다는 내용을 팀원들에게 알리고 병합을 진행하면 되겠습니다.

<br>

- feature/issue-이슈번호<br>
각자 맡은 기능을 개발하는 브랜치 입니다. <br>
브랜치 이름은 <b>`feature/issue-이슈번호`</b>로 하고

작업이 완료되면, develop 브랜치에  pull request를 진행합니다.

PR 리뷰어는 팀원 전원으로 합니다.

코드리뷰의 기준은 다음과 같습니다.

- 1. 해당 이슈에서 에러 없이 정상작동하는가?
- 2. 테스트케이스를 만들었는가?
  - 만들었다면, 성공케이스/실패케이스 를 만들었는가?
- 3. 코드컨벤션을 잘 지켰는가?
- 4. 코드가 잘 읽혀지는가? 코드를 읽고 동작의 흐름이 이해되는가?


- main<br>
모든 내용이 문제가 없을 경우에는 main 브랜치로 코드를 병합시켜서 보관합니다.

```
❗️ Pull request & Merge 규칙 ❗️
 - Pull request와 Merge는 다른 사람이 하도록
 - Merge하기 전에 Pull request코드 확인하고 리뷰 남기기
```

## ✅ Code Convention
- Class & FileName
  - Pascal Case (ex: `SampleClass`, `SampleController.ts` )
  
- Model
  - Pascal Case (ex: `SampleModel`)
  - Model Field: camelCase (ex: `sampleField`)
  - Model Method: camelCase (ex: `sampleMethod()`)
  - Modeling Conventions
    - 1:1 관계: 단수
    - 1:N 관계: 복수
    - M:N 관계: 중간 연결 테이블은 단수, 메인테이블은 복수
  
- Function
  - camelCase (ex: `getUser()` )
  
<br>  
  
- Variables
  - camelCase (ex: `sampleVariable`)

<br>

- Constant / Global => 전부다 대문자 사용.
  - `.env` 파일에 있는 설정값 및 포트번호
  - 고정된 상수값인 경우


```js
// .env 파일


DB_HOST=127.0.0.1
DB_PORT=3306
```

 
 ### 주석처리
 
 
