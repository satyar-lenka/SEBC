<p>Cloud provider - AWS</>


<p>Private IPs</p>

* ip-172-31-6-74.us-west-2.compute.internal
* ip-172-31-3-113.us-west-2.compute.internal
* ip-172-31-13-157.us-west-2.compute.internal
* ip-172-31-14-253.us-west-2.compute.internal
* ip-172-31-12-173.us-west-2.compute.internal


<p>Public IPs</p>

* ec2-52-89-255-147.us-west-2.compute.amazonaws.com
* ec2-35-165-10-154.us-west-2.compute.amazonaws.com
* ec2-52-35-172-166.us-west-2.compute.amazonaws.com
* ec2-34-215-199-205.us-west-2.compute.amazonaws.com
* ec2-34-212-65-210.us-west-2.compute.amazonaws.com


<p>Linux release</p>

centos-release-7-4.1708.el7.centos.x86_64



<p>List the file system capacity for the first node</p>
<pre><code>
[root@ip-172-31-6-74 centos]# df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvda1       30G  822M   30G   3% /
devtmpfs        7.3G     0  7.3G   0% /dev
tmpfs           7.3G     0  7.3G   0% /dev/shm
tmpfs           7.3G   17M  7.3G   1% /run
tmpfs           7.3G     0  7.3G   0% /sys/fs/cgroup
tmpfs           1.5G     0  1.5G   0% /run/user/0
tmpfs           1.5G     0  1.5G   0% /run/user/1000
[root@ip-172-31-6-74 centos]
</code></pre>


<p>List the command and output for yum repolist enabled</p>

[root@ip-172-31-6-74 centos]# yum repolist enabled
Loaded plugins: fastestmirror
Loading mirror speeds from cached hostfile
 * base: mirrors.sonic.net
 * extras: mirror.genesisadaptive.com
 * updates: mirror.web-ster.com
repo id                                               repo name                                                       status
base/7/x86_64                                         CentOS-7 - Base                                                 9,591
extras/7/x86_64                                       CentOS-7 - Extras                                               227
updates/7/x86_64                                      CentOS-7 - Updates                                              740
repolist: 10,558
[root@ip-172-31-6-74 centos]# 



<p>List the /etc/passwd entries for jimenez and beltran</p>
<pre><code>
jimenez:x:2800:2800::/home/jimenez:/bin/bash
beltran:x:2900:2900::/home/beltran:/bin/bash
</code></pre>


<p>List the /etc/group entries for astros and rangers</p>
<pre><code>
astros:x:2901:beltran
rangers:x:2902:jimenez
</code></pre>
