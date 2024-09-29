What is the purpose of this project is to list the users how are all having acess to my git hub repositry 
For this i was using the shell scrpiting and git hub repositry.
Steps to create the shell scripting:
     * Create an ec2 instances im aws and my instance name is script_project
     *Once the instances is lanuched and by using its public ip i was connected this public ip to the moboxterm by shh login.
     *After login to the server i was using this cammond to update my instances update "sudo apt update"
     *And then i checked whether the git is installed or not using git --version.
     *Next clone my git repositry using "git clone  https://github.com/Varshid3443/Shell_scripting_Projects"
     *Then check the our own git repositry is available in the server and then give the the right executable permission to the file list_users.sh
     *Next step  you need to export our username and token for username is our git name and token we need to generate in our oun git hub repositry.
     *cammonds "export usernsme="username_git"  "export token="git_token"
     *And then execute the script file ./list_users.sh organization_name repositry_name"
     *Finally you will get the users who are all having acess to the git repositry.
     
