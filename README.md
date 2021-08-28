# InvertedIndexMR
Performing Inverted Index on Mahabharta text file.

1. export HADOOP_CLASSPATH=$(hadoop classpath)
 
2. hadoop fs -mkdir /InvertedIndexMR

3.hadoop fs -mkdir /InvertedIndexMR/Input

4. hadoop fs -put '/home/hadoop/Desktop/InvertedIndexMR/Data' /InvertedIndexMR/Input

5.cd /home/hadoop/Desktop/InvertedIndexMR

6.chmod 777 InvertedIndexMR (Change permissions of all files)

7. javac -classpath  ${HADOOP_CLASSPATH} -d 'foldernameWhereYouWantToStoreClassFiles' 'JavaProgramPath'

8. jar -cvf NameForTheJarFile -C ClassFolderName/ .

9. hadoop jar '/home/hadoop/Desktop/InvertedIndexMr/JarFilename' InvertedIndexMR /InvertedIndexMR/Input/Data /InvertedIndexMR/Output

10. hadoop dfs -cat /InvertedIndexMR/Output/*
