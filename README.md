# healthcare_incubyte_asgn
Performed ETL on covid data


Tools and technologies used:

Operating system:  
Ubuntu 20.04.3 LTS


Apache Hadoop:
Version: 
hadoop-3.3.1

It provides a software framework for distributed storage and processing of big data using the MapReduce programming model.

Apache Hive:
Version: 
hive-2.3.8

Apache Hive is a data warehouse software project built on top of Apache Hadoop for providing data query and analysis. Hive gives an SQL-like interface to query data stored in various databases and file systems that integrate with Hadoop.

Steps followed during the process:

1)Open the terminal and start the hadoop cluster by giving following commands:
'''start-dfs.sh
start-yarn.sh'''

2)Check the namenode and datanodes are up and running by giving following command:
'''jps'''

3)Start Hive from where its installed:
'''./bin/hive'''

4)Execute the commands provided in hive_queries.txt file

5)Check the location of the partitioned table by giving following command:

Note: Here we are using the CLI of ubuntu
'''hdfs dfs -ls /user/hive/warehouse/transformation.db/country_part'''

6)Creating output directory for retrieving the data

'''mkdir /home/sabby/incu_covid_data'''
Note: Here the output will be stored in 'incu_covid_data' directory

