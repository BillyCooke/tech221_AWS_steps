# Creating an EC2 instance on AWS steps

1. Log into AWS and select the region you would like to use
2. In the search bar type in EC2
3. Select Instances in the resources section
4. In the top right click Launch instance
5. Name your instance
6. Scroll down a little and select browse AMI's
7. Choose the AMI that you need
8. Then in Instance type select the size of the instance
9. Next you need to add the key pair (we had already made one on Git called tech221)
10. In network settings we need to select what we allow SSH traffic from and it can never be left on anywhere. Use the drop down to select My IP
11. Underneath that also select allow HTTP traffic from the internet
12. Next select how many instances you want to launch in the summary section (we left it as one)
13. Then select launch
14. Select the instances page on the left side of the screen and click onto your instance
15. Wait until the status checks have been completed and your instance is running
16. Click the connect box at the top of the page and head to SSH client
17. This will provide you a command to run in Git Bash
18. Open up Git Bash and head to the .ssh directory using ```cd .ssh```
19. Enter the first command given to you to ensure your key is not publicly viewable. For example mine is ```chmod 400 tech221.pem```
20. Then enter the second code into Git Bash. For example mine is ```ec2-3-250-178-47.eu-west-1.compute.amazonaws.com```
21. If you are doing this for the first time you may be prompted to select an option, please select yes. This should not happen in the future.
