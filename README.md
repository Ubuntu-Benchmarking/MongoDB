# MongoDB

sudo wget https://github.com/brianfrankcooper/YCSB/releases/download/0.17.0/ycsb-mongodb-binding-0.17.0.tar.gz

sudo tar sudo tar xvf  ycsb-mongodb-binding-0.17.0.tar.gz

sudo wget https://www.python.org/ftp/python/2.7.9/Python-2.7.9rc1.tgz

//curl -O https://www.python.org/ftp/python/2.7.9/Python-2.7.9rc1.tgz

sudo tar -xzvf Python-2.7.9rc1.tgz

cd Python-2.7.9rc1

./configure

make

sudo make install

python2 –version

nano docker_compose.yml

sudo docker compose -f docker_compose.yml up -d

http://localhost:8081/

loading phase: picocluster64@pc0:~/fe/ycsb-mongodb-binding-0.17.0 $ sudo ./bin/ycsb load mongodb -s -P workloads/workloadc -threads 16 -p mongodb.url="mongodb://10.0.13.240:27017/admin"

transaction phase: picocluster64@pc0:~/fe/ycsb-mongodb-binding-0.17.0 $ sudo ./bin/ycsb run mongodb -s -P workloads/workloadd -threads 16 -p mongodb.url="mongodb://10.0.13.240:27017/admin"
