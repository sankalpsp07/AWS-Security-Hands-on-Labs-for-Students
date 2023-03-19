<h1>Lab on AWS Inspector</h1>
  
We have a production ec2 instance that needs a network accessibility check. we will use amazon inspector to assess, analyze, and identify vulnerabilities.
To test security, we will open port 21 on our ec2 instance. port 21 is typically associated with ftp and is not recommended to keep open on production instances.
  
Steps -

1) Launch an Amazon Linux EC2 instance with inbound port 21 open. This will be our target EC2 instance for assessment 
   Note-Port 21, we are keeping it open intentionally to create a security threat. 

2) Add a tag to your target EC2 instance

3) Key-Environment

4) Value Production

5) Define an Assessment Target

6) Select your EC2 instance as the assessment target

7) Check Install Agent on EC2

8) Define an Assessment Template

9) Provide a name

10) Select Rule Packages

11) Set duration to 15 minutes

12) Uncheck the box for recurring Assessment Schedule

13) Review and create the template

14) Assessment Run will initiate automatically

15) Review Findings and recommendations
