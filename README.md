# Simple Kitty Piano Website

This is a simple piano web app made by our super kitty at Clooudemy. 
We often demo this website as class material in Cloudemy online classes, and occasionally play it in the parties.
For grandmasters like you, this is your new world-class instrument. 

### Note:
The sound of kitty piano is generated using Web Audio API.
Go to: https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API for more details.
The Kitty Piano works on most recent browsers (not IE). 

## Deployment Option 1: Use the following command to deploy the website, if you're using AWS EC2 user data.
Copy & paste the following onto the User Data, when you launch an EC2 instance:

    #!/bin/bash
    yum update -y
    yum install -y httpd
    systemctl start httpd
    systemctl enable httpd
    git clone https://github.com/CloudemyTV/simple-web-kitty-piano.git /var/www/html/
    
