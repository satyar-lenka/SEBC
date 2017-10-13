<p>The full teragen/time command and job output</p>

<pre><code>
[jimenez@ip-172-31-3-113 centos]$ time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar teragen -Dmapreduce.job.maps=8 -D dfs.block.size=64M -Dmapreduce.map.memory.mb=512 65536000 /user/jimenez/tgen
17/10/13 18:21:48 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-12-173.us-west-2.compute.internal/172.31.12.173:8032
17/10/13 18:21:48 INFO terasort.TeraSort: Generating 65536000 using 8
17/10/13 18:21:48 INFO mapreduce.JobSubmitter: number of splits:8
17/10/13 18:21:48 INFO Configuration.deprecation: dfs.block.size is deprecated. Instead, use dfs.blocksize
17/10/13 18:21:49 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1507917691547_0001
17/10/13 18:21:49 INFO impl.YarnClientImpl: Submitted application application_1507917691547_0001
17/10/13 18:21:49 INFO mapreduce.Job: The url to track the job: http://ip-172-31-12-173.us-west-2.compute.internal:8088/proxy/application_1507917691547_0001/
17/10/13 18:21:49 INFO mapreduce.Job: Running job: job_1507917691547_0001
17/10/13 18:21:56 INFO mapreduce.Job: Job job_1507917691547_0001 running in uber mode : false
17/10/13 18:21:56 INFO mapreduce.Job:  map 0% reduce 0%
17/10/13 18:22:10 INFO mapreduce.Job:  map 9% reduce 0%
17/10/13 18:22:11 INFO mapreduce.Job:  map 17% reduce 0%
17/10/13 18:22:13 INFO mapreduce.Job:  map 24% reduce 0%
17/10/13 18:22:14 INFO mapreduce.Job:  map 27% reduce 0%
17/10/13 18:22:16 INFO mapreduce.Job:  map 30% reduce 0%
17/10/13 18:22:17 INFO mapreduce.Job:  map 31% reduce 0%
17/10/13 18:22:18 INFO mapreduce.Job:  map 32% reduce 0%
17/10/13 18:22:19 INFO mapreduce.Job:  map 36% reduce 0%
17/10/13 18:22:21 INFO mapreduce.Job:  map 38% reduce 0%
17/10/13 18:22:22 INFO mapreduce.Job:  map 43% reduce 0%
17/10/13 18:22:24 INFO mapreduce.Job:  map 45% reduce 0%
17/10/13 18:22:25 INFO mapreduce.Job:  map 49% reduce 0%
17/10/13 18:22:27 INFO mapreduce.Job:  map 50% reduce 0%
17/10/13 18:22:28 INFO mapreduce.Job:  map 53% reduce 0%
17/10/13 18:22:30 INFO mapreduce.Job:  map 54% reduce 0%
17/10/13 18:22:31 INFO mapreduce.Job:  map 59% reduce 0%
17/10/13 18:22:33 INFO mapreduce.Job:  map 61% reduce 0%
17/10/13 18:22:34 INFO mapreduce.Job:  map 66% reduce 0%
17/10/13 18:22:36 INFO mapreduce.Job:  map 68% reduce 0%
17/10/13 18:22:38 INFO mapreduce.Job:  map 72% reduce 0%
17/10/13 18:22:40 INFO mapreduce.Job:  map 74% reduce 0%
17/10/13 18:22:41 INFO mapreduce.Job:  map 81% reduce 0%
17/10/13 18:22:44 INFO mapreduce.Job:  map 83% reduce 0%
17/10/13 18:22:46 INFO mapreduce.Job:  map 84% reduce 0%
17/10/13 18:22:47 INFO mapreduce.Job:  map 85% reduce 0%
17/10/13 18:22:52 INFO mapreduce.Job:  map 86% reduce 0%
17/10/13 18:22:53 INFO mapreduce.Job:  map 87% reduce 0%
17/10/13 18:22:55 INFO mapreduce.Job:  map 89% reduce 0%
17/10/13 18:22:56 INFO mapreduce.Job:  map 91% reduce 0%
17/10/13 18:22:59 INFO mapreduce.Job:  map 93% reduce 0%
17/10/13 18:23:02 INFO mapreduce.Job:  map 94% reduce 0%
17/10/13 18:23:04 INFO mapreduce.Job:  map 95% reduce 0%
17/10/13 18:23:08 INFO mapreduce.Job:  map 96% reduce 0%
17/10/13 18:23:11 INFO mapreduce.Job:  map 97% reduce 0%
17/10/13 18:23:17 INFO mapreduce.Job:  map 98% reduce 0%
17/10/13 18:23:20 INFO mapreduce.Job:  map 99% reduce 0%
17/10/13 18:23:28 INFO mapreduce.Job:  map 100% reduce 0%
17/10/13 18:23:38 INFO mapreduce.Job: Job job_1507917691547_0001 completed successfully
17/10/13 18:23:38 INFO mapreduce.Job: Counters: 31
	File System Counters
		FILE: Number of bytes read=0
		FILE: Number of bytes written=979464
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=682
		HDFS: Number of bytes written=6553600000
		HDFS: Number of read operations=32
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=16
	Job Counters 
		Launched map tasks=8
		Other local map tasks=8
		Total time spent by all maps in occupied slots (ms)=586904
		Total time spent by all reduces in occupied slots (ms)=0
		Total time spent by all map tasks (ms)=586904
		Total vcore-seconds taken by all map tasks=586904
		Total megabyte-seconds taken by all map tasks=600989696
	Map-Reduce Framework
		Map input records=65536000
		Map output records=65536000
		Input split bytes=682
		Spilled Records=0
		Failed Shuffles=0
		Merged Map outputs=0
		GC time elapsed (ms)=1885
		CPU time spent (ms)=138850
		Physical memory (bytes) snapshot=1466437632
		Virtual memory (bytes) snapshot=9108451328
		Total committed heap usage (bytes)=1830813696
	org.apache.hadoop.examples.terasort.TeraGen$Counters
		CHECKSUM=140750829423462787
	File Input Format Counters 
		Bytes Read=0
	File Output Format Counters 
		Bytes Written=6553600000

real	1m52.765s
user	0m6.373s
sys	0m0.326s
[jimenez@ip-172-31-3-113 centos]$ 
</code></pre>



<p>The command and output of hdfs dfs -ls /user/jimenez/tgen</p>

<pre><code>
[jimenez@ip-172-31-3-113 centos]$ hdfs dfs -ls /user/jimenez/tgen
Found 9 items
-rw-r--r--   3 jimenez rangers          0 2017-10-13 18:23 /user/jimenez/tgen/_SUCCESS
-rw-r--r--   3 jimenez rangers  819200000 2017-10-13 18:23 /user/jimenez/tgen/part-m-00000
-rw-r--r--   3 jimenez rangers  819200000 2017-10-13 18:23 /user/jimenez/tgen/part-m-00001
-rw-r--r--   3 jimenez rangers  819200000 2017-10-13 18:23 /user/jimenez/tgen/part-m-00002
-rw-r--r--   3 jimenez rangers  819200000 2017-10-13 18:23 /user/jimenez/tgen/part-m-00003
-rw-r--r--   3 jimenez rangers  819200000 2017-10-13 18:23 /user/jimenez/tgen/part-m-00004
-rw-r--r--   3 jimenez rangers  819200000 2017-10-13 18:23 /user/jimenez/tgen/part-m-00005
-rw-r--r--   3 jimenez rangers  819200000 2017-10-13 18:22 /user/jimenez/tgen/part-m-00006
-rw-r--r--   3 jimenez rangers  819200000 2017-10-13 18:23 /user/jimenez/tgen/part-m-00007
[jimenez@ip-172-31-3-113 centos]$ 
</code></pre>


<p>The command and output of hadoop fsck -blocks /user/jimenez</p>

<pre><code>
[jimenez@ip-172-31-3-113 centos]$ hadoop fsck -blocks /user/jimenez
DEPRECATED: Use of this script to execute hdfs command is deprecated.
Instead use the hdfs command for it.

Connecting to namenode via http://ip-172-31-12-173.us-west-2.compute.internal:50070
FSCK started by jimenez (auth:SIMPLE) from /172.31.3.113 for path /user/jimenez at Fri Oct 13 18:26:05 UTC 2017
.........Status: HEALTHY
 Total size:	6553600000 B
 Total dirs:	3
 Total files:	9
 Total symlinks:		0
 Total blocks (validated):	104 (avg. block size 63015384 B)
 Minimally replicated blocks:	104 (100.0 %)
 Over-replicated blocks:	0 (0.0 %)
 Under-replicated blocks:	0 (0.0 %)
 Mis-replicated blocks:		0 (0.0 %)
 Default replication factor:	3
 Average block replication:	3.0
 Corrupt blocks:		0
 Missing replicas:		0 (0.0 %)
 Number of data-nodes:		4
 Number of racks:		1
FSCK ended at Fri Oct 13 18:26:05 UTC 2017 in 6 milliseconds


The filesystem under path '/user/jimenez' is HEALTHY
[jimenez@ip-172-31-3-113 centos]$ 
</code></pre>