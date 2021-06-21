## mysql
- mysql 跳过密码
1.vim /ect/my.cnf  添加一行 skip-grant-tables
2.use mysql;   
  update user set authentication_string=password('LinkCM@123') where user='root';
3.flush privileges
