# HDFS Basic Commands
- HDFS is the primary or major component of the Hadoop ecosystem which is responsible for storing large data sets of structured or unstructured data across various nodes and thereby maintaining the metadata in the form of log files.

## Starting the Hadoop Services
- D:\software\Installation\BDA\hadoop-3.2.1\sbin>start-all.cmd

## To check the Hadoop services are up
- D:\software\Installation\BDA\hadoop-3.2.1\sbin>jps
#
    3892 ResourceManager
    7480 DataNode
    7672 Jps
    4508 NodeManager
    652 NameNode
    
## mkdir: To create a directory.
- D:\software\Installation\BDA\hadoop-3.2.1\sbin>hdfs dfs -mkdir /creatingDir

## ls: This command is used to list all the files. Use lsr for recursive approach. It is useful when we want a hierarchy of a folder.
- D:\software\Installation\BDA\hadoop-3.2.1\sbin>hdfs dfs -ls /
# 
    Found 4 items
    drwxr-xr-x   - Shalini supergroup          0 2021-05-03 18:51 /basicComm
    drwxr-xr-x   - Shalini supergroup          0 2021-05-03 19:13 /creatingDir
    drwxr-xr-x   - Shalini supergroup          0 2021-05-03 19:01 /sample
    drwxr-xr-x   - Shalini supergroup          0 2021-05-03 19:01 /sampleCopied
- D:\software\Installation\BDA\hadoop-3.2.1\sbin>hdfs dfs -ls /basicComm
#
    Found 4 items
    drwxr-xr-x   - Shalini supergroup          0 2021-05-03 18:24 /basicComm/$RECYCLE.BIN
    drwxr-xr-x   - Shalini supergroup          0 2021-05-03 18:47 /basicComm/Desktop
    -rw-r--r--   1 Shalini supergroup          9 2021-05-03 18:51 /basicComm/cutAndPaste.txt
    -rw-r--r--   1 Shalini supergroup          0 2021-05-03 18:28 /basicComm/testFile.txt
    
## copyFromLocal (or) put: To copy files/folders from local file system to hdfs store.
- D:\software\Installation\BDA\hadoop-3.2.1\sbin>hdfs dfs -copyFromLocal C:\Users\Shalini\Desktop\employee.txt \creatingDir
#
    2021-05-03 19:20:43,690 INFO sasl.SaslDataTransferClient: SASL encryption trust check: localHostTrusted = false, remoteHostTrusted = false
- D:\software\Installation\BDA\hadoop-3.2.1\sbin>hdfs dfs -ls \creatingDir
#
    Found 1 items
    -rw-r--r--   1 Shalini supergroup       7196 2021-05-03 19:20 /creatingDir/employee.txt


