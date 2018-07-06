# helper
Stuff about everything

#Linux
lsof -i -P -n | grep LISTEN | grep java
java      26419   root   21u  IPv6 120843      0t0  TCP *:8881 (LISTEN)
java      26851   root    7u  IPv6 121553      0t0  TCP *:8070 (LISTEN)

ps aux | grep jar
root     26419  0.4 10.6 2615168 228104 pts/0  Sl   18:40   0:22 java -jar target/configuration-service.jar

kill javas
kill $(ps aux | grep "java" | grep -v 'grep' | awk '{print $2}')

#Git
