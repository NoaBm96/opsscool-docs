# Building your python coding environment 

This is a short tutorial on how to build you python programming environement for OpsSchool coding sessoins and home assignmnets. 

### Phase 1 - Create an EC2 instance
- Create your python EC2 instance using this AMI **_opsschool-oct-2020-base-ubuntu_** (AMI ID: *ami-011025cab7de3bd7e*)
- Make sure you:
  - Open port 22 for ssh access
  - Download the SSH key and save it in your opsschool projects directory on your computer
  - Save you server public DNS/IP address

### Phase 2 - Install Visual Studio Code 
- Download VSC [here](https://code.visualstudio.com/Download)
- Install it on your computer

### Phase 3 - Install and configure remote ssh extentio
- Download/Install remote ssh extention from [here](vscode:extension/ms-vscode-remote.remote-ssh)
- It should loook like this: 
  ![](https://code.visualstudio.com/assets/docs/remote/ssh-tutorial/remote-ssh-extension.png "remote-ssh-extension")
- With the Remote - SSH extension installed, you will see a new Status bar item at the far left:  
![](https://code.visualstudio.com/assets/docs/remote/ssh-tutorial/remote-status-bar.png "remote-status-bar")
- The Remote Status bar item can quickly show you in which context VS Code is running (local or remote) and clicking on the item will bring up the Remote - SSH commands.
  ![](https://code.visualstudio.com/assets/docs/remote/ssh-tutorial/remote-ssh-commands.png "remote-ssh-commands")
- Select the remote status bar -> Remote-SSH: Connect to Host... -> Configure SSH Hosts -> Select you ssh config file
- Edit the ssh config file and set your host alias, host address, user name, and ssh key path like this:
```
Host opsschool
  HostName 123.123.123.123
  IdentityFile /home/mickey/private_keys/opssschool.pem
  User ubuntu
```
- Select the remote status bar -> Remote-SSH: Connect to Host... -> Your host name
- VSC should open on your remote host and you should be good to go! 

### Refrences
- Using and configuring Remote SSH for VSC [here](https://code.visualstudio.com/docs/remote/ssh-tutorial)
- How to SSH to AWS servers using an SSH config file? [here](https://codingfundas.com/ssh-to-aws-servers-using-an-ssh-config-file/index.html)
 
