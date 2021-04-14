# openssh-8.5p1 RPM Upgrade

## Upgrade steps
- Download the RPM files and run the following command to upgrade on both CentOS7 and CentOS8
   
      sudo rpm -Uvh openssh-8.5p1*.rpm openssh-clients-8.5p1*.rpm openssh-server-8.5p1*.rpm
      
 - Restart and enable sshd service 
 
       sudo systemctl restart sshd
       sudo systemctl enable sshd

- You can validate by running following Command 
            
      ssh -V
      
      OpenSSH_8.5p1, OpenSSL 1.1.1g FIPS  21 Apr 2020
