What is the purpose of this project? 
Is to list the users who are all having access to my github repository
For this, I was using shell scripting and github repositories.
Steps to create the shell scripting:
What is the purpose of this project? 
* Create an EC2 instance im AWS, and my instance name is script_project.
*Once the instance is launched and by using its public IP, I connected this public IP to the moboxterm by shh login.
*After logging in to the server, I was using this command to update my instances: "sudo apt update."
*And then I checked whether the git is installed or not using git --version.
*Next, clone my git repository using "git clone https://github.com/Varshid3443/Shell_scripting_Projects."
*Then check if our own git repository is available on the server and then give the right executable permission to the file list_users.sh.
*Next step you need to export our username and token. The username is our git name, and the token we need to generate in our old github repository.
*cammonds "export usernsme="username_git" "export token="git_token"
*And then execute the script file./list_users.sh organization_name repositry_name."
*Finally, you will get the users who are all having access to the git repository.
