make sure your system has ssh connectivity with remote system. If not follow the below commands

it's a good practice to move your key.pem file to the ~/.ssh/ dir
    
    chmod 400 ~/.ssh/Practice-devops.pem

Edit ~/.ssh/config file

    nano ~/.ssh/config

and update like this (for ubuntu)

    Host IP-dns-address
        HostName IP-dns-address
        User Ubuntu
        IdentityFile ~/.ssh/key.pem

save the file and Run below command

    ssh IP-dns-address
OR you can use 

    ssh -i ~/.ssh/key.pem ec2-user@ip-address


        

    
    

   
