<p>terasort command and full output</p>

<pre><code>
	[jimenez@ip-172-31-3-113 centos]$ hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar terasort /user/jimenez/tgen /user/jimenez/tsort
	17/10/13 18:52:12 INFO terasort.TeraSort: starting
	17/10/13 18:52:14 INFO hdfs.DFSClient: Created token for jimenez: HDFS_DELEGATION_TOKEN owner=jimenez@SATYAR-LENKA.TX, renewer=yarn, realUser=, issueDate=1507920734406, maxDate=1508525534406, sequenceNumber=1, masterKeyId=2 on 172.31.12.173:8020
	17/10/13 18:52:14 INFO security.TokenCache: Got dt for hdfs://ip-172-31-12-173.us-west-2.compute.internal:8020; Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.12.173:8020, Ident: (token for jimenez: HDFS_DELEGATION_TOKEN owner=jimenez@SATYAR-LENKA.TX, renewer=yarn, realUser=, issueDate=1507920734406, maxDate=1508525534406, sequenceNumber=1, masterKeyId=2)
	17/10/13 18:52:14 INFO input.FileInputFormat: Total input paths to process : 8
	Spent 367ms computing base-splits.
	Spent 4ms computing TeraScheduler splits.
	Computing input splits took 371ms
	Sampling 10 splits of 104
	Making 8 from 100000 sampled records
	Computing parititions took 828ms
	Spent 1202ms computing partitions.
	17/10/13 18:52:15 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-12-173.us-west-2.compute.internal/172.31.12.173:8032
	17/10/13 18:52:15 INFO mapreduce.JobSubmitter: number of splits:104
	17/10/13 18:52:16 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1507920504084_0001
	17/10/13 18:52:16 INFO mapreduce.JobSubmitter: Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.12.173:8020, Ident: (token for jimenez: HDFS_DELEGATION_TOKEN owner=jimenez@SATYAR-LENKA.TX, renewer=yarn, realUser=, issueDate=1507920734406, maxDate=1508525534406, sequenceNumber=1, masterKeyId=2)
	17/10/13 18:52:17 INFO impl.YarnClientImpl: Submitted application application_1507920504084_0001
	17/10/13 18:52:17 INFO mapreduce.Job: The url to track the job: http://ip-172-31-12-173.us-west-2.compute.internal:8088/proxy/application_1507920504084_0001/
	17/10/13 18:52:17 INFO mapreduce.Job: Running job: job_1507920504084_0001
	17/10/13 18:52:27 INFO mapreduce.Job: Job job_1507920504084_0001 running in uber mode : false
	17/10/13 18:52:27 INFO mapreduce.Job:  map 0% reduce 0%
	17/10/13 18:52:35 INFO mapreduce.Job:  map 1% reduce 0%
	17/10/13 18:52:41 INFO mapreduce.Job:  map 3% reduce 0%
	17/10/13 18:52:42 INFO mapreduce.Job:  map 6% reduce 0%
	17/10/13 18:52:45 INFO mapreduce.Job:  map 9% reduce 0%
	17/10/13 18:52:49 INFO mapreduce.Job:  map 11% reduce 0%
	17/10/13 18:52:50 INFO mapreduce.Job:  map 13% reduce 0%
	17/10/13 18:52:57 INFO mapreduce.Job:  map 14% reduce 0%
	17/10/13 18:52:58 INFO mapreduce.Job:  map 17% reduce 0%
	17/10/13 18:52:59 INFO mapreduce.Job:  map 19% reduce 0%
	17/10/13 18:53:00 INFO mapreduce.Job:  map 21% reduce 0%
	17/10/13 18:53:03 INFO mapreduce.Job:  map 22% reduce 0%
	17/10/13 18:53:08 INFO mapreduce.Job:  map 24% reduce 0%
	17/10/13 18:53:09 INFO mapreduce.Job:  map 26% reduce 0%
	17/10/13 18:53:10 INFO mapreduce.Job:  map 30% reduce 0%
	17/10/13 18:53:17 INFO mapreduce.Job:  map 33% reduce 0%
	17/10/13 18:53:18 INFO mapreduce.Job:  map 35% reduce 0%
	17/10/13 18:53:20 INFO mapreduce.Job:  map 36% reduce 0%
	17/10/13 18:53:21 INFO mapreduce.Job:  map 38% reduce 0%
	17/10/13 18:53:26 INFO mapreduce.Job:  map 40% reduce 0%
	17/10/13 18:53:27 INFO mapreduce.Job:  map 42% reduce 0%
	17/10/13 18:53:31 INFO mapreduce.Job:  map 44% reduce 0%
	17/10/13 18:53:32 INFO mapreduce.Job:  map 46% reduce 0%
	17/10/13 18:53:34 INFO mapreduce.Job:  map 48% reduce 0%
	17/10/13 18:53:36 INFO mapreduce.Job:  map 50% reduce 0%
	17/10/13 18:53:38 INFO mapreduce.Job:  map 51% reduce 0%
	17/10/13 18:53:42 INFO mapreduce.Job:  map 52% reduce 0%
	17/10/13 18:53:43 INFO mapreduce.Job:  map 54% reduce 0%
	17/10/13 18:53:44 INFO mapreduce.Job:  map 58% reduce 0%
	17/10/13 18:53:45 INFO mapreduce.Job:  map 59% reduce 0%
	17/10/13 18:53:52 INFO mapreduce.Job:  map 63% reduce 0%
	17/10/13 18:53:53 INFO mapreduce.Job:  map 64% reduce 0%
	17/10/13 18:53:54 INFO mapreduce.Job:  map 66% reduce 0%
	17/10/13 18:54:00 INFO mapreduce.Job:  map 67% reduce 0%
	17/10/13 18:54:01 INFO mapreduce.Job:  map 68% reduce 0%
	17/10/13 18:54:02 INFO mapreduce.Job:  map 69% reduce 0%
	17/10/13 18:54:03 INFO mapreduce.Job:  map 71% reduce 0%
	17/10/13 18:54:04 INFO mapreduce.Job:  map 72% reduce 0%
	17/10/13 18:54:06 INFO mapreduce.Job:  map 74% reduce 0%
	17/10/13 18:54:07 INFO mapreduce.Job:  map 75% reduce 0%
	17/10/13 18:54:09 INFO mapreduce.Job:  map 76% reduce 0%
	17/10/13 18:54:10 INFO mapreduce.Job:  map 77% reduce 0%
	17/10/13 18:54:12 INFO mapreduce.Job:  map 79% reduce 0%
	17/10/13 18:54:13 INFO mapreduce.Job:  map 80% reduce 0%
	17/10/13 18:54:14 INFO mapreduce.Job:  map 81% reduce 0%
	17/10/13 18:54:16 INFO mapreduce.Job:  map 83% reduce 0%
	17/10/13 18:54:17 INFO mapreduce.Job:  map 84% reduce 0%
	17/10/13 18:54:18 INFO mapreduce.Job:  map 85% reduce 0%
	17/10/13 18:54:20 INFO mapreduce.Job:  map 86% reduce 0%
	17/10/13 18:54:21 INFO mapreduce.Job:  map 88% reduce 0%
	17/10/13 18:54:26 INFO mapreduce.Job:  map 89% reduce 0%
	17/10/13 18:54:27 INFO mapreduce.Job:  map 90% reduce 0%
	17/10/13 18:54:29 INFO mapreduce.Job:  map 90% reduce 9%
	17/10/13 18:54:30 INFO mapreduce.Job:  map 91% reduce 9%
	17/10/13 18:54:32 INFO mapreduce.Job:  map 93% reduce 15%
	17/10/13 18:54:35 INFO mapreduce.Job:  map 93% reduce 16%
	17/10/13 18:54:36 INFO mapreduce.Job:  map 95% reduce 16%
	17/10/13 18:54:37 INFO mapreduce.Job:  map 96% reduce 16%
	17/10/13 18:54:38 INFO mapreduce.Job:  map 97% reduce 16%
	17/10/13 18:54:41 INFO mapreduce.Job:  map 99% reduce 16%
	17/10/13 18:54:42 INFO mapreduce.Job:  map 100% reduce 16%
	17/10/13 18:54:44 INFO mapreduce.Job:  map 100% reduce 33%
	17/10/13 18:54:47 INFO mapreduce.Job:  map 100% reduce 35%
	17/10/13 18:54:48 INFO mapreduce.Job:  map 100% reduce 36%
	17/10/13 18:54:50 INFO mapreduce.Job:  map 100% reduce 43%
	17/10/13 18:54:52 INFO mapreduce.Job:  map 100% reduce 47%
	17/10/13 18:54:54 INFO mapreduce.Job:  map 100% reduce 59%
	17/10/13 18:54:56 INFO mapreduce.Job:  map 100% reduce 62%
	17/10/13 18:54:57 INFO mapreduce.Job:  map 100% reduce 67%
	17/10/13 18:54:59 INFO mapreduce.Job:  map 100% reduce 74%
	17/10/13 18:55:00 INFO mapreduce.Job:  map 100% reduce 81%
	17/10/13 18:55:01 INFO mapreduce.Job:  map 100% reduce 82%
	17/10/13 18:55:02 INFO mapreduce.Job:  map 100% reduce 84%
	17/10/13 18:55:03 INFO mapreduce.Job:  map 100% reduce 87%
	17/10/13 18:55:04 INFO mapreduce.Job:  map 100% reduce 88%
	17/10/13 18:55:05 INFO mapreduce.Job:  map 100% reduce 94%
	17/10/13 18:55:06 INFO mapreduce.Job:  map 100% reduce 95%
	17/10/13 18:55:08 INFO mapreduce.Job:  map 100% reduce 97%
	17/10/13 18:55:11 INFO mapreduce.Job:  map 100% reduce 98%
	17/10/13 18:55:14 INFO mapreduce.Job:  map 100% reduce 99%
	17/10/13 18:55:15 INFO mapreduce.Job:  map 100% reduce 100%
	17/10/13 18:55:16 INFO mapreduce.Job: Job job_1507920504084_0001 completed successfully
	17/10/13 18:55:16 INFO mapreduce.Job: Counters: 49
		File System Counters
			FILE: Number of bytes read=2912223207
			FILE: Number of bytes written=5778124229
			FILE: Number of read operations=0
			FILE: Number of large read operations=0
			FILE: Number of write operations=0
			HDFS: Number of bytes read=6553615704
			HDFS: Number of bytes written=6553600000
			HDFS: Number of read operations=336
			HDFS: Number of large read operations=0
			HDFS: Number of write operations=16
		Job Counters 
			Launched map tasks=104
			Launched reduce tasks=8
			Data-local map tasks=104
			Total time spent by all maps in occupied slots (ms)=854104
			Total time spent by all reduces in occupied slots (ms)=262557
			Total time spent by all map tasks (ms)=854104
			Total time spent by all reduce tasks (ms)=262557
			Total vcore-seconds taken by all map tasks=854104
			Total vcore-seconds taken by all reduce tasks=262557
			Total megabyte-seconds taken by all map tasks=874602496
			Total megabyte-seconds taken by all reduce tasks=268858368
		Map-Reduce Framework
			Map input records=65536000
			Map output records=65536000
			Map output bytes=6684672000
			Map output materialized bytes=2851934348
			Input split bytes=15704
			Combine input records=0
			Combine output records=0
			Reduce input groups=65536000
			Reduce shuffle bytes=2851934348
			Reduce input records=65536000
			Reduce output records=65536000
			Spilled Records=131072000
			Shuffled Maps =832
			Failed Shuffles=0
			Merged Map outputs=832
			GC time elapsed (ms)=15578
			CPU time spent (ms)=704850
			Physical memory (bytes) snapshot=58216964096
			Virtual memory (bytes) snapshot=176942047232
			Total committed heap usage (bytes)=65596293120
		Shuffle Errors
			BAD_ID=0
			CONNECTION=0
			IO_ERROR=0
			WRONG_LENGTH=0
			WRONG_MAP=0
			WRONG_REDUCE=0
		File Input Format Counters 
			Bytes Read=6553600000
		File Output Format Counters 
			Bytes Written=6553600000
	17/10/13 18:55:16 INFO terasort.TeraSort: done
	[jimenez@ip-172-31-3-113 centos]$ 
	
</code></pre>