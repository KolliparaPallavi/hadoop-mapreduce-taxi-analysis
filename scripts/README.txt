

Pallavi Kollipara (s4015344)

Task1:

In Task1 I have created three files.
- Task1mapper.py, Task1reducer.py and Task1-run.sh. 
- first we have to copy the files from local to jumphost. 
- And second step is to copy the files from jumphost to master node. 
- And later make sure all the input (Trips.txt) files are in hdfs in the Input folder or not. 
- And copy jar file to master node as well.

Commands I used:

Copy to Jumphost:

scp -i s4015344-cosc2637.pem /Users/pallavikollipara/Desktop/rmit/sem3/Bigdata/Assignment1/Task1mapper.py jumphost:~/a1/

scp -i s4015344-cosc2637.pem /Users/pallavikollipara/Desktop/rmit/sem3/Bigdata/Assignment1/Task1reducer.py jumphost:~/a1/


scp -i s4015344-cosc2637.pem /Users/pallavikollipara/Desktop/rmit/sem3/Bigdata/Assignment1/Task1-run.sh jumphost:~/a1/

Copy to master node:

scp -i ~/s4015344-cosc2637.pem Task1mapper.py hadoop@s4015344.emr.cosc2637.route53.aws.rmit.edu.au:~/


scp -i ~/s4015344-cosc2637.pem Task1reducer.py hadoop@s4015344.emr.cosc2637.route53.aws.rmit.edu.au:~/

scp -i ~/s4015344-cosc2637.pem Task1-run.sh hadoop@s4015344.emr.cosc2637.route53.aws.rmit.edu.au:~/

Give execute permission for shell file. Use the command below.
chmod +x Task1-run.sh

And run the file 
./Task1-run.sh

Task2:

In Task2 I have created three files. 

- Task2mapper.py, Task2reducer.py and Task2-run.sh. 
- first we have to copy the files from local to jumphost. 
- And second step is to copy the files from jumphost to master node. 
- And later make sure all the input (Trips.txt and initialization.txt) files are in place. 
- And copy jar file to master node as well if its not there.

Commands I used:

Copy to jumphost:
scp -i s4015344-cosc2637.pem /Users/pallavikollipara/Desktop/rmit/sem3/Bigdata/Assignment1/Task2mapper.py jumphost:~/a1/

scp -i s4015344-cosc2637.pem /Users/pallavikollipara/Desktop/rmit/sem3/Bigdata/Assignment1/Task2reducer.py jumphost:~/a1/

scp -i s4015344-cosc2637.pem /Users/pallavikollipara/Desktop/rmit/sem3/Bigdata/Assignment1/Task2-run.sh jumphost:~/a1/

Copy to master node:

scp -i ~/s4015344-cosc2637.pem Task2-run.sh hadoop@s4015344.emr.cosc2637.route53.aws.rmit.edu.au:~/

scp -i ~/s4015344-cosc2637.pem Task2mapper.py hadoop@s4015344.emr.cosc2637.route53.aws.rmit.edu.au:~/

scp -i ~/s4015344-cosc2637.pem Task2reducer.py hadoop@s4015344.emr.cosc2637.route53.aws.rmit.edu.au:~/

Give execute permission for shell file. Use the command below.
chmod +x Task2-run.sh

And run the file
./Task2-run.sh

Task3:

In Task3 I have created 7 files. 
- Task3mapper1.py, Task3reducer1.py to do the join of two text files. 
- And Task3mapper2.py, Task3reducer2.py for doing the count operation. 
- And Task3mapper3.py, Task3reducer3.py for doing the sort operation. 
- And last file Task3-run.sh for executing the task. 
- first we have to copy the files from local to jumphost. 
- And second step is to copy the files from jumphost to master node. 
- And later make sure all the input Taxis.txt,Trips.txt files are in hdfs in the Input folder or not. 
- And copy jar file to master node as well if it is not there.


Comands I used:

Copy to jumphost:

scp -i s4015344-cosc2637.pem /Users/pallavikollipara/Desktop/rmit/sem3/Bigdata/Assignment1/Task3mapper1.py jumphost:~/a1/

scp -i s4015344-cosc2637.pem /Users/pallavikollipara/Desktop/rmit/sem3/Bigdata/Assignment1/Task3mapper2.py jumphost:~/a1/

scp -i s4015344-cosc2637.pem /Users/pallavikollipara/Desktop/rmit/sem3/Bigdata/Assignment1/Task3mapper3.py jumphost:~/a1/

scp -i s4015344-cosc2637.pem /Users/pallavikollipara/Desktop/rmit/sem3/Bigdata/Assignment1/Task3reducer1.py jumphost:~/a1/

scp -i s4015344-cosc2637.pem /Users/pallavikollipara/Desktop/rmit/sem3/Bigdata/Assignment1/Task3reducer2.py jumphost:~/a1/

scp -i s4015344-cosc2637.pem /Users/pallavikollipara/Desktop/rmit/sem3/Bigdata/Assignment1/Task3reducer3.py jumphost:~/a1/

scp -i s4015344-cosc2637.pem /Users/pallavikollipara/Desktop/rmit/sem3/Bigdata/Assignment1/Task3-run.sh jumphost:~/a1/

Copy to master node:

scp -i ~/s4015344-cosc2637.pem Task3-run.sh hadoop@s4015344.emr.cosc2637.route53.aws.rmit.edu.au:~/

scp -i ~/s4015344-cosc2637.pem Task3reducer1.py hadoop@s4015344.emr.cosc2637.route53.aws.rmit.edu.au:~/

scp -i ~/s4015344-cosc2637.pem Task3reducer2.py hadoop@s4015344.emr.cosc2637.route53.aws.rmit.edu.au:~/

scp -i ~/s4015344-cosc2637.pem Task3reducer3.py hadoop@s4015344.emr.cosc2637.route53.aws.rmit.edu.au:~/

scp -i ~/s4015344-cosc2637.pem Task3mapper1.py hadoop@s4015344.emr.cosc2637.route53.aws.rmit.edu.au:~/

scp -i ~/s4015344-cosc2637.pem Task3mapper2.py hadoop@s4015344.emr.cosc2637.route53.aws.rmit.edu.au:~/

scp -i ~/s4015344-cosc2637.pem Task3mapper3.py hadoop@s4015344.emr.cosc2637.route53.aws.rmit.edu.au:~/


Give execute permission for shell file. Use the command below.
chmod +x Task3-run.sh

And run the file 
./Task3-run.sh

All the outputs will be saved in hdfs Output folder as mentioned in requirements.