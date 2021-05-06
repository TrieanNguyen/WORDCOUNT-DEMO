# WORDCOUNT-DEMO
## INSTRODUCTION
* Run demo Wordcount to performances Map-Reduce
* In this demo, count the number of times HCMUTE students won scholarships from 2018 to 2020
* Project include: map.java, reduce.java, runner.java, data.txt
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
