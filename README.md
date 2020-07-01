# Simple Kitty Piano Website

This website is a simple piano made by our super kitty at Clooudemy. 
We often demo this website as class material in Cloudemy online classes, and occasionally play it in the parties.
For grandmasters like you, this is your new world-class instrument. 

## Option 1: Use the following command to deploy the website, if you're using AWS EC2 user data.
Copy & paste the following onto the User Data, when you launch an EC2 instance:

    #!/bin/bash
    yum update -y
    yum install -y httpd
    systemctl start httpd
    systemctl enable httpd
    git clone https://github.com/CloudemyTV/simple-web-kitty-piano.git /var/www/html/
    
