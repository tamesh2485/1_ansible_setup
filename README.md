############################################################################
		Set up git on the working Directory
############################################################################
# cd /home/tamesh/ANSIBLE
# git init 
# git config user.email "tameshchakraborty2@gmail.com"
# git config user.name "Tamesh
# git config --list
############################################################################
		Connect to the remote Repo
############################################################################
# git remote add origin https://github.com/tamesh2485/1_ansible_setup.git
# git remote -v 
origin	https://github.com/tamesh2485/1_ansible_setup.git (fetch)
origin	https://github.com/tamesh2485/1_ansible_setup.git (push)

# git pull origin master
# ls 
README.md
############################################################################
		ANSIBLE COMMAND MODULE
############################################################################
[tamesh@ansibleserver ANSIBLE]$  ansible all  -m shell -a "id"
centos | CHANGED | rc=0 >>
uid=0(root) gid=0(root) groups=0(root) context=unconfined_u:unconfined_r:unconfined_t:s0-s0:c0.c1023
client2 | CHANGED | rc=0 >>
uid=0(root) gid=0(root) groups=0(root) context=unconfined_u:unconfined_r:unconfined_t:s0-s0:c0.c1023
[tamesh@ansibleserver ANSIBLE]$  ansible all  -m shell -a "uptime"
centos | CHANGED | rc=0 >>
 15:11:29 up  2:40,  3 users,  load average: 0.07, 0.02, 0.04
client2 | CHANGED | rc=0 >>
 15:11:29 up  2:40,  4 users,  load average: 0.27, 0.10, 0.15

############################################################################
		Install posix Collection for firewalld,mount module
############################################################################
# ansible-galaxy collection install ansible.posix
# ansible-doc firewalld ; ansible-doc mount 
############################################################################

############################################################################

############################################################################

############################################################################
