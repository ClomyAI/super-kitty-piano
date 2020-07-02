# Simple Kitty Piano Website

This is a simple piano web app made by our super kitty at Clooudemy. 

We often demo this website as class material in Cloudemy online classes, and occasionally play it in the parties.

For grandmasters like you, this is your new world-class instrument. 

You can play [Super Kitty Piano](http://superkittypiano.com)  at superkittypiano.com


![Super Kitty](/images/super-kitty.gif)


#### Super Kitty Piano - Copyright 2020 Cloudemy.tv



### Note:

The sound of kitty piano is generated using Web Audio API.

Go to: https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API for more details.

The Kitty Piano works on most recent browsers (not IE). We recommend you to play it on Firefox or Chrome.



## Option 1: Deploy to AWS EC2 using user data.

Copy & paste the Shell Script below onto the EC2 User Data, when you launch an EC2 instance:

    #!/bin/bash
    yum update -y
    yum install git -y
    yum install httpd -y
    systemctl start httpd
    systemctl enable httpd
    git clone https://github.com/CloudemyTV/super-kitty-piano.git /var/www/html/
    
