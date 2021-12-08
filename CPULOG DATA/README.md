PERFORMING HQL QUERIES ON  CPULOGDATA(storing to hive from hdfs)  USING PYHIVE and performing visualization :

PYTHON VERSION :(python3 --version) : 3.8.10

     HIVE VERSION :(hive --version) : 3.1.2

     HADOOP VERSION ::(hadoop version):3.3.1


INSTALL  FOLLOWING LIBRARIES along with pyhive:

	i)Install Thrift

	pip3 install thrift
	
	ii) Install thrift sasl

	pip3 install thrift_sasl
	
	iii)Installing Pyhive

	pip3 install pyhive

Fixing  sasl error – fatal error: sasl/sasl.h while installing 

If you are configuring it for the first time, then it is likely that you may get a sasl.h error when installing the sasl module. 
	
	iv)Install libsasl2-dev module to get rid of errors.
	
	sudo apt-get install libsasl2-dev

	v)Install SASL

	pip3 install sasl

Start all Hadoop servers,start hiveserver2

	$Start-all.sh

	$jps

	~$ hiveserver2

In another terminal start beeline and give username,password:
	
	~$ beeline

	beeline> !connect jdbc:hive2://localhost:10000

	Enter username for jdbc:hive2://localhost:10000: P-Rashmi

	Enter password for jdbc:hive2://localhost:10000: *********

	Execute the vs code python program will see the execution on terminal

And queries shows on hiveserver2 UI 

