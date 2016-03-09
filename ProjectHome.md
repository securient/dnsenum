## IMPORTANT - NEW DOWNLOAD ##
### You can find dnsenum on GITHUB from now on: https://github.com/fwaeytens/dnsenum.git ###


The purpose of Dnsenum is to gather as much information as possible about a domain. The program currently performs the following operations:

1) Get the host's addresse (A record).
2) Get the namservers (threaded).
3) Get the MX record (threaded).
4) Perform axfr queries on nameservers and get BIND versions(threaded).
5) Get extra names and subdomains via google scraping (google query = "allinurl: -www site:domain").
6) Brute force subdomains from file, can also perform recursion on subdomain that have NS records (all threaded).
7) Calculate C class domain network ranges and perform whois queries on them (threaded).
8) Perform reverse lookups on netranges ( C class or/and whois netranges) (threaded).
9) Write to domain\_ips.txt file ip-blocks.