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
{Scirpt expalnation}
Line 1 -------- i am using the git api url
Line 2 --------Here i am getting an input of my github_username and token of my git by using "export" cammond
Line 3 --------In this line i am grtting my organization name and repositories [Which acess i need to check]this one i am getting like an argument
Line 4 --------I am creating an two function here one function is to get the api and another function is to list the users here i am using curl cammond to get the api [curl -s -u ${USERNAME}:${TOKEN}" "$url" ]
Line 5 --------local url = "${API_URL}/${endpoint}"
Line 6 --------local endpoint = reposiry_name
Line 7 --------In the next function i was just listing the user name collaborators="$(github_api_get "$endpoint" "
Loine 8--------local endpoint = "repos/${REPO_OWNER}/${REPO_NAME}/collaborators"
Line 10 -------Next i was creating the if and else condion here i am using if [[-z "$collaborators" ]]then,if the no other string ist there it will print no user
Line 11 --------If some string is present it will print the users who are having acess.



