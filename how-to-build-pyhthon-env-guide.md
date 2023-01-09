# Building your python coding environment 

At OpsSchool, we use an AWS remote IDE environment called Cloud9 for our home and class assignments. We do this to avoid the different compatability problems and frustrations when working with the local OS env of each student.

In order to setup Cloud9 you must follow the instructions in this blog:
https://aws.amazon.com/blogs/architecture/field-notes-use-aws-cloud9-to-power-your-visual-studio-code-ide

## We also summarized the instructions here for your convenience

### *Important notes*

⚠️ You should be aware that these remote environment take compute(EC2 instance) and disk (gp2 volume) resources which you will be charged on their usage. Try to utilize the [aws free tier](https://aws.amazon.com/free) as much as possible and take these charges into consideration
⚠️ For setting up the Cloud9 environment, we recommend **skipping the automated cloudfromation** offered in the blog and instead just create it manually.

### First Step - Configure Cloud9 env in your personal account
1. Sign in to your AWS account
2. Search for **Cloud9** service in the search bar
    ![image](https://user-images.githubusercontent.com/3054733/211280315-13ba1990-3073-4106-8d43-b77de1cdf86e.png)
3. Click "Create environment"
4. In the create environment screen fill in the required details: \
    **Name:** Give it a meaningful name something like: "opsschool9-dev-env" \
    **Environment type:** Keep the default to "New EC2 instance" \
    **Instance type:** Select the instance type you wish to use. Remember that smaller instances cost less but can also be slow and mis perform. \
    **Platform:** Keep the default pick of "Amazon Linux 2" \
    **Timeout:** We recommend a minimum timeout of 1 hour to be picked 
5. Click "Create" to create the environment

### Step 2 - Install Visual Studio Code 
- Download VSC [here](https://code.visualstudio.com/Download)
- Install it on your computer

### Follow rest of the steps in AWS Blog link
https://aws.amazon.com/blogs/architecture/field-notes-use-aws-cloud9-to-power-your-visual-studio-code-ide

Steps will be:
- Installing and configuring Remote – SSH Extension
- Installing the Session Manager plugin for the AWS CLI
- Creating an SSH key pair to use with remote IDE instance
- Add a shutdown script that will save you money when the IDE is closed and not in use
- Connect and test your connection

### Refrences
- Using and configuring Remote SSH for VSC [here](https://code.visualstudio.com/docs/remote/ssh-tutorial)
- How to SSH to AWS servers using an SSH config file? [here](https://codingfundas.com/ssh-to-aws-servers-using-an-ssh-config-file/index.html)
 
