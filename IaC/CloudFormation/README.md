# Stack Features
- [Step 1: Create Stack](#createstack)
- [Step 2: Update Stack](#updatestack)
- [Step 3: Create Change Sets](#createchange)
- [Step 4: Rollback](#rollback)

## <a name="createstack">Step 1: Create Stack</a>
1. Choose 'Create Stack' in Cloud formation.
2. Choose 'Template is ready' and upload a template file. [Here is a sample file to create an EC2 instance in Ohio region](../CloudFormation/resources/stack1.yaml)
3. Click on 'Next' to see if there is validation error.
4. Enter a name for your stack.
5. Leave other options as it is and click on the 'Create Stack' button.

## <a name="updatestack">Step 2: Update Stack</a>
1. Choose EC2 Instance Connect.
2. Verify the user name and choose Connect to open a terminal window.
3. Run curl command to verify the instance type (curl http://169.254.169.254/latest/meta-data/instance-type)
4. Close the browser window to disconnect.

## <a name="createchange">Step 3: Create Change Sets</a>
Once you are done with Step 1 & 2, you can terminate the instance.
1. Select the instance under Instances section in the navigation pane.
2. Choose Instance state, Terminate instance.
3. Choose Terminate when prompted for confirmation.

## <a name="rollback">Step 4: Rollback</a>
Once you are done with Step 1 & 2, you can terminate the instance.
1. Select the instance under Instances section in the navigation pane.
2. Choose Instance state, Terminate instance.
3. Choose Terminate when prompted for confirmation.




