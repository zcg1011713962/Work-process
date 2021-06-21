

## mysql
- mysql 跳过密码
  - 1.vim /ect/my.cnf  添加一行 skip-grant-tables
  - 2.use mysql;   
     update user set authentication_string=password('LinkCM@123') where user='root';
  - 3.flush privileges

## centos7
- 防火墙
 - 防火墙开启端口 firewall-cmd --zone=public --add-port=8080/tcp --permanent <br/>
 - 重启防火墙 firewall-cmd --reload <br/>
 - 查看开通的端口列表 firewall-cmd --list-port <br/>
- 内核
 - 查看内核版本 hostnamectl <br/>

# jdk
- linux配置jdk
  export JAVA_HOME=/usr/local/java/1.8.0_281 <br/>
  export CLASSPATH=.:$JAVA_HOME/jre/lib/rt.jar:$JAVA_HOME/lib/dt.jar:$JAVA_HOME/lib/tools.jar <br/>
  export PATH=$PATH:$JAVA_HOME/bin <br/>

## 可用的视频流地址
- rtsp
  - rtsp://wowzaec2demo.streamlock.net/vod/mp4:BigBuckBunny_175k.mov <br/>
- http-flv
  - http://img.ksbbs.com/asset/Mon_1704/15868902d399b87.flv <br/>
  
## ffmpeg命令行
截取某段视频 ffmpeg  -i  -vcodec copy -acodec copy -ss 00:00:00 -to 00:02:00 d://yingshi.mp4 -y <br/>


