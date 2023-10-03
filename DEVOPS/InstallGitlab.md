---
sort: 1
---



<center><font size='50'><b>安装代码库--Gitlab</b></font></center>









```bash
docker run --detach \
  --hostname gitlab.example.city \
  --publish 443:443 --publish 80:80 --publish 22:22 \
  --name gitlab \
  --restart always \
  --volume /data/gitlab/config:/etc/gitlab \
  --volume /data/gitlab/logs:/var/log/gitlab \
  --volume /data/gitlab/data:/var/opt/gitlab \
  --volume /opt/gitlab/backups/:/var/opt/gitlab/backups/ \
  -e TZ=Asia/Shanghai \
  gitlab/gitlab-ce:13.12.15-ce.0
```



