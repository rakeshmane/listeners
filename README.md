
List of one liners to run standard services (HTTP, FTP, SMTP, etc)



 
# SMTP Server

#### sudo python -m smtpd -n -c DebuggingServer 192.168.0.2:25

# SMTP Client
#### swaks --to user@example.com --server 192.168.0.2:25


# HTTP Server

#### sudo python -m SimpleHTTPServer 80
    
    
# HTTPS Server

#### python BelowFile.py

```
import BaseHTTPServer, SimpleHTTPServer
import ssl,base64

cert='LS0tLS1CRUdJTiBQUklWQVRFIEtFWS0tLS0tCk1JSUV2QUlCQURBTkJna3Foa2lHOXcwQkFRRUZBQVNDQktZd2dnU2lBZ0VBQW9JQkFRQ2RjYlh4ZFJPNno1N1cKK0lhcHRweTJmQlF0ZzV3ZVNERERaMVZ2ZnFZd1MvMHJYTUxBS2YycXRlVjh0VUdEbE5DcTJrSGRkVHd4YkU2bApOM2cxUHlhT3IvMjlDbnpTNS9hM3dRVWM3VFVuQXhTYUJaVW9xUGd6TFZUZXRNdmN0SjRPUXhiTFRueThMSGMwCmNyLzlHSDhVa3krYnZyQlBWV2lrWlpMS3BBS2lxdjBkdTBKNFFJYVZOQmNIbWZHekhjRTk2Mmg2YnFidlRQTDcKYnB1K25MWEVKQWs2ZVRLVnNnS2Y5U2Vkd3ZXZ0dPRUlMaEhUSzQrekJzOTdsSHJ3dXp0VFdma2I5eXJVMUt4eApFdWE3eCtLRkxwRzNxSnU5d3hyUnlJQldPTCtObzhNRElMMXY3UFVGcFN2amN6bDdnS1VBaXk0SVFMcXgrVHUrCkhHQkF1dVNsQWdNQkFBRUNnZ0VBUlRXOFBrVXlCQmZLZ2tORHB3MFFQS08wbHdGWXVuTVBoSVpESnp6c1B5VFkKU0p5Qk84bjVxWFpHU0JqQmtONzFEM1hjS0VhbHpEQUpMbFdBOFI4dWl1RFFVSzV3aXFIUGNaMVc2dzFYSlN3VQpmVlJnNmp2RXgzSnc4V2xXaUZHWmZUbCtwcVo4N0pjN1c0SHA1WTlFSmI1QjJsdnIweVAvV08wUnB5U0x5QWRqCnRQM1R5WExudEoyUHB4bTVxOW5YQnRqSDVDNTBmM2pNTEVMU1hmeDJqanNzdHFXTkFkUk13eEtzRmt0VXpNNmUKNW5RWEk5YS9oWHZSWU82eDdDRmpVNUFKK3pUY3ZnT2JwbCtPMVMvbTBDTHpzU3BuOEVWclFYUW1OT1ZuNFU5QQpBVE05NHB3ODVwenBzbE1IcTNSWFE1Sml5VVdGMHdqMDgxeDJ1MDhtb1FLQmdRREppTGErSUxka0Rjd3QzamVZCmxTN2ZlUGczVlM1L2o3ZXpNWjQ0Uk1QQk80QmUxN2Yra2dmY1J0VFlUNktlMFJ3NzJLcUhmV2t1YVREUVBnSm0KR3RXdDd1NjhEUDNkVjBrdkduNENGSTFKUWFrUE83cjBzZUhqT0dHR3BoMGNIQ0R5UlgvUmVEQitkOWxQR2Y3eQpObnYzejVURmYvZFJMcFNldGNDQ1dydnNqUUtCZ1FESC9wdEgzRkNRaEQrNytwR2JRcERuU2xkU3NPQUFBaS8xCnBHQjY3WmwzejUxMnE1Q3Q0QVVNcWZvaU5WMnJrbXBZenc0ZmRsMEtJK2d3S1NpWWZCNFhNSXdqa2lrd3ZyUWcKOTUwbnlrS2ovM0oxbTJrMFArVllOQmpUTTZjTHR5K1Rqa3lKMlR6cWk2N2ZpaDNPeFFYS0wvcXlkOFlNUkMzZAp2MVJBSlRIdWVRS0JnQjhIOFBObmdEVmt0bnFkaTd2dnhJN2VSb0htbU1sRmJNaW5yREFIem9oelMvbk9oMk1vClF4T1V5SE1pRiswU1Q2R2JZKzZHemVvNmdpeWVUNm8vR1lXMWs0YmJEVC9HajlzejNoRWQ3djlIbit0YmpCYmYKU09PK3E2MmE2RUtLeGp2bm5aMjRQdWRLTnVpcUhRcFlmMUFSNDF0aHI4Z05QdzhNOXo1YkVES0ZBb0dBSnc0RApTTTh2TkdsL0FMaDN3cmdIRUFPbWRkRndqTS9naWJtbDFadWNncGNhaXRnS0VzcFNjaHluYWhLOXpnbHpseEFvCkUrRExYbldRbkFjTmxHbDRmdExPS3d3WjJ4a0NtQVdDdlFoMFp3NDFUZDRoZDBDYkN0UnhuSnpUbkNnVHRGN3YKZDJQaXozS2puYWVkRm9uSERhcTg3Q2tUbGNXaXAxRDdwT01la3hFQ2dZQXdTelJvUmZqN09DRG1RR1BMRSt0eApESmRrWTJ3N3NXbkdjVFI1cm1vZm1GaWlZSUlWUWdBdVAxcVJmYkZvamgwVzFmOW8zYlkvbkxlc2lzV2NhMmZ1Ck8xbklIbjlCNk1lb3VEYlZ1NytubnlGZlkrYzFOUUpYVmRlMDVjQklZQjlrTEFJNnFBQUVabjFRTThMOWhGQ3YKcEVaLzlIZlhwR2d3Y2tYTTdCTGxlUT09Ci0tLS0tRU5EIFBSSVZBVEUgS0VZLS0tLS0KLS0tLS1CRUdJTiBDRVJUSUZJQ0FURS0tLS0tCk1JSUNwRENDQVl3Q0NRRHczTW5uTDJJR2RqQU5CZ2txaGtpRzl3MEJBUXNGQURBVU1SSXdFQVlEVlFRRERBbHMKYjJOaGJHaHZjM1F3SGhjTk1Ua3hNVEl4TVRVMU9USTNXaGNOTWpBeE1USXdNVFUxT1RJM1dqQVVNUkl3RUFZRApWUVFEREFsc2IyTmhiR2h2YzNRd2dnRWlNQTBHQ1NxR1NJYjNEUUVCQVFVQUE0SUJEd0F3Z2dFS0FvSUJBUUNkCmNiWHhkUk82ejU3VytJYXB0cHkyZkJRdGc1d2VTREREWjFWdmZxWXdTLzByWE1MQUtmMnF0ZVY4dFVHRGxOQ3EKMmtIZGRUd3hiRTZsTjNnMVB5YU9yLzI5Q256UzUvYTN3UVVjN1RVbkF4U2FCWlVvcVBnekxWVGV0TXZjdEo0TwpReGJMVG55OExIYzBjci85R0g4VWt5K2J2ckJQVldpa1paTEtwQUtpcXYwZHUwSjRRSWFWTkJjSG1mR3pIY0U5CjYyaDZicWJ2VFBMN2JwdStuTFhFSkFrNmVUS1ZzZ0tmOVNlZHd2V2dHT0VJTGhIVEs0K3pCczk3bEhyd3V6dFQKV2ZrYjl5clUxS3h4RXVhN3grS0ZMcEczcUp1OXd4clJ5SUJXT0wrTm84TURJTDF2N1BVRnBTdmpjemw3Z0tVQQppeTRJUUxxeCtUdStIR0JBdXVTbEFnTUJBQUV3RFFZSktvWklodmNOQVFFTEJRQURnZ0VCQURkRlR1eDlnRGcyClI0Wk1IWGpsT2hXVWxsYml6azEzREVKNzhUc3dMTU5ub0U5VTRpMHV3QjZTY1MwODBKOEljbjlua1lVRWJSU24KSG9tV2FlbUxXd1JzN2FCclE1aGdNaER1QUZOem85ZUNmdUswa3grWlAzZWM2Q1hJVGNFTlJQZ05QVy9pNU55bQptKzByQjlwUnpodDNNMllvZEpPVnh5Y3dlVE13UmFrZlRXYU1wT0hySWtoekVoMEJwQ0Jyakw3RlRCb1lISVNpCkNzdjFuSVdSQ3NJWXNJR21sZ2gxT1J0d2pwYkgwMExiSU1YZ1Bla0hUcnFtalA4czZ2QWhaaXJ5dTUyd3IvQTQKRXBPNzB2Z2QvVUxBQzArVDJGT0dvdktJazRkeFB2ZHFxVDIyMEtTMEEwSFFmL2VuOXErckVSaC96RmJ2RjFmUwpWS0RUNEI0NzZhdz0KLS0tLS1FTkQgQ0VSVElGSUNBVEUtLS0tLQo='

cert=base64.b64decode(cert)

open("/tmp/server.pem","w").write(cert)

httpd = BaseHTTPServer.HTTPServer(('0.0.0.0', 8443), SimpleHTTPServer.SimpleHTTPRequestHandler)
httpd.socket = ssl.wrap_socket(httpd.socket, certfile='/tmp/server.pem', server_side=True)
httpd.serve_forever()
```

# FTP Server

#### sudo python -m pyftpdlib -p 21 -V -D -w
```
-i ADDRESS, --interface=ADDRESS
     specify the interface to run on (default all interfaces)
 
-p PORT, --port=PORT
     specify port number to run on (default 2121)

-w, --write
     grants write access for logged in user (default read-only)

-d FOLDER, --directory=FOLDER
     specify the directory to share (default current directory)

-n ADDRESS, --nat-address=ADDRESS
     the NAT address to use for passive connections

-r FROM-TO, --range=FROM-TO
     the range of TCP ports to use for passive connections (e.g. -r 8000-9000)

-D, --debug
     enable DEBUG logging evel

-v, --version
     print pyftpdlib version and exit

-V, --verbose
     activate a more verbose logging

-u USERNAME, --username=USERNAME
     specify username to login with (anonymous login will be disabled and password required if supplied)

-P PASSWORD, --password=PASSWORD
     specify a password to login with (username required to be useful)
```
