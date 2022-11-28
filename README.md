
# 깃블로그 만든 과정

준비 과정 : 루비 및 지킬 설치 우선적으로 완료

1. 깃허브 시작하기
- 깃허브에 로그인한후 계정 옆의 + 를 누르고 [New repository] 선택
- repository name 필드에 <계정.github.io> 입력
 
2.지역저장소를 원격 저장소에 연결
- 지역저장소 만들기: git blog 생성

- 원격저장소에 연결하기
+윈도우 이용으로 강의안 리눅스 기준으로 된 강의안을 따라하기가 쉽지 않아 보다 쉬운 이용을 위해서 깃허브 데스크탑 설치
+깃허브 데스크탑 file버튼 clone repository 후 생성해둔 지역저장소에 clone 완료

-지역저장소 활동
지킬 설치 여부를 확인 
jeklly -v

지킬 시작
jeklly new . force --force

지킬 서버 실행 후, localhost:4000 접속 
(bundle exec) jekyll serve 

yujin831.github.io 접속시 잘 반영된걸 확인

3. 원격저장소에 올리기 및 내려받기
- 깃블로그 Lanyon 테마 파일을 zip파일로 다운받아 지역저장소에 파일 저장
- 이미 존재하는 파일은 덮어쓰기


## 추가 기능 구현
1. 댓글 기능 구현
- Disqus 가입 후 세팅

- config.yml 파일에 
  comment:
  provider: "disqus"
  disqus:
    shortname: "yujin8731" 코드 추가
    
 - layouts/post.html 파일에 Universal Code 추가
    주석 해제 후, PAGE_URL과 PAGE_IDENTIFIER를 설정하고 s.src가 잘 지정되어있는지 확인
    
 댓글을 허용하고 싶은 곳에 comments: True로 지정


# 참고 자료
책 사진 넣기 



