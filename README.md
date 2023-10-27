Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu
AIM
To implement Pseudo Node configuration for Hadoop on ubuntu

Pre-requisites
a) jdk

Single-Node Configuration
Create a dedicated user account for hadoop
image

Install java1.8 in folder /usr/local
image

Install Hadoop
image

Set the hadoop environment variables: Include the following lines in the $HOME/.bashrc file
image

Set hadoop environment variables: Include the following lines /etc/profile file
image

Run the.bashrc & profile files from the $ prompt for updating the changes
image

image

Configuration of the hadoop files: hadoop-env.sh, core-site.xml, mapred-site.xml, hdfs- site.xml and yarn-site.xml
path :: /usr/local/hadoop-2.5.1/etc/hadoop

a) hadoop-env.sh Include the following lines in hadoop-env.sh file

image

b) core-site.xml Configure the directory for Hadoop to store its data files, the network ports it listens to, etc. Setup will use Hadoop’s Distributed File System (HDFS-single local machine)

image

Include the following lines in core-site.xml file between and tags

image

c) mapred-site.xml

image

Include the following lines in mapred-site.xml file

image

d) hdfs-site.xml Include the following lines in hdfs-site.xml file

image

e) yarn-site.xml Include the following lines in yarn-site.xml file

image

Format the Hadoop File system implemented on top of the local file system using
image

Start Hadoop using
image

Explore Hadoop using http://localhost:50070/ from the browser

The commonly used HDFS Commands are as follows:
image

Create a directory ‘/input’ in HDFS
image

Copy the input files into the distributed file system
image

Run some of the examples provided
image

Examine the output files
image

Copy the output files from the distributed file system to the local file system and examine them:

image

or

View the output files on the distributed file system

image

Result:
Thus, the implementation of Pseudo Node configuration for Hadoop on ubuntu is successfully executed.
