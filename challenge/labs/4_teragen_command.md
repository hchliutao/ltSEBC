[hdfs@node01 hadoop-0.20-mapreduce]$ time hadoop jar hadoop-examples.jar teragen -Ddfs.block.size=33554432 51200000 /user/jetli/tgen32<br>
16/05/20 10:24:25 INFO client.RMProxy: Connecting to ResourceManager at node01/192.168.60.71:8032<br>
16/05/20 10:24:26 INFO terasort.TeraSort: Generating 51200000 using 2<br>
16/05/20 10:24:26 INFO mapreduce.JobSubmitter: number of splits:2<br>
16/05/20 10:24:26 INFO Configuration.deprecation: dfs.block.size is deprecated. Instead, use dfs.blocksize<br>
16/05/20 10:24:26 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1463709302758_0001<br>
16/05/20 10:24:27 INFO impl.YarnClientImpl: Submitted application application_1463709302758_0001<br>
16/05/20 10:24:27 INFO mapreduce.Job: The url to track the job: http://node01:8088/proxy/application_1463709302758_0001/<br>
16/05/20 10:24:27 INFO mapreduce.Job: Running job: job_1463709302758_0001<br>
16/05/20 10:24:36 INFO mapreduce.Job: Job job_1463709302758_0001 running in uber mode : false<br>
16/05/20 10:24:36 INFO mapreduce.Job:  map 0% reduce 0%<br>
16/05/20 10:24:50 INFO mapreduce.Job:  map 10% reduce 0%<br>
16/05/20 10:24:53 INFO mapreduce.Job:  map 18% reduce 0%<br>
16/05/20 10:24:56 INFO mapreduce.Job:  map 25% reduce 0%<br>
16/05/20 10:24:59 INFO mapreduce.Job:  map 32% reduce 0%<br>
16/05/20 10:25:05 INFO mapreduce.Job:  map 38% reduce 0%<br>
16/05/20 10:25:18 INFO mapreduce.Job:  map 40% reduce 0%<br><br>
16/05/20 10:25:27 INFO mapreduce.Job:  map 41% reduce 0%<br>
16/05/20 10:25:34 INFO mapreduce.Job:  map 42% reduce 0%<br>
16/05/20 10:25:49 INFO mapreduce.Job:  map 43% reduce 0%<br>
16/05/20 10:25:57 INFO mapreduce.Job:  map 44% reduce 0%<br>
16/05/20 10:25:59 INFO mapreduce.Job:  map 45% reduce 0%<br>
16/05/20 10:26:06 INFO mapreduce.Job:  map 46% reduce 0%<br>
16/05/20 10:26:13 INFO mapreduce.Job:  map 47% reduce 0%<br>
16/05/20 10:26:16 INFO mapreduce.Job:  map 48% reduce 0%<br>
16/05/20 10:26:22 INFO mapreduce.Job:  map 49% reduce 0%<br>
16/05/20 10:26:25 INFO mapreduce.Job:  map 50% reduce 0%<br>
16/05/20 10:26:31 INFO mapreduce.Job:  map 51% reduce 0%<br>
16/05/20 10:26:34 INFO mapreduce.Job:  map 52% reduce 0%<br>
16/05/20 10:26:37 INFO mapreduce.Job:  map 53% reduce 0%<br>
16/05/20 10:26:40 INFO mapreduce.Job:  map 54% reduce 0%<br>
16/05/20 10:26:43 INFO mapreduce.Job:  map 56% reduce 0%<br>
16/05/20 10:26:46 INFO mapreduce.Job:  map 58% reduce 0%<br>
16/05/20 10:26:49 INFO mapreduce.Job:  map 59% reduce 0%<br>
16/05/20 10:26:52 INFO mapreduce.Job:  map 60% reduce 0%<br>
16/05/20 10:26:55 INFO mapreduce.Job:  map 61% reduce 0%<br>
16/05/20 10:27:01 INFO mapreduce.Job:  map 62% reduce 0%<br>
16/05/20 10:27:07 INFO mapreduce.Job:  map 63% reduce 0%<br>
16/05/20 10:27:16 INFO mapreduce.Job:  map 64% reduce 0%<br>
16/05/20 10:27:22 INFO mapreduce.Job:  map 66% reduce 0%<br>
16/05/20 10:27:25 INFO mapreduce.Job:  map 69% reduce 0%<br>
16/05/20 10:27:28 INFO mapreduce.Job:  map 71% reduce 0%<br>
16/05/20 10:27:31 INFO mapreduce.Job:  map 73% reduce 0%<br>
16/05/20 10:27:34 INFO mapreduce.Job:  map 76% reduce 0%<br>
16/05/20 10:27:40 INFO mapreduce.Job:  map 77% reduce 0%<br>
16/05/20 10:27:46 INFO mapreduce.Job:  map 79% reduce 0%<br>
16/05/20 10:27:49 INFO mapreduce.Job:  map 80% reduce 0%<br>
16/05/20 10:27:56 INFO mapreduce.Job:  map 81% reduce 0%<br>
16/05/20 10:27:59 INFO mapreduce.Job:  map 82% reduce 0%<br>
16/05/20 10:28:05 INFO mapreduce.Job:  map 83% reduce 0%<br>
16/05/20 10:28:06 INFO mapreduce.Job:  map 84% reduce 0%<br>
16/05/20 10:28:08 INFO mapreduce.Job:  map 85% reduce 0%<br>
16/05/20 10:28:11 INFO mapreduce.Job:  map 87% reduce 0%<br>
16/05/20 10:28:14 INFO mapreduce.Job:  map 88% reduce 0%<br>
16/05/20 10:28:17 INFO mapreduce.Job:  map 89% reduce 0%<br>
16/05/20 10:28:18 INFO mapreduce.Job:  map 90% reduce 0%<br>
16/05/20 10:28:20 INFO mapreduce.Job:  map 91% reduce 0%<br>
16/05/20 10:28:21 INFO mapreduce.Job:  map 92% reduce 0%<br>
16/05/20 10:28:23 INFO mapreduce.Job:  map 93% reduce 0%<br>
16/05/20 10:28:24 INFO mapreduce.Job:  map 94% reduce 0%<br>
16/05/20 10:28:27 INFO mapreduce.Job:  map 95% reduce 0%<br>
16/05/20 10:28:29 INFO mapreduce.Job:  map 96% reduce 0%<br>
16/05/20 10:28:35 INFO mapreduce.Job:  map 97% reduce 0%<br>
16/05/20 10:28:44 INFO mapreduce.Job:  map 98% reduce 0%<br>
16/05/20 10:29:00 INFO mapreduce.Job:  map 99% reduce 0%<br>
16/05/20 10:29:02 INFO mapreduce.Job:  map 100% reduce 0%<br>
16/05/20 10:29:05 INFO mapreduce.Job: Job job_1463709302758_0001 completed successfully<br>
16/05/20 10:29:05 INFO mapreduce.Job: Counters: 31<br>
	File System Counters<br>
		FILE: Number of bytes read=0<br>
		FILE: Number of bytes written=229822<br>
		FILE: Number of read operations=0<br>
		FILE: Number of large read operations=0<br>
		FILE: Number of write operations=0<br>
		HDFS: Number of bytes read=170<br>
		HDFS: Number of bytes written=5120000000<br>
		HDFS: Number of read operations=8<br>
		HDFS: Number of large read operations=0<br>
		HDFS: Number of write operations=4<br>
	Job Counters <br>
		Launched map tasks=2<br>
		Other local map tasks=2<br>
		Total time spent by all maps in occupied slots (ms)=492655<br>
		Total time spent by all reduces in occupied slots (ms)=0<br>
		Total time spent by all map tasks (ms)=492655<br>
		Total vcore-seconds taken by all map tasks=492655<br>
		Total megabyte-seconds taken by all map tasks=504478720<br>
	Map-Reduce Framework<br>
		Map input records=51200000<br>
		Map output records=51200000<br>
		Input split bytes=170<br>
		Spilled Records=0<br>
		Failed Shuffles=0<br>
		Merged Map outputs=0<br>
		GC time elapsed (ms)=1017<br>
		CPU time spent (ms)=142720<br>
		Physical memory (bytes) snapshot=462442496<br>
		Virtual memory (bytes) snapshot=3134517248<br>
		Total committed heap usage (bytes)=255852544<br>
	org.apache.hadoop.examples.terasort.TeraGen$Counters<br>
		CHECKSUM=109963291816450258<br>
	File Input Format Counters <br>
		Bytes Read=0<br>
	File Output Format Counters <br>
		Bytes Written=5120000000<br>

real	4m43.557s<br>
user	0m7.691s<br>
sys	0m0.911s<br>
[hdfs@node01 hadoop-0.20-mapreduce]$ <br>

----------------------------------<br>


[root@node01 ~]# hdfs dfs -ls /user/jetli/tgen32<br>
Found 3 items<br>
-rw-r--r--   3 hdfs supergroup          0 2016-05-20 10:29 /user/jetli/tgen32/_SUCCESS<br>
-rw-r--r--   3 hdfs supergroup 2560000000 2016-05-20 10:28 /user/jetli/tgen32/part-m-00000<br>
-rw-r--r--   3 hdfs supergroup 2560000000 2016-05-20 10:29 /user/jetli/tgen32/part-m-00001<br>
[root@node01 ~]# <br>
