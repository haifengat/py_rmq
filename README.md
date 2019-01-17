# ali_rmq_demo

#### 介绍
rocketMQ 接口测试

#### 软件架构
软件架构说明

#### 安装教程

* 官方sdk安装说明 https://help.aliyun.com/document_detail/29555.html?spm=a2c4g.11186623.6.569.7ae3650eOuGUim
* 编译时采用动态编译方�
    * 增加boost和rmq路径 export LD_LIBRARY_PATH=../lib/lib-boost-share:/usr/local/lib
    * g++ -shared -fPIC -Wall -Wno-deprecated -L ../lib/lib-boost-share/ -I ../include/   -lonsclient4cpp -lboost_system -lboost_thread -lboost_chrono -lboost_filesystem -lpthread consumer.cpp -o consumer.so
    * g++ -shared -fPIC -Wall -Wno-deprecated -L ../lib/lib-boost-share/ -I ../include/   -lonsclient4cpp -lboost_system -lboost_thread -lboost_chrono -lboost_filesystem -lpthread producer.cpp -o producer.so


#### 使用说明

* 按照官方说明把c++sdk下载安装�
* 修改上面g++指令中的 `../include` �`../lib/lib-boost-share/` 为sdk对应的文件夹
