# demo-activemq
##1、安装方法:
</br>
brew install apache-activemq
</br>

##2、启动方法:
<br/>
cd /usr/local/Cellar/activemq/bin
<br/>
./activemq start
<br/>
启动后访问http://127.0.0.1:8161/admin/,可查看控制台
<br/>

##3、点对点模式
![image](./src/main/resources/ptp.png)
<br/>
生产者发送一条消息到queue，只有一个消费者能收到。
<br/>
示例代码见 com/kiven/demo/activemq/ptp
<br/>

##4、订阅模式
![image](./src/main/resources/subscribe.png)
<br/>
发布者发送到topic的消息，只有订阅了topic的订阅者才会收到消息。
<br/>
订阅者只能接收订阅后发送的消息,订阅之前发送的消息,接收不到
<br/>
示例代码见 com/kiven/demo/activemq/topic