소프트웨어학부 20212983 김지윤

Make your git! - Git BLog 만드는 과정 기술

기존의 리눅스에서 테마를 적용하는 과정에서 오류 발생 -> 아예 repository 삭제 후 fork 방법으로 처음부터 다시 진행

1. jekyll-now 테마를 fork 함
2. config.yml 파일에 name, description 수정
3. about.md를 내 정보로 수정
4. 특강에 다뤄졌던 내용 Topic 중 배운 내용에 관련해 2021-12-16-Eureka_Project.md 작성
5. 댓글 기능을 구현하기 위해 Disqus 가입하고 세팅
6. config.yml에 key-value 추가
7. layouts/post.html에 Universal Code를 복사하고 주석처리를 해제하고 PAGE_URL과 PAGE_IDENTIFER를 설정
8. 그리고 Universal Code의 맨 앞에는 {% if page.comments %}, <h2>Comments</h2>를, 맨 뒤에는 {% endif %}를 추가
9. 아까 만들어둔 2021-12-16-Eureka_Project.md에 comments: true 를 해줘서 댓글 기능 구현
10. Google Analytics를 하기위해 Google Analytics 계정 생성
11. Google Analytics에서 속성 설정(이름, 시간대 등등)
12. Google Analytics의 속성에서 데이터 스트림 추가(웹 선택 후 블로그 url 입력)
13. 생성된 추적 ID를 원래 탬플릿에 있던 config.yml에 있는 google_analytics: 옆에 입력
14. 2021-12-16-Eureka_Project.md에 Google Analytics 내용을 추가
15. favicon 추가를 위해서 https://realfavicongenerator.net/ 에서 스마일 사진으로 압축 파일 다운로드
16. images/smilefavi 폴더 생성 후 다운 받은 압축 파일에 있는 내용을 추가
17. 만든 사이트에서 제공해주는 HTML 코드를 복사해와서 layouts/default.html <head> 부분에 추가
18. 코드에 href 링크 맨 앞에 {{site.baseurl}}/images/smilefavi 를 다 추가
