16/05/18 12:04:11 INFO client.RMProxy: Connecting to ResourceManager at node01/192.168.60.71:8032
16/05/18 12:04:12 INFO terasort.TeraSort: Generating 10000000 using 2
16/05/18 12:04:12 INFO mapreduce.JobSubmitter: number of splits:2
16/05/18 12:04:12 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1463533040225_0001
16/05/18 12:04:13 INFO impl.YarnClientImpl: Submitted application application_1463533040225_0001
16/05/18 12:04:13 INFO mapreduce.Job: The url to track the job: http://node01:8088/proxy/application_1463533040225_0001/
16/05/18 12:04:13 INFO mapreduce.Job: Running job: job_1463533040225_0001
16/05/18 12:04:21 INFO mapreduce.Job: Job job_1463533040225_0001 running in uber mode : false
16/05/18 12:04:21 INFO mapreduce.Job:  map 0% reduce 0%
16/05/18 12:04:34 INFO mapreduce.Job:  map 65% reduce 0%
16/05/18 12:04:36 INFO mapreduce.Job:  map 80% reduce 0%
16/05/18 12:04:37 INFO mapreduce.Job:  map 100% reduce 0%
16/05/18 12:04:37 INFO mapreduce.Job: Job job_1463533040225_0001 completed successfully
16/05/18 12:04:38 INFO mapreduce.Job: Counters: 31
	File System Counters
		FILE: Number of bytes read=0
		FILE: Number of bytes written=233576
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=167
		HDFS: Number of bytes written=1000000000
		HDFS: Number of read operations=8
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=4
	Job Counters 
		Launched map tasks=2
		Other local map tasks=2
		Total time spent by all maps in occupied slots (ms)=26573
		Total time spent by all reduces in occupied slots (ms)=0
		Total time spent by all map tasks (ms)=26573
		Total vcore-seconds taken by all map tasks=26573
		Total megabyte-seconds taken by all map tasks=27210752
	Map-Reduce Framework
		Map input records=10000000
		Map output records=10000000
		Input split bytes=167
		Spilled Records=0
		Failed Shuffles=0
		Merged Map outputs=0
		GC time elapsed (ms)=226
		CPU time spent (ms)=26420
		Physical memory (bytes) snapshot=747204608
		Virtual memory (bytes) snapshot=3098927104
		Total committed heap usage (bytes)=657457152
	org.apache.hadoop.examples.terasort.TeraGen$Counters
		CHECKSUM=21472776955442690
	File Input Format Counters 
		Bytes Read=0
	File Output Format Counters 
		Bytes Written=1000000000
