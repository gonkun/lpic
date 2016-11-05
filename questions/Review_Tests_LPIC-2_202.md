202
----------------------------------------------------------------------------------------------------------------------------
Considering the following excerpt from the httpd.conf file, select the correct answer below:
<Location> 
    AllowOverride
    AuthConfig
    Indexes
</Location>

**The excerpt is incorrect, because AllowOverride cannot be used inside a Location 
section**

Which of the following lines in the Apache configuration file would allow only clients with a
valid certificate to access the website?

**SSLVerifyClient require**



Using vsftpd (and some other ftp servers) what is the option in the configuration file to allow anonymous ftp? Include the parameter and value.
**anonymous_enable=yes** (without whitespaces)


Fill in the blank with the options that would be used with the host command to view the mail entries for penguintutor.com.
**host -t MX penguintutor.com**


What format is used for the sendmail /etc/aliases file? Select the most appropriate answer.
**alias: user**


Which of the following programs is required for a computer to act as a DHCP client?
**dhclient**


When configuring DNS what option can be configured on the master server, so that the slave servers are informed when an update is made to a zone file?
**notify**


Which of the following are tools able to query an LDAP database. Select 3 answers.
**ldapsearch**
**slapcat**
**slurpd**


What is the name of the file used to hold the DHCP lease on a DHCP Server? Enter the filename, without any path.
**dhcp.leases**


Which of the following daemons is not normally involved in NFS?
**rpc.tcpd**


What is the name of the daemon used to interface tcp/ip connections to the appropriate RPC calls? Just provide the named of the daemon, no options or path information.
**portmap** or **portmapper**


Which of the following is a command to see what clients have mounted partitions off the local server using nfs?
**showmount**


Which of the following is not one of the PAM module-types.
**login**


In the DNS configuration file, what does the channel option do?
**define where logs go**


Enter a line for the squid.conf file which would create an access control list called "internal" for the IP network range 192.168.1.0 with a network mask of 255.255.255.0. This is to be used as a source address range.
**acl internal src 192.168.1.0/24**


Enter a line for the squid.cfg file which would all access for the access control list "internal"
**http_access allow internal**


What port is normally used by POP3 (PostOffice Protocol Version 3)?
**110**


What command is used to reload the /etc/inittab file after it has been updated? Choose the most appropriate answer:
**/sbin/init q**


Write an entry for dhcpd.conf to give the dns server 192.168.1.2 and 192.168.3.3.
**option domain-name-servers 192.168.1.2,192.168.3.3;**


ll in the blank with the options that would be used with the dig command to view the DNS servers (and their addresses) for penguintutor.com. The command should query specifically the DNS servers, not display all / transfer all entries.
**dig -t NS penguintutor.com** or **dig NS penguintutor.com**


What is the name of the file used to configure the openssh server?
**/etc/ssh/sshd_config**


By default what tcp port is used by the squid proxy server?
**3128**


When configuring a DHCP server what is the option used to ensure a certain machine is always given the same address?
**fixed-address**


What is the name of the command normally used to control the Apache web server and can also query the status?
Enter the command name only.
This is normally, but not always available.
**apachectl** or **apache2ctl**


What protocol(s) are supported by TCP wrappers?
**tcp and udp**


Enter a single line entry for a dns zone that will allow the server 1.2.3.4 to transfer that zone. The rest of the zone file is:

zone mydomain.com {
  type master;
  file "primary/mydomain.com";
  
};

**allow-transfer {1.2.3.4;};**



