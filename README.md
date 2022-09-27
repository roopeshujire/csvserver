[roopesh@localhost solution]$ sudo docker run -d -v /home/roopesh/solution/solution/inputFile:/csvserver/inputdata -p 9393:9300 -e CSVSERVER_BORDER=Orange infracloudio/csvserver:latest
f4ce846fe622236eaa916eda48bd637e28188ceec9a761d8d4c88703043b76b3
[roopesh@localhost solution]$ 
[roopesh@localhost solution]$ 
[roopesh@localhost solution]$ sudo docker ps
CONTAINER ID   IMAGE                           COMMAND                  CREATED          STATUS         PORTS                                       NAMES
f4ce846fe622   infracloudio/csvserver:latest   "/csvserver/csvserver"   11 seconds ago   Up 8 seconds   0.0.0.0:9393->9300/tcp, :::9393->9300/tcp   focused_lewin
[roopesh@localhost solution]$ ls -lrth
total 12K
-rw-rw-r-- 1 roopesh roopesh 90 Sep 27 17:22 inputfile
-rw-rw-r-- 1 roopesh roopesh  0 Sep 27 17:31 inputdata
-rw-rw-r-- 1 roopesh roopesh 58 Sep 27 18:06 gencsv.sh
-rw-rw-r-- 1 roopesh roopesh 89 Sep 27 18:06 inputFile
[roopesh@localhost solution]$ vim gencsv.sh 

