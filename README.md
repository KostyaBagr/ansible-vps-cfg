<h1> ANSIBLE SCRIPT FOR CONFIG VPS </h1>


<h2> <b> What it can </b> </h2>
<br>
1) Install necessary packages <br>
2) Install Docker, Docker-Compose, add docker user to sudo <br>
3) Create new user (you can set username in env), add user to sudo group <br>
4) Install oh-my-zsh, make it default for new user <br>
5) Copy ssh keys to remote host <br>
6) Change ssh config: block login by root, change ssh port (you can set it in env), block login by password

<h2> <b> How to start </b> </h2> <br>
- create .env and run <code> export $(grep -v '^#' .env | xargs) </code> <br>
- create authorized_keys file <code> touch authorized_keys </code> <br>
- run <code> ansible-playbook -i inventory.yml playbook.yml </code> <br>

