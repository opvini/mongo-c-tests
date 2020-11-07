After mongoDB installed and running

RUN MONGO:
$ sudo mongod --fork --logpath /var/log/mongodb/mongod.log
OR
$ sudo mongod --fork --logpath /home/opvini/Git/mongo-c-tests/mongo/mongo-server-log/mongo-log.txt --dbpath /home/opvini/Git/mongo-c-tests/mongo/mongo-db

BUILD (in ./build):
$ cmake .
$ make