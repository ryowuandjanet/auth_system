1.先啟動postsql
  set PGHOME=D:\Program\pgsql12.4-1\pgsql
  set PATH=%PGHOME%\bin;%path%
  set PGHOST=localhost
  set PGLIB=%PGHOME%\lib
  set PGDATA=%PGHOME%\data

  pg_ctl start

2.編譯frontend(前端)的React程式碼
  C:\RyowuTestCode\djangotest\AUTH_SYSTEM\frontend (master)
  λ npm run build

3.到backend(後端)的Django程式碼，去修改settings.py
  EMAIL_HOST_USER = '管理者gmail的帳號'
  EMAIL_HOST_PASSWORD = '管理者gmail的密碼'

4.執行backend(後端)的Django程式碼
  python manage.py runserver 3000

4.進入localhost:3000