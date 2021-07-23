# WORDCOUNT-DEMO
## INSTRODUCTION
* Run demo Wordcount to performances Map-Reduce
* In this demo, count the number of times HCMUTE students won scholarships from 2018 to 2020
* Project include: map.java, reduce.java, runner.java, data.txt
* Use file data.txt together run Map-Reduce on Hadoop and Spark
* Target for Project: Use Word-count to compare Map-Reduce on Hadoop and Map-Reduce on Spark.

## INSTALL PROJECT WORD-COUNT
* Install project wordcount, run command: [WordCount_Demo](https://github.com/TrieanNguyen/WORDCOUNT-DEMO.git)
## RUN WORDCOUNT BY HADOOP 

* STEP 1: Create folder to Demo
    * mkdir Demo
* STEP 2: Package the java classes(map.java, reduce.java. runner.java) and hadoop-mapreduce and hadoop-common libraries in a jar file:
    * javac -cp $HADOOP_HOME/share/hadoop/common/hadoop-common-2.7.7.jar:$HADOOP_HOME/share/hadoop/mapreduce/hadoop-mapreduce-client-core-2.7.7.jar:Demo/:.                                         -d Demo map.java
    * javac -cp $HADOOP_HOME/share/hadoop/common/hadoop-common-2.7.7.jar:$HADOOP_HOME/share/hadoop/mapreduce/hadoop-mapreduce-client-core-2.7.7.jar:Demo/:.                                         -d Demo reduce.java
    * javac -cp $HADOOP_HOME/share/hadoop/common/hadoop-common-2.7.7.jar:$HADOOP_HOME/share/hadoop/mapreduce/hadoop-mapreduce-client-core-2.7.7.jar:Demo/:.                                         -d Demo runner.java
* STEP 3: Create file Jar:
    * Run command:  jar -cvf Wordcount.jar -C Demo/ .
* STEP 4: Create input on hdfs:
    * Run command: hdfs dfs -mkdir -p input
* STEP 5: Put file data to folder input on HDFS
    * Run command: hdfs dfs -put /WORDCOUNT-DEMO/data.txt input
* STEP 6: Run file jar
    * Run command: hadoop jar Wordcount.jar PackageDemo.runner input output
* STEP 7: Read file output
    * Run command: hdfs dfs -cat output/part-00000
## RUN WORDCOUNT BY SPARK

* STEP 1: Push file jar to HDFS
    * Run command: hdfs dfs -put simple-project_2.12-1.0.jar
* STEP 2: Run file jar use mode spark-submit
    * Run command: spark-submit simple-project_2.12-1.0.jar
### Map-Reduce run on Spark faster Map-Reduce on Hadoop.
   
Here, you already finish demo Wordcount use Mapreduce, Gook Luck!!!!
    

    
