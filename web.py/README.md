Setup Server with Python
==

- [Install web.py](webpy.md) 


- Test the server

```
nohup python test.py 80 &
```
you must be able to see "hello, this is a test" after you input the url ``` http://<you server ip>/wx ``` in your browser.

- Run main.py as server 

```
nohup python main.py 80 &

```
you must be able to see "hello, this is handle view" after you input the url ``` http://<you server ip>/wx ``` in your browser.

- Stop the Server

```
# netstat -nlpt
Active Internet connections (only servers)
Proto Recv-Q Send-Q Local Address               Foreign Address             State       PID/Program name
tcp        0      0 0.0.0.0:80                  0.0.0.0:*                   LISTEN      10667/python
tcp        0      0 0.0.0.0:22                  0.0.0.0:*                   LISTEN      1281/sshd
tcp        0      0 127.0.0.1:25                0.0.0.0:*                   LISTEN      1360/master
tcp        0      0 :::22                       :::*                        LISTEN      1281/sshd

# kill -9  10667
```