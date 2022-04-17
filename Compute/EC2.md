# EC2
https://github.com/rajdwipchaki/learnAWS/blob/5fbf70f631fb18db7444b8b34c88d7b834aef53e/Compute/ec2/images/ec2-one-pager.jpg
- [Step 1: Launch an instance](#launchec2)
- [Step 2: Connect to your instance](#connectec2)
- [Step 3: Clean up your instance](#cleanec2)

## <a name="launchec2">Step 1: Launch an instance</a>
1. Choose 'Launch Instance' from EC2 dashboard
2. Give a name (e.g., Test) to your virtual machine
3. Select the appropriate AMI (An AMI is a template that contains the software configuration (operating system, application server, and applications) required to launch your instance. Search or Browse for AMIs if you don’t see what you are looking for). Select an HVM version of Amazon Linux 2. Notice that these AMIs are marked "Free tier eligible."
4. Select an instance type that meets your computing, memory, networking, or storage needs. Select the t2.micro instance type, which is selected by default. The t2.micro instance type is eligible for the free tier. In Regions where t2.micro is unavailable, you can use a t3.micro instance under the free tier. 
5. Next a create a key-pair to securely connect to your instance. If you already have a key-pair, select it from the drop down. **Don't select Proceed without a key pair. If you launch your instance without a key pair, then you can't connect to it.**
6. Choose Launch Instance to let the wizard complete the other configuration settings for you.
7. Once the instance is successfully launched, it can be found under the instances section.
8. Select the instance, and click in the Connect option.

## <a name="connectec2">Step 2: Connect to your instance</a>
1. Choose EC2 Instance Connect.
2. Verify the user name and choose Connect to open a terminal window.
3. Run curl command to verify the instance type (curl http://169.254.169.254/latest/meta-data/instance-type)
4. Close the browser window to disconnect.

## <a name="cleanec2">Step 3: Clean up your instance</a>
Once you are done with Step 1 & 2, you can terminate the instance.
1. Select the instance under Instances section in the navigation pane.
2. Choose Instance state, Terminate instance.
3. Choose Terminate when prompted for confirmation.

