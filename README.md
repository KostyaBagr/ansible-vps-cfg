- create .env and run <code> export $(grep -v '^#' .env | xargs) </code>
- create authorized_keys file <code> touch authorized_keys </code>
- start <code> ansible-playbook -i inventory.yaml playbook.yaml </code>

What it can:

install packages
install docker
create new user
add zsh
add oh-my-zsh
block login by root
add ssh keys
change ssh port
block login by password
