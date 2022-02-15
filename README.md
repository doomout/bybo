# 파이썬, 장고를 이용한 게시판 개발
IDE : PyCharm 2021.3.1  
DB  : sqlite3(64비트)  
언어 : 파이썬 3.10.1  
사용 프레임워크 : 장고 3.1.3  
사용 웹 화면 : html5, css, bootstrap 4.5.3   

개발 서버 구동 명령어 : python manage.py runserver  

---- 서버 설정 ------  
서버 시간 설정하기(한국 시간으로)   
sudo ln -sf /usr/share/zoneinfo/Asia/Seoul /etc/localtime

가상 환경 설치  
sudo apt update  
sudo apt install python3-venv  
mkdir projects, mkdir venvs

venvs 디렉터리로 이동해 장고 가상 환경  
cd venvs  
python3 -m venv mysite  
cd mysite  
cd bin  
 . activate  

wheel 패키지 설치 - pip install wheel  

django 패키지 설치 - pip install django==3.1.3  

markdown 패키지 설치 - pip install markdown  

데이터베이스 생성 - python manage.py migrate  

Gunicorn 설치 - pip install gunicorn  
Gunicorn 자동등록 - sudo systemctl enable mysite.service  

Nginx 설치 - sudo apt install nginx

서버 git 업데이트 후 - sudo systemctl restart mysite.service


 localhost:8000/admin   
 id: admin   
 pw: ska123   
   
도서 공식 소스 : https://wikidocs.net/book/4223