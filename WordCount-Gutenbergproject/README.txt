**Before running this code make sure all the 6 files are present in assignment1 directory
Note: Stop words are being fetched from the following: hdfs://cshadoop1/user/lps160130/stopwords.txt

1. Unzip wordcount.zip and remember the location.

2. Import the project into Eclipse for Java EE. For this, go to File -> Import and choose "Existing Maven Projects".

3.Build the project by right clicking on the pom.xml file to generate wordcount-0.0.1-SNAPSHOT

4. Change to the Remote System Explorer (RSE) perspective by clicking Window -> Perspective -> Open Perspective -> Remote System Explorer.

5. Connect to the UTD cluster and then copy the jar file that you obtained in step-3 to the "My Home" directory of the cluster.

6. SSH into the cs6360.utdallas.edu node using netid and run the following command to execute the jar file:

hadoop jar wordcount-0.0.1-SNAPSHOT.jar wordcount.wordcount.ModifiedWordCount hdfs://cshadoop1/user/sxr161730/assignment1 hdfs://cshadoop1/user/sxr161730/output27

Note: we have included the output file with name 'output'. open it with notepad++ to view the results