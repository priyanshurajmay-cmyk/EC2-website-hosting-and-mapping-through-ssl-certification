# Hosting a website in EC2 AWS, SSL certification can't be initiated due to an unknown error
## Steps for Ec2 server Deployment

Quick Deployment Steps
1. Log in to AWS Console: Go to the AWS Management Console and sign in.
2. Navigate to EC2: Search for and select EC2 from the services list.
3. Launch Instance: Click the Launch Instance button.
4. Choose AMI & Type: Select your desired AMI (e.g., Ubuntu, Amazon Linux) and an Instance Type (e.g., t2.micro).
5. Configure: Leave most settings as default, but ensure Auto-assign Public IP is enabled if needed.
6. Add Storage & Tags: Adjust the storage size and add a Name tag to identify your instance.
7. Configure Security Group: Set up firewall rules to allow traffic on specific ports like SSH (22) and HTTP (80).
8. Review & Launch: Confirm your settings, then click Launch.
9. Select Key Pair: Choose an existing key pair or create a new one to securely connect to your instance.
![](https://github.com/priyanshurajmay-cmyk/EC2-website-hosting-and-mapping-through-ssl-certification/blob/main/images%20ec2/Screenshot%202025-08-30%20164504.png)

## 2. Connect to EC2 (using PuTTY/SSH)
1. Download the Putty.exe file and install.
2. Write the public IP in the session.
3. Go to connection -> ssh -> auth
4. Browse the key pair.
5. Now select Open.
6. Use Ubuntu as a user name

## 3. Install Apache
`sudo apt install apache2`
Use a browser to open `http://instance public ip`
it will show a confirmation page of it.

Now in puTTY `cd /var/www/html
sudo rm index.html
sudo vi index.html`
1. Press I and insert HTML code.
2. Write your code.
3. After writing all code, Press Ctrl+C and then write ":wq" Press Enter.

## 5. Domain Mapping with 53
![](https://github.com/priyanshurajmay-cmyk/EC2-website-hosting-and-mapping-through-ssl-certification/blob/main/images%20ec2/Screenshot%202025-08-30%20164756.png)
## 6. Name Server
![](https://github.com/priyanshurajmay-cmyk/EC2-website-hosting-and-mapping-through-ssl-certification/blob/main/images%20ec2/Screenshot%202025-08-30%20164833.png)
## 7. Domain Name, Name server
![](https://github.com/priyanshurajmay-cmyk/EC2-website-hosting-and-mapping-through-ssl-certification/blob/main/images%20ec2/Screenshot%202025-08-30%20164904.png)
## 8. Website before SSL (Showing Not Secure)
![]()
