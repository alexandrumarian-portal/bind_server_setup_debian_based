# bind_server_setup_debian_based

source : 
https://lowendbox.com/blog/how-to-create-a-dns-server-on-debian-stretch/

https://blog.andreev.it/?p=4219


10 most used DIG commands

1. How to find the website’s IP address?
 ``` 
 dig example.com
 dig example.com +short
 ```
2. How to find the name servers, responsible for your domain?
```
dig NS example.com +short
```
3. What is the delegation path to your DNS Zone?
```
dig example.com +trace
```
