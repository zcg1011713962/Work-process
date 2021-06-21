## mysql
- mysql 跳过密码
  - 1.vim /ect/my.cnf  添加一行 skip-grant-tables
  - 2.use mysql;   
     update user set authentication_string=password('LinkCM@123') where user='root';
  - 3.flush privileges

## centos7
开启端口
firewall-cmd --zone=public --add-port=8080/tcp --permanent

重启防火墙
firewall-cmd --reload

查看开通的端口列表
firewall-cmd --list-port

查看内核版本
hostnamectl

## 可用的视频流地址
- rtsp
  rtsp://wowzaec2demo.streamlock.net/vod/mp4:BigBuckBunny_175k.mov
- http-flv
  http://img.ksbbs.com/asset/Mon_1704/15868902d399b87.flv
