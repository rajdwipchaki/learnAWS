# Stack Features
- [Step 1: Create Stack](#createstack)
- [Step 2: Update Stack](#updatestack)
- [Step 3: Create Change Sets](#createchange)
- [Step 4: Rollback](#rollback)

## <a name="createstack">Step 1: Create Stack</a>
1. Choose 'Create Stack' in Cloud formation.
2. Choose 'Template is ready' and upload a template file. [Here is a sample file to create an EC2 instance in Ohio region](../CloudFormation/Resources/stack1.yaml)
3. Click on 'Next' to see if there is validation error.
4. Enter a name for your stack.
5. Leave other options as it is and click on the 'Create Stack' button.
6. EC2 instance is provisioned and it can be found in the EC2 dashboard (region = ohio)

## <a name="updatestack">Step 2: Update Stack</a>
1. Add a new propoerty 'KeyName' in the previous template.
2. Choose the update stack option and replace the current template. 
3. Specify the template. [Use this template to add a KeyName](../CloudFormation/Resources/stack1-Add-KeyName.yaml)
4. Click on the next button.
5. The change details will be shown under 'Change set preview' section.
6. Go ahead and click on the 'Update Stack' option.

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




