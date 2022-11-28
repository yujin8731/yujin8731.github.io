
# 깃블로그 생성 과정
-----
준비 과정 : 루비 및 지킬 설치 우선적으로 완료

1. 깃허브 시작하기
- 깃허브에 로그인한후 계정 옆의 + 를 누르고 [New repository] 선택
- repository name 필드에 <계정.github.io> 입력
 
2.지역저장소를 원격 저장소에 연결
- 지역저장소 만들기: git blog 생성

- 원격저장소에 연결하기
+윈도우 이용으로 강의안 리눅스 기준으로 된 강의안을 따라하기가 쉽지 않아 보다 쉬운 이용을 위해서 깃허브 데스크탑 설치
+깃허브 데스크탑 file버튼 clone repository 후 생성해둔 지역저장소에 clone 완료

- 지역저장소 활동
  [지킬 설치 여부를 확인]
  jeklly -v


  [지킬 시작]
  jeklly new . force --force


  [지킬 서버 실행 후, localhost:4000 접속]
  (bundle exec) jekyll serve 

  yujin831.github.io 접속시 잘 반영된걸 확인

3. 원격저장소에 올리기 및 내려받기
- 깃블로그 Lanyon 테마 파일을 zip파일로 다운받아 지역저장소에 파일 저장
- 이미 존재하는 파일은 덮어쓰기

-----
### 추가 기능 구현
1. 댓글 기능 구현
- Disqus 가입 후 세팅

- config.yml 파일 수정 
  comment:
  provider: "disqus"
  disqus:
    shortname: "yujin8731" 코드 추가
    
 - layouts/post.html 파일에 Universal Code 추가
    주석 해제 후, PAGE_URL과 PAGE_IDENTIFIER를 설정하고 s.src가 잘 지정되어있는지 확인
    
 - 댓글을 허용하고 싶은 곳에
 -  comments: True
 -  로 지정
 
 
 -----
  ### 선택 과제 구현
1. Google Analytics 구현
- GA 계정 생성
  -  https://analytics.google.com/ 으로 이동하여 ‘측정 시작’ 클릭
  - ‘계정이름’ 입력하고 ‘다음’ 클릭
  - ‘웹’ 선택하고 ‘다음’ 클릭
  - 웹사이트 이름 : 아무거나
  - 블로그 웹사이트 URL : yujin8731.github.io
  - ‘만들기’ 버튼 선택

- 깃허브 블로그 연동
  - 관리자 화면의 상단에 추적 ID 를 복사후 깃허브 블로그 repository 의 _config.yml 파일을 수정

2. favicon 구현
- https://icons8.kr/icons/set/favicon-ico 에서 원하는 favicon 이미지를 16x16으로 다운받는다
- 루트 디렉토리에 asset 폴더를 새롭게 만들고 다운받는 이미지를 넣는다
- /_config.yml 에 코드 asset_url: /assets 추가한다
- /_include/head.html 12라인에 favicon 설정하는 코드를 추가한다


------
### 참고 자료




