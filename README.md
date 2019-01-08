# Apache-SSL-Configuration
Apache 2.4.6 SSL Configuration

Usage

First install apache:

    Step 1
      yum clean all

    Step 2
      yum –y update

    Step 3
      yum –y install httpd

    Step 4
      firewall-cmd --permanent –add-port=80/tcp

    Step 5
      firewall-cmd –permanent –add-port=443/tcp

    Step 6
      firewall-cmd –reload

    Step 7
      systemctl start httpd

    Step 8
      systemctl enable httpd

    Step 9
      yum –y update

Now we config ssl:

    Step 10
      Download and copy ssl.conf file to /etc/httpd/conf.d

    Step 11
      Copy your Certificate file in /etc/pki/tls/certs

    Step 12
      Copy your Private key file in /etc/pki/tls/private  

    Step 13
      Copy your CA file in the /etc/pki/tls/certs

    Step 14
      Change this line in the httpd.conf

          ServerName localhost:80

    Step 15
      Systemctl restart httpd 
 
  

  
  
