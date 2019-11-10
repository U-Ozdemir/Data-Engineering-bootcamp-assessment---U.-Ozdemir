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



