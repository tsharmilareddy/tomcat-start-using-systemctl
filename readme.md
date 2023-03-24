# Create an ec2 instance
# Install java and  tomcat 
# then open a file in this path /etc/systemd/system/tomcat.service

# In this file copy data , we gave this date in tomcat file
# In the file u have to change java path only for this u have to move /usr/lib/jvm/java-17-amazon-corretto.x86_64


# Then add user and give permissions to that

# then we will move tomcat bin path then will enter below commands

systemctl daemon-reload

systemctl start tomcat.service

systemctl enable tomcat.service
