Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu
AIM
To implement Pseudo Node configuration for Hadoop on ubuntu

Pre-requisites
a) jdk

Single-Node Configuration
Create a dedicated user account for hadoop
Screenshot (246)

Install java1.8 in folder /usr/local
Screenshot (247)

Install Hadoop
Screenshot (248)

Set the hadoop environment variables: Include the following lines in the $HOME/.bashrc file
Screenshot (249)

Set hadoop environment variables: Include the following lines /etc/profile file
Screenshot (250)

Run the.bashrc & profile files from the $ prompt for updating the changes
Screenshot (251)

Screenshot (252)

Configuration of the hadoop files: hadoop-env.sh, core-site.xml, mapred-site.xml, hdfs- site.xml and yarn-site.xml
path :: /usr/local/hadoop-2.5.1/etc/hadoop

a) hadoop-env.sh Include the following lines in hadoop-env.sh file

Screenshot (253)

b) core-site.xml Configure the directory for Hadoop to store its data files, the network ports it listens to, etc. Setup will use Hadoop’s Distributed File System (HDFS-single local machine)

Screenshot (254)

Include the following lines in core-site.xml file between and tags

Screenshot (255)

c) mapred-site.xml

Screenshot (256)

Include the following lines in mapred-site.xml file

Screenshot (257)

d) hdfs-site.xml Include the following lines in hdfs-site.xml file

Screenshot (258)

e) yarn-site.xml Include the following lines in yarn-site.xml file

Screenshot (259)

Format the Hadoop File system implemented on top of the local file system using
Screenshot (260)

Start Hadoop using
Screenshot (261)

Explore Hadoop using http://localhost:50070/ from the browser

The commonly used HDFS Commands are as follows:
Screenshot (262)

Create a directory ‘/input’ in HDFS
Screenshot (263)

Copy the input files into the distributed file system
Screenshot (264)

Run some of the examples provided
Screenshot (265)

Examine the output files
Screenshot (266)

Copy the output files from the distributed file system to the local file system and examine them:

Screenshot (267)

or

View the output files on the distributed file system

Screenshot (268)

Result:
Thus, the implementation of Pseudo Node configuration for Hadoop on ubuntu is successfully executed.
