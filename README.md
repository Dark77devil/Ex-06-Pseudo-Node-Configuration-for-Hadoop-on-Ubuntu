# Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu

## AIM

To implement Pseudo Node configuration for Hadoop on ubuntu

## Pre-requisites

a) jdk

### Single-Node Configuration

1.	Create a dedicated user account for hadoop

![Screenshot (246)](https://github.com/MaheshS03/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/128498431/cb1e7b24-1fed-4834-a05b-11a5aadf45c5)

2.	Install java1.8 in folder /usr/local                                                         

![Screenshot (247)](https://github.com/MaheshS03/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/128498431/649ef0cd-ab55-4fa4-a1d6-bc240a932979)

3.	Install Hadoop

![Screenshot (248)](https://github.com/MaheshS03/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/128498431/ba83c091-b842-4bf8-9d0d-15fd1c9719bf)

4.	Set the hadoop environment variables: Include the following lines in the
$HOME/.bashrc file

 ![Screenshot (249)](https://github.com/MaheshS03/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/128498431/1c4bcc05-06a5-4637-a36e-39268cb5bc8d)

5.	Set hadoop environment variables: Include the following lines /etc/profile file

![Screenshot (250)](https://github.com/MaheshS03/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/128498431/fb4038b0-4c82-4a7d-be76-61e4b9070db3)

6.	Run the.bashrc & profile files from the $ prompt for updating the changes

![Screenshot (251)](https://github.com/MaheshS03/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/128498431/f0dfcea4-7463-4103-800f-ce5fc9cdcbfc)

![Screenshot (252)](https://github.com/MaheshS03/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/128498431/989fd3ae-c684-4dec-8dc5-8739bf454084)


7.	Configuration of the hadoop files: hadoop-env.sh, core-site.xml, mapred-site.xml, hdfs- site.xml and yarn-site.xml

path ::	/usr/local/hadoop-2.5.1/etc/hadoop

a)	hadoop-env.sh
Include the following lines in hadoop-env.sh file

![Screenshot (253)](https://github.com/MaheshS03/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/128498431/5b009301-0739-42ef-983c-c4097a0a7e50)

b)	core-site.xml
Configure the directory for Hadoop to store its data files, the network ports it listens to, etc. Setup will use Hadoop’s Distributed File System (HDFS-single local machine)

![Screenshot (254)](https://github.com/MaheshS03/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/128498431/10183af6-6b6f-47ee-b01a-805609e46467)
 
Include the following lines in core-site.xml file between <configuration> and </configuration> tags

![Screenshot (255)](https://github.com/MaheshS03/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/128498431/e3dcddd3-e487-4f5d-b69b-8744d35c52f1)

c)	mapred-site.xml
 
![Screenshot (256)](https://github.com/MaheshS03/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/128498431/100c5e71-fb4b-4b7d-8989-38bbde9d11cb)

Include the following lines in mapred-site.xml file
 
![Screenshot (257)](https://github.com/MaheshS03/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/128498431/10a96037-fe17-4d44-9e65-48e307ebe870)

d)	hdfs-site.xml
Include the following lines in hdfs-site.xml file

![Screenshot (258)](https://github.com/MaheshS03/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/128498431/068e2e96-7213-4c59-8412-60574b91e7c6)

e)	yarn-site.xml
Include the following lines in yarn-site.xml file

![Screenshot (259)](https://github.com/MaheshS03/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/128498431/3868cc81-4348-4fd7-ab60-b7045f204619)

8.	Format the Hadoop File system implemented on top of the local file system using

![Screenshot (260)](https://github.com/MaheshS03/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/128498431/3f911eb1-ff46-4507-9ca6-7e05228f3a8f)

9.	Start Hadoop using

![Screenshot (261)](https://github.com/MaheshS03/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/128498431/affdd8a1-fe50-4dc7-9642-417eebcca454)

Explore Hadoop using http://localhost:50070/ from the browser	
 
10.	The commonly used HDFS Commands are as follows:

![Screenshot (262)](https://github.com/MaheshS03/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/128498431/7bd11556-0a63-4285-a77a-f64c3a91c077)

11.	Create a directory ‘/input’ in HDFS

![Screenshot (263)](https://github.com/MaheshS03/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/128498431/2ee55402-ca91-495e-b776-4815cbdbff68)

12.	Copy the input files into the distributed file system

![Screenshot (264)](https://github.com/MaheshS03/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/128498431/e24652ce-13a4-44b1-99ac-e2858818a006)

13.	Run some of the examples provided

![Screenshot (265)](https://github.com/MaheshS03/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/128498431/dd915e98-fbd7-4484-97a3-d0501f953c22)

14.	Examine the output files

![Screenshot (266)](https://github.com/MaheshS03/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/128498431/06a6f8b8-59ac-43b2-8655-b801a37cb8f3)

Copy the output files from the distributed file system to the local file system and examine them:

![Screenshot (267)](https://github.com/MaheshS03/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/128498431/ab12e187-6aed-4576-a9fc-e141ea0d9428)

or

View the output files on the distributed file system

![Screenshot (268)](https://github.com/MaheshS03/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/128498431/380ed3ad-49b7-4d03-b58e-af9a85c70058)

## Result:
Thus, the implementation of Pseudo Node configuration for Hadoop on ubuntu is successfully executed.
