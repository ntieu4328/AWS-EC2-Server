<h1>AWS EC2 Server</h1>

<h2>Description</h2>
The project consists of creating an AWS EC2 server instance. You can use the server for cybersecurity, virtual servers, and managing cookies.
<br/>

<h2>Table of contents:</h2>

[What is AWS EC2?](what-is-aws-ec2?)

[Why would you use it?](why-would-you-use-it?)

[Set Up](set-up:)

<h2>What is AWS EC2?</h2>
AWS EC2 is resizable compute capacity in the cloud.
<br/>

<h2>Why would you use it?</h2>

- Easy to set up
- It's all in the cloud so you don't provide the hardware
- You can scale it up or down
- You pay for what you use
- It's very secure because it's provided by Amazon
- You can access it from anywhere

<h2>Set Up:</h2>

1. Go to [AWS sign in page](https://signin.aws.amazon.com/signin?redirect_uri=https%3A%2F%2Fconsole.aws.amazon.com%2Fconsole%2Fhome%3FhashArgs%3D%2523%26isauthcode%3Dtrue%26nc2%3Dh_ct%26src%3Dheader-signin%26state%3DhashArgsFromTB_us-east-2_1e9033bf1efdf7a6&client_id=arn%3Aaws%3Asignin%3A%3A%3Aconsole%2Fcanvas&forceMobileApp=0&code_challenge=zl8TQMFJ3wIvus8czNqQLoM3FI_8pvtMJEYumj0zSQ4&code_challenge_method=SHA-256). Sign in if you already have an account or create an AWS account. When you create a new account it will ask for credit card information.

2. In the search bar look up EC2 and it will bring you to the dashboard.
![ec2 dashboard](https://github.com/ntieu4328/AWS-EC2-Server/assets/156137990/866a43dc-13d6-44bf-812e-d263ae9b0021)

3. Name the server.
   
   ![server name](https://github.com/ntieu4328/AWS-EC2-Server/assets/156137990/4d6f5e97-f810-4177-b2ba-d68b7a805b85)

4. Choose which OS image you want to use. Different OSs have different features.
![choose os image](https://github.com/ntieu4328/AWS-EC2-Server/assets/156137990/c1461e5f-b60c-4460-84c5-22f73110a011)

If you notice in the image above there are certain images that you can run for free. If you click "Browse more AMIs" you can find third-party AMIs.
![more amis](https://github.com/ntieu4328/AWS-EC2-Server/assets/156137990/d23389fa-4266-4050-a745-324f93259351)

5. Choose instance type.

![instance type](https://github.com/ntieu4328/AWS-EC2-Server/assets/156137990/e04b0924-14e2-403e-94d8-d9a6b0667ac7)

If you click on the instance type you can choose other options. The other instance types may have a different number of CPUs and memory. If you look at the picture you can see that it says "free tier eligible". This means that you can use that instance type for free. Instance types that don't say "free tier eligible" will make you pay a certain amount per hour to use it. It will show you how much you have to pay when you select it.

6. Create Key pair for login.
   
![create key pair](https://github.com/ntieu4328/AWS-EC2-Server/assets/156137990/1bdbd001-a645-44bd-949e-55a40b1db12a)

Click "Create new keypair".

![key pair setup](https://github.com/ntieu4328/AWS-EC2-Server/assets/156137990/22f336ef-15e9-4d54-80e0-525253358fea)

Name the Key pair whatever you want. The rest of the settings should be kept the same. After clicking the "Create key pair" it will download the key pair to your downloads folder.

7. Network settings.
   
![network settings](https://github.com/ntieu4328/AWS-EC2-Server/assets/156137990/082ed50f-5ff1-41f0-9f0d-f2f2ffb29cd3)

To make it so you are the only person that can access the server I would change the security group rule from "Anywhere" to "My IP".

![change to my ip](https://github.com/ntieu4328/AWS-EC2-Server/assets/156137990/c6da8895-e572-4691-aeba-5f5e0732d861)

8. Configure storage.
   
![Configure storage](https://github.com/ntieu4328/AWS-EC2-Server/assets/156137990/1c149c79-f208-48cb-9ee0-c249f0f5d406)

<b>You get 30 GiB for free. If you want more storage it will tell you how much you have to pay per hour.</b>

9. Scroll to the bottom and click "Launch instance".
    
![launch instance](https://github.com/ntieu4328/AWS-EC2-Server/assets/156137990/f07d4743-3e57-47be-a22a-3c41e4f07c4d)

10. Wait for the EC2 instance to start running
    
![wait for run](https://github.com/ntieu4328/AWS-EC2-Server/assets/156137990/b0bf1f4b-dd3a-4c77-bd08-c55ecad925b7)

<b>Make sure that the instance state says "Running" and the status check shows "2/2 checks passed"</b>

11. Click on the instance and then connect at the top. (Button circled in yellow)
    
![connect highlited](https://github.com/ntieu4328/AWS-EC2-Server/assets/156137990/1ea2d7fa-acca-4899-969b-5b8e51562eb3)

12. Choose how you would like to connect
  - EC2 Instance Connect

![EC2 instance connect](https://github.com/ntieu4328/AWS-EC2-Server/assets/156137990/d15e3a97-337c-4bb2-b62f-201432d72a9a)

Choosing this way to connect to the EC2 instance brings up a browser-based client.

  - SSH client

![SSH client](https://github.com/ntieu4328/AWS-EC2-Server/assets/156137990/ed0b2014-0601-4637-8d60-7e8cf24998c4)

Copy the command under "Example" and input that into the terminal. Choosing this way allows you to SSH into the server.

<b>You have now created an AWS EC2 server!!!</b>
