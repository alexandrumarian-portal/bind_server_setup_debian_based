# bind_server_setup_debian_based

sources : 
```
https://lowendbox.com/blog/how-to-create-a-dns-server-on-debian-stretch/
https://blog.andreev.it/?p=4219
https://www.cloudns.net/blog/10-most-used-dig-commands/
https://www.cloudns.net/blog/basic-dns-terms-you-should-know/
https://www.ubuntupit.com/everything-you-need-to-know-about-ubuntu-dns-servers/
```

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
4. Which is the responsible mail server for your domain?
```
dig MX example.com +short
```
5. With which IP address a domain name is associated with?
```
dig -x 1.2.3.4
```
6. Which are the name servers, responsible for the TLDs (top-level domains)?
```
dig NS com +short
```
7. How to check if your DNS zone is synchonized over all authoritative name servers?
```
dig example.com +nssearch
```
8. How can I check when the cache of an answer will expire?
```
dig example.com +noall +answer
```
9. How to check is a zone existing on a name server?
```
dig SOA example.com @ns1.example.com 
```
10. How to check which value is in cache in a given resolver?
```
dig example.com @8.8.8.8
```











