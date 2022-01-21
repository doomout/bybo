# 파이썬, 장고를 이용한 게시판 개발
IDE : PyCharm 2021.3.1  
DB  : sqlite3(64비트)  
언어 : 파이썬 3.10.1  
사용 프레임워크 : 장고 3.1.3  
사용 웹 화면 : html5, css, bootstrap 4.5.3   

서버 구동 명령어 : python manage.py runserver  

대략의 흐름  
1. 서버(현재는 localhost:8000/pybo/)  
2. config/urls.py 에서 URL 해석해서 pybo/views.py 파일의 index함수 호출  
3. pybo/views.py 파일의 index함수를 실행하여 결과를 웹 브라우저에 전달  

DB 구조 (1 : N)  
질문 1개에 답변이 여러개 연결  
질문 삭제시 답변도 함께 삭제  
Question모델 -> Answer모델   

 localhost:8000/admin   
 id: admin   
 pw: ska123   