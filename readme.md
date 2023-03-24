# Create an ec2 instance
# Install java and  tomcat by using below command
# yum install java -y
# wget https://dlcdn.apache.org/tomcat/tomcat-9/v9.0.73/bin/apache-tomcat-9.0.73.tar.gz



Then open a file 

vi /etc/systemd/system/tomcat.service

In this file copy data 
       
In the file u have to change java path like cd /usr/lib/jvm   then we will 

get path , that java file name we can pass above

Then add useradd tomcat

chown -R tomcat:tomcat /opt/tomcat

Then move to tomcat bin path

systemctl daemon-reload

systemctl start tomcat.service

systemctl enable tomcat.service