This project is just a basic showcase of the folder structure for an ansible project.
This project also illustrates how to differentiate between a debian os and redhat os.Since the packages used to install will be different  


Steps to setup the ec2 ubuntu machines hosted in aws
- setup the machines with key-pairs(DONT SETUP WITHOUT KEY PAIRS)
- copy the contents of your key into your local linux machine which acts as a control.add it into ./ssh/id_rsa
- and do a chmod 600 ./ssh/id_rsa 





Command to run:
- ansible-playbook playbooks/site.yml