### Установка sngrep на centos 7 linux
1. Добавить irontec repository в локальные репо. Создать файл sngrep.repo  в /etc/yum.repos.d  и добавить в него:
```
[irontec]
name=Irontec RPMs repository
baseurl=http://packages.irontec.com/centos/$releasever/$basearch/
```
2. Затем добавить в систему Irontec repositories public key, используя следующую коммнаду: 
```
rpm --import http://packages.irontec.com/public.key
```
3. Обновляем yum cache и устанавливаем sngrep:
```
yum update
yum install sngrep
```
