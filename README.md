###<strong>Ansible playbook to add sftp users. If home folder does not exist, it will create it and chmod as root with 755 permissions</strong> 

***
<strong>Usage:</strong> <br />
ansible-playbook -i inventory sftponly.yml

You can also pass the variables to the command line. Eg: ansible-playbook -i hosts sftponly.yml --extra-vars "sftp_user=$USER real_mount=$FULL_PATH bind_mount=$HOME/sftp_user/$RELATIVE_PATH "

***




####<strong>TO DO</strong> <br />

Better check sshd_config if it's already configured for sftp-only
