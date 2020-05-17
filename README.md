# elastic-search
Elastic Search

* elastic search 설치하기

vi /etc/yum.repos.d/elasticsearch.repo

[elasticsearch-6.x]
name=Elasticsearch repository for 6.x packages
baseurl=https://artifacts.elastic.co/packages/6.x/yum
gpgcheck=1
gpgkey=https://artifacts.elastic.co/GPG-KEY-elasticsearch
enabled=1
autorefresh=1
type=rpm-md

* java memory heap size 문제 발생시 메모리 크기조정
vim /etc/elasticsearch/jvm.options

-Xms500m 
-Xmx500m 

* 서비스 등록하기
service elasticsearch start

