README - dnsenum.pl VERSION: 1.2

multithread perl script to enumerate DNS information on a domain
and to discover non-contiguous ip blocks.

OPERATIONS:

	1) Get the host's addresse (A record).

	2) Get the namservers (threaded).

	3) Get the MX record (threaded).

	4) Perform axfr queries on nameservers (threaded).

	5) Get extra names and subdomains via google scraping
	   (google query = "allinurl: -www site:domain").

	6) Brute force subdomains from file, can also perform recursion
	   on subdomain that have NS records (all threaded).

	7) Calculate C class domain network ranges and perform whois
	   queries on them (threaded).

	8) Perform reverse lookups on netranges
	   ( C class or/and whois netranges) (threaded).

	9) Write to domain_ips.txt file ip-blocks.


PREREQUISITES: 

  Modules that are included in perl 5.10.0:
	Getopt::Long 
	IO::File 
	Thread::Queue

  Other Necessary modules:
	Must have:
		Net::IP
		Net::DNS 
		Net::Netmask
	Optional:
		Net::Whois::IP
		HTML::Parser
		WWW::Mechanize

  Perl ithreads support:
	perl version must be compliled with ithreads support.
	threads
	threads::shared


OPTIONS: run "perldoc dnsenum.pl".


Special thanks to perl and module developpers.

Filip Waeytens		<filip.waeytens[at]gmail.com>	
tix tixxDZ		<tixxdz[at]gmail.com>
	
