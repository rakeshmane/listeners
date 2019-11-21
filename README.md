
List of one liners to run standard services (HTTP, FTP, SMTP, etc)



 
# SMTP Server

#### sudo python -m smtpd -n -c DebuggingServer 192.168.0.2:25

# SMTP Client
#### swaks --to user@example.com --server 192.168.0.2:25


# HTTP Server

#### sudo python -m SimpleHTTPServer 80


# FTP Server

#### sudo python -m pyftpdlib -p 21 -V -D -w

> ` -i ADDRESS, --interface=ADDRESS
     specify the interface to run on (default all interfaces)`
     
> `-p PORT, --port=PORT
     specify port number to run on (default 2121)`

> ` -w, --write
     grants write access for logged in user (default read-only)`

 > `-d FOLDER, --directory=FOLDER
     specify the directory to share (default current directory)`

 >` -n ADDRESS, --nat-address=ADDRESS
     the NAT address to use for passive connections`

> ` -r FROM-TO, --range=FROM-TO
     the range of TCP ports to use for passive connections (e.g. -r 8000-9000)`

 >` -D, --debug
     enable DEBUG logging evel`

>  `-v, --version
     print pyftpdlib version and exit`

 >` -V, --verbose
     activate a more verbose logging`

 >` -u USERNAME, --username=USERNAME
     specify username to login with (anonymous login will be disabled and password required if supplied)`

 >` -P PASSWORD, --password=PASSWORD
     specify a password to login with (username required to be useful)`
     
     
   
