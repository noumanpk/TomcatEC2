# TomcatEC2 DEMO
[![TomcatEC2 DEMO](https://img.youtube.com/vi/N3C3V7QRn4k/0.jpg)](https://www.youtube.com/watch?v=N3C3V7QRn4k&index=2&list=PLgxhSvoP-iTpuxlFy0f5Y49fCFSZp22TH)

# Quick start
On your terminal, type
     
     git clone https://github.com/micklinISgood/TomcatEC2.git
     cd  TomcatEC2
     ./bin/catalina.sh run
     
On your browser, paste the following link and click on Tweets Elapse. (host on EC2)

     http://<your_EC2_DNS>:8080/elapse/TweetElapse.html
     
On your browser, paste the following link and click on Tweets Elapse. (host on your laptop)

     http://localhost:8080/elapse/TweetElapse.html 

Dependency issue?
Follow [this](https://www.youtube.com/watch?v=-qPLGRNtgqU) 

Tweets elapse porject repo only? [here](https://github.com/micklinISgood/TweetsElapse) 

#Geek detail

![Fetch data](https://github.com/micklinISgood/TomcatEC2/blob/b0eb3f0b882c8f8145c5ac848835232b180ee17e/webapps/docs/fetch.png)

For distribution convenience, I pick up a sample data set from the No-SQL database as tweets_data.txt.

![Fetch data](https://github.com/micklinISgood/TomcatEC2/blob/b0eb3f0b882c8f8145c5ac848835232b180ee17e/webapps/docs/websocket.png)

Why WebSocket?
    
Websocket is a full-duplex communication channel between server and client. This could be prepared for trending push notification instead of polling the server from a client. 

However, you need to be comfortable to work with JSON because we need to define and manufacture the message identifier to branch out a specific request&response. 

