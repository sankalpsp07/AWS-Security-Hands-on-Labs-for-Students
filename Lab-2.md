<h1>Lab on AWS Inspector</h1>
  
We have a production ec2 instance that needs a network accessibility check. we will use amazon inspector to assess, analyze, and identify vulnerabilities.
To test security, we will open port 21 on our ec2 instance. port 21 is typically associated with ftp and is not recommended to keep open on production instances.
  
Steps -

1) Launch an Amazon Linux EC2 instance with inbound port 21 open. This will be our target EC2 instance for assessment 
   Note-Port 21, we are keeping it open intentionally to create a security threat. 

2) Add a tag to your target EC2 instance
   Key-Env
   Value- Prod

3) Define an Assessment Target
   -Select your EC2 instance as the assessment target
   -Check Install Agent on EC2

4) Define an Assessment Template
   -Provide a name
   -Select Rule Packages
   -Set duration to 15 minutes
   -Uncheck the box for recurring Assessment Schedule

5) Review and create the template

6) Assessment Run will initiate automatically

7) Review Findings and recommendations


