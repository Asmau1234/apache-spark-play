playing with Apache spark with scala. 

To use, find inputs.txt in the app directory. 

Before serve, create your output folder in the desired directory.

To run in spark shell: `$spark-shell`

compile: `$ scalac -classpath "spark-core_2.10-1.3.0.jar:/usr/local/spark/lib/spark-assembly-1.4.0-hadoop2.6.0.jar" SparkWordCount.scala`

create jar: `jar -cvf wordcount.jar SparkWordCount*.class spark-core_2.10-1.3.0.jar/usr/local/spark/lib/spark-assembly-1.4.0-hadoop2.6.0.jar`

suubmit: `spark-submit --class SparkWordCount --master local wordcount.jar`

