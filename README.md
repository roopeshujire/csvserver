
roopesh@localhost solution]$ sudo docker run -d -v /home/roopesh/solution/solution/inputFile:/csvserver/inputdata -p 9393:9300 -e CSVSERVER_BORDER=Orange infracloudio/csvserver:latest

f4ce846fe622236eaa916eda48bd637e28188ceec9a761d8d4c88703043b76b3


[roopesh@localhost solution]$
[roopesh@localhost solution]$
[roopesh@localhost solution]$ sudo docker ps


CONTAINER ID   IMAGE                           COMMAND                  CREATED          STATUS         PORTS                                       NAMES
f4ce846fe622   infracloudio/csvserver:latest   "/csvserver/csvserver"   11 seconds ago   Up 8 seconds   0.0.0.0:9393->9300/tcp, :::9393->9300/tcp   focused_lewin


