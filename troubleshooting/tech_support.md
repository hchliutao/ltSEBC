Troubleshooting
Enabling field partners
Using documentation, getting assistance
Defining problems, bugs, and customer issues
Troubleshooting methodology
Preparing for Friday challenges
 General Resources to Have

ASF account for reporting/reviewing bugs
Cloudera Connect - partner portal
Most of our consultants use Github to share code.
 Documentation & Support

We must review all materials customers can access
Follow and participate in Cloudera's forums
Always ask which CM/CDH versions are in use?
Documentation starts here
Review all Technical Service Bulletins
Learn to use the Diagnostic Bundle Collector
 Defining Problems, Bugs, Customer Issues

 Troubleshooting Wisdom

Potential measures by how much you lost -- my college track coach

Fixing a recurring or well-known problem quickly is a common pitfall
You need a method you can recite when you encounter new/unfamiliar territory
To remind yourself what you know
To recall tools that can tell you what you don't know
To remember tools don't solve problems, they help reveal them
To write down what you've learned so you can share it
 Methodology: Guidance

We have many technologies to consider. A good general-purpose book for articulating your practice is Debugging, by David J. Agans. These nine points are the focus:

Understand the System
Check the Plug
Divide and Conquer
Make It Fail
Quit Thinking and Look
Change One Thing at a Time
Keep an Audit Trail
Get a Fresh View
If You Didn't Fix It, It Ain't Fixed
Note: Apply #7 to documenting your fix, and adding it to the community's knowledge

 Pro Tip: Find Patches by Release

Review the change log
Search by CDH project -- put JIRA identifier in double quotes
Grep the code! For example, to find FLUME-2245 in CDH 5.1.x:
$ git clone https://github.com/cloudera/flume-ng 
$ cd flume-ng 
$ git branch -a 
$ git log origin/cdh5-1.4.0_5.0.2 | grep 'FLUME-2245' 
$ git log origin/cdh5-1.4.0_5.0.3 | grep 'FLUME-2245' 
FLUME-2245. Pre-close flush failure can cause HDFS Sinks to not process events
Getting patch updates: $ git fetch origin 
 Pro Action: Finding Patches with Better Tools

Fork/review Jarcec Cecho's gb-grep tool
Doesn't require branch-specific search <!-- Use Miklos Christine's instructions on using Jarcec's script) -->
Usage:
$ git clone http://github.mtv.cloudera.com/CDH/hadoop
$ cd hadoop/
$ gb-grep "HDFS-7575"
Sample output line:  Searching for HDFS-7575 hadoop-hdfs-project: f1a2fce5b3c21e3335f99fe210edbb1f9c7bb29f HDFS-7575. Upgrade should generate a unique storage ID for each volume. (Contributed by Arpit Agarwal)
 Friday Challenges

Read through the challenges in this document
These challenges were part of the last delivery
Notice the following
The focus of each challenge
The details in the instructions
The submission requirements
The deadlines
 Lab: Review time

You should:
Review the challenges.
Review your class notes
Repeat or continue lab work
Prepare new instances for tomorrow's challenges
You should not:
Write scripts to automate tomorrow's work -- waste of time
Install software to your new instances
