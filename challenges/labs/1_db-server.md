<p>The command hostname -f and its output</p>

<pre><code>
[root@ip-172-31-6-74 centos]# hostname -f
ip-172-31-6-74.us-west-2.compute.internal
[root@ip-172-31-6-74 centos]# 
</code></pre>

<p>The command mysql -u <user> -p<password> -e "status;" and its output</p>

<pre><code>
[root@ip-172-31-6-74 centos]# 
[root@ip-172-31-6-74 centos]# mysql -u root -proot -e "status;"
--------------
mysql  Ver 14.14 Distrib 5.5.57, for Linux (x86_64) using readline 5.1

Connection id:		21
Current database:	
Current user:		root@localhost
SSL:			Not in use
Current pager:		stdout
Using outfile:		''
Using delimiter:	;
Server version:		5.5.57 MySQL Community Server (GPL)
Protocol version:	10
Connection:		Localhost via UNIX socket
Server characterset:	latin1
Db     characterset:	latin1
Client characterset:	utf8
Conn.  characterset:	utf8
UNIX socket:		/var/lib/mysql/mysql.sock
Uptime:			15 min 16 sec

Threads: 1  Questions: 65  Slow queries: 0  Opens: 34  Flush tables: 1  Open tables: 27  Queries per second avg: 0.070
--------------
</code></pre>

<p>The command mysql -u <user> -p<password> -e "show databases;" and its output</p>
	

<pre><code>
[root@ip-172-31-6-74 centos]# mysql -u root -proot -e "show databases;"
+--------------------+
| Database           |
+--------------------+
| information_schema |
| hive               |
| hue                |
| mysql              |
| oozie              |
| performance_schema |
| rman               |
| scm                |
| sentry             |
+--------------------+
[root@ip-172-31-6-74 centos]# 
</code></pre>