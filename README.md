# sparkjobs

++++ To Build ++
sbt assembly 
++++++

#####
/apache/spark-beta/bin/spark-submit   --master yarn  --queue hdlq-data-default  --class "SparkSqlJob" rajesh/SparkSqlJobs-assembly-0.1.jar
####


  /apache/releases/spark-2.3.1-bin-hadoop2.7/bin/spark-submit  --master yarn  --conf spark.ui.port=5151  --queue hdlq-data-default  --num-executors 3 --driver-memory 512m --executor-memory 512m --executor-cores 1   --class "SparkSqlJob" /tmp/SparkSqlJobs-assembly-0.1.jar
#####
