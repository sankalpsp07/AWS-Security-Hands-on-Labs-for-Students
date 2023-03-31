# Lab Exercise I


You can launch a Linux instance using the AWS Management Console as described in the following procedure. This tutorial is intended to help you quickly launch your first instance, so it doesn't cover all possible options. For information about advanced options, see [Launch an instance using the new launch instance wizard](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/launching-instance.html). For information about other ways to launch your instance, see [Launch your instance](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EC2_GetStarted.html).

### To launch an instance

1. Open the [Amazon EC2 console](https://console.aws.amazon.com/ec2/)

2. From the EC2 console dashboard, in the Launch instance box, choose Launch instance, and then choose Launch instance from the options that appear.

3. Under Name and tags, for Name, enter a descriptive name for your instance.

4. Under Application and OS Images (Amazon Machine Image), do the following: choose Amazon Linux. This is the operating system (OS) for your instance.

5. From Amazon Machine Image (AMI), select an HVM version of Amazon Linux 2. Notice that these AMIs are marked Free tier eligible. An Amazon Machine Image (AMI) is a basic configuration that serves as a template for your instance.

6. Under Instance type, from the Instance type list, you can select the hardware configuration for your instance. Choose the t2.micro instance type, which is selected by default. The t2.micro instance type is eligible for the free tier. In Regions where t2.micro is unavailable, you can use a t3.micro instance under the free tier. For more information, see [AWS Free Tier](https://aws.amazon.com/free/).

7. Under Key pair (login), for Key pair name, choose the key pair that you created when getting set up.

8. Next to Network settings, choose Edit. For Security group name, you'll see that the wizard created and selected a security group for you. You can use this security group, or alternatively you can select the security group that you created when getting set up using the following steps:

9. Choose Select existing security group.

10. From Common security groups, choose your security group from the list of existing security groups.

11. Keep the default selections for the other configuration settings for your instance.

12. Review a summary of your instance configuration in the Summary panel, and when you're ready, choose Launch instance.

13. A confirmation page lets you know that your instance is launching. Choose View all instances to close the confirmation page and return to the console.

14. On the Instances screen, you can view the status of the launch. It takes a short time for an instance to launch. When you launch an instance, its initial state is pending. After the instance starts, its state changes to running and it receives a public DNS name. If the Public IPv4 DNS column is hidden, choose the settings icon ( Settings icon. ) in the top-right corner, toggle on Public IPv4 DNS, and choose Confirm.

15. It can take a few minutes for the instance to be ready for you to connect to it. Check that your instance has passed its status checks; you can view this information in the Status check column.
