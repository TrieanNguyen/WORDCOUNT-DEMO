# WORDCOUNT-DEMO
## INSTRODUCTION
* Run demo Wordcount to performances Map-Reduce
* In this demo, count the number of times HCMUTE students won scholarships from 2018 to 2020
* Project include: map.java, reduce.java, runner.java, data.txt
## INSTALL PROJECT WORD-COUNT
* Install project wordcount, run command: [WordCount_Demo](https://github.com/TrieanNguyen/WORDCOUNT-DEMO.git)
## RUN WORDCOUNT BY HADOOP 

* STEP 1: Create folder to Demo
    * mkdir Demo
* STEP 2: Package the java classes(map.java, reduce.java. runner.java) and hadoop-mapreduce and hadoop-common libraries in a jar file:
    * javac -cp $HADOOP_HOME/share/hadoop/common/hadoop-common-2.7.7.jar:$HADOOP_HOME/share/hadoop/mapreduce/
      hadoop-mapreduce-client-core-2.7.7.jar:operation/:.                                         -d Demo map.java
    * javac -cp $HADOOP_HOME/share/hadoop/common/hadoop-common-2.7.7.jar:$HADOOP_HOME/share/hadoop/mapreduce/
      hadoop-mapreduce-client-core-2.7.7.jar:operation/:.                                         -d Demo reduce.java
    * javac -cp $HADOOP_HOME/share/hadoop/common/hadoop-common-2.7.7.jar:$HADOOP_HOME/share/hadoop/mapreduce/
      hadoop-mapreduce-client-core-2.7.7.jar:operation/:.                                         -d Demo runner.java
* STEP 3: Create file Jar:
    * Run command:  jar -cvf Wordcount.jar -C Demo/ .
* STEP 4: Run file jar:
    * Run command:  hadoop jar wordcount.jar Packedemo.runner.java input output 
    
