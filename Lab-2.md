# Lab on AWS Inspector

We need to perform a network accessibility check on our production EC2 instance and identify any vulnerabilities using Amazon Inspector. To test the security, we will intentionally open port 21 on our EC2 instance. However, please note that port 21 is typically associated with FTP and is not recommended to be kept open on production instances.

## Steps

1. Launch an Amazon Linux EC2 instance with inbound port 21 open. This will be the target EC2 instance for assessment. 

   > **Note:** We are intentionally keeping port 21 open to create a security threat.

2. Add a tag to your target EC2 instance:
   - Key: `Env`
   - Value: `Prod`

3. Define an Assessment Target:
   - Select your EC2 instance as the assessment target.
   - Check "Install Agent on EC2".

4. Define an Assessment Template:
   - Provide a name.
   - Select rule packages.
   - Set the duration to 15 minutes.
   - Uncheck the box for recurring Assessment Schedule.

5. Review and create the template.

6. The assessment run will initiate automatically.

7. Review findings and recommendations.

Use this lab to identify vulnerabilities on your EC2 instance and take appropriate measures to secure it.
