# helper
**Stuff about everything**

* [Hibernate](java-hibernate.md)
* [Hibernate](java-hibernate.md)

## Linux

``` lsof -i -P -n | grep LISTEN | grep java```<br>
java      26419   root   21u  IPv6 120843      0t0  TCP *:8881 (LISTEN)<br>
java      26851   root    7u  IPv6 121553      0t0  TCP *:8070 (LISTEN)

```ps aux | grep jar```<br>
root     26419  0.4 10.6 2615168 228104 pts/0  Sl   18:40   0:22 java -jar target/configuration-service.jar

kill javas<br>
```kill $(ps aux | grep "java" | grep -v 'grep' | awk '{print $2}')```

## Git

Aproved method __(+)__ <br>
Add .gitignore
Commit all pending changes, then run this command:<br>

```git rm -r --cached .```<br>
This removes everything from the index, then just run:<br>
```git add .```<br>
Commit it:<br>
```git commit -m ".gitignore is now working"```
