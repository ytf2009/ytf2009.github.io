---
sort: 2
---



<center><font size='50'><b>安装制品库--Nexus</b></font></center>







```bash
docker run 	-d \
	--net host \
	-p 8081:8081 \
	--user root \
	--name nexus \
	--restart=unless-stopped \
	-v /data/nexus:/nexus-data \
	sonatype/nexus3:3.25.1
```













