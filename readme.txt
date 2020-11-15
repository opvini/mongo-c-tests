After mongoDB installed and running

RUN MONGO:
$ sudo mongod --fork --logpath /var/log/mongodb/mongod.log
OR
$ sudo mongod --fork --logpath /home/opvini/Git/mongo-c-tests/mongo/mongo-server-log/mongo-log.txt --dbpath /home/opvini/Git/mongo-c-tests/mongo/mongo-db

BUILD (in ./build):
$ cmake .
$ make

Install: CMake Tools in VSC
1) In the console (ctrl+shift+P): CMake: Configure
2) Debug shall be done using the CMake Tools (bottom toolbar)
3) Press to debug, and voiala