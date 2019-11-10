# Data-Engineering-bootcamp-assessment - U.Ozdemir


## HDP Sandbox

1. First I checked the requirements for the HDP Sandbox (10gb RAM needed for virtual box) and assumed that my computer (6gb RAM) would not match this. 

So I tried to make use of the free cloud services from Microsoft Azure and Google Cloud Platform, but because I don't have a creditcard, I could not make use of the cloud services for both.

2. I downloaded the HDP_3.0.1_vmware_181205, which had a size of 20,5gb and took 5 hours to download. To reduce this time I used the internet cable and the download process went to 2 hours. 

3. I downloaded the VMware-player-15.5.0-14665864, which is needed to setup the HDP Sandbox. 

4. Open virtual machine (HDP) and here I changed the settings of the virtualbox to 4gb RAM because my computer would not be able to handle more. The import, extraction and loading took very long. My computer went very slow and also I could not connect to my browser with the given of the Sandbox. 

I changed the settings of the virtualbox to 1gb because my computer almost froze. I still could not connect to my browser, so I searched what the problems could be. 

I checked my firewall and the Vmware Network Adapter, both are not causing any problem. The problem was fixed by opening a new browser and disabling AdBlock. 

After connecting to the browser I selected the HDP and logged in Ambari with maria_dev, because this one had the tools I needed to use later on. Another problem here was that Ambari was loading very slow, I could not reach the dashboard screen. This is probebly because 1gb reduces the performance drasticly.

So again I changed the setting to 2.5gb and repeated everything, and now the Ambari screen loaded faster. The problem here was that the services were loading very slow.


## HDFS & Hive on Spark

1. I downloaded sbt which was needed to build a scala application and java (OpenJDK8U-jdk_x64_windows_hotspot_8u232b09).

2. After this I got pretty much stuck because the Ambari servers would not load fast or had some errors.


## Other approaches

Because Ambari was very slow I've tried to setup Hadoop and Spark first manually.  

1. Following a tutorial, I downloaded spark-2.3.2-bin-hadoop2.7, hadoop-3.1.1.tar, and jdk-8u231-windows-x64. I installed Java first and changed the directory to C:\Java, because there could be trouble with directories with spaces in their names. This is also done for Hadoop and Spark.

2. I had to setup environment variables in control panel > System > Advanced System Settings > Environment Variables. I created system variables for Java, Hadoop and Spark by naming them and adding a directory path in which they are located. After that I need to add these into the PATH variable with \bin at the end of their respective paths.

3. I checked in cmd by using echo %PATH% if these directories were added in the PATH variable, which was not the case. I tried the process of step 2 again but this time I created the variables in user variables and also this did not work.

I am not sure what was wrong, but I did notice that one tutorial creates them in 'system' and the other in 'user'. Also these tutorials were made for windows 10 (mine is windows 7), which might explain why it did not work on m computer.




