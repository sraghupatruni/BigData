Goal: To perform MapReduce job on Movie Lens Dataset to calculate average rating of each movie

1. Unzip movielens.zip and remember the location.

2. Import the project into Eclipse for Java EE. For this, go to File -> Import and choose "Existing Maven Projects".


3.Build the project by right clicking on the pom.xml file to generate movielens-0.0.1-SNAPSHOT

4. Change to the Remote System Explorer (RSE) perspective by clicking Window -> Perspective -> Open Perspective -> Remote System Explorer.

5. Connect to the UTD cluster and then copy the jar file that you obtained in step-3 to the "My Home" directory of the cluster.

6. SSH into the cs6360.utdallas.edu node using netid and run the following command to execute the jar file:

hadoop jar movielens-0.0.1-SNAPSHOT.jar averagemovierating.movielens.AvgRating hdfs://cshadoop1/movielens/ratings.csv hdfs://cshadoop1/user/sxr161730/movieoutput

Note: We have included the output in this directory with name 'output'. open it with notepad++ to view the results 
