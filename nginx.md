# Nginx
## Description

Nginx is a high performance HTTP server. At the same time it is also a reverse proxy and IMAP/POP3 proxy server. Nginx popularized itself by providing rich feature set, high performance, stability, simple configuration and low resource consumption. Ngnix open source web server is powering more than 130 million website. And the popularity of this platform among high traffic website is noteworthy.

Nginx claims to provide with a better load balancing with cookies. The platform has kept the 4 mega trends of the IT sector: Cloud, Big data, Mobility and Social in mind to manage the traffic in a sophisticated manner. According to the [recent Ntecraft web survey] (http://news.netcraft.com/archives/2015/04/20/april-2015-web-server-survey.html "recent Ntecraft web survey"), Nginx has served or proxied 21.43% of the busiest websites. [Igor Sysoev] (http://en.wikipedia.org/wiki/Igor_Sysoev "Igor Sysoev") must be a proud man who originally wrote Nginx.

**References:** http://nginx.org/en/

## Quick Facts
* **Main Site** - http://nginx.com/
* **Documentation** - http://nginx.org/en/docs/
* **Wikipedia** - http://en.wikipedia.org/wiki/Nginx
* **Main Git Repo** - https://github.com/nginx/nginx
* **Current Version** - NGINX Plus R6
* **Current Version Released** - 14 April 2015

### Google Trends

Nginx has been gaining popularity on a gradual basis. If one tracks the Google Trends, he will find the popularity of the keyword "Nginx" on the rise. Here are some of the Google Trends about Nginx: Nginx, Nginx - Web server Software, Php nginx, Nginx vs Apache, nginx server, ubuntu nginx, nginx proxy, install nginx and many more.

The worldwide data analytics of Google Trend shows that the particular keyword "Nginx" is mostly popular in China following by Russia, Ukraine, Belarus, Latvia, South Korea, Hong Kong, Moldova, Estonia and Taiwan.

**Source:** http://www.google.com/trends/explore#q=Nginx

### Number of downloads over time

More than 3 million times.

**Source:** http://nginx.com/blog/12-reasons-why-nginx-is-the-standard-for-containerized-applications-and-deploying-microservices/

## Major versions

Version No.| Release Date | Documentation | Status
:-----------:|:------------:|:-------------:|:-------
NGINX Plus R6 | 14 April 2015 | http://nginx.com/blog/nginx-plus-r6-released/ | Commercially-supported version with added features
v1.9.0 | 28 April 2015 | http://nginx.org/en/CHANGES | Mainline Version with Stream Module
v1.8.0 | 21 April 2015 | http://nginx.org/en/CHANGES-1.8 | Stable Version with Hash load balancing method, Backend SSL certificate verification, Experimental thread pools support, Proxy_request_buffering and more
v1.6.3 | 7 April 2015 | http://nginx.org/en/CHANGES-1.6 | Legacy version
v1.4.7 | 18 March 2014 | http://nginx.org/en/CHANGES-1.4 | Legacy version

## Security exploits
Following are the known issues of Nginx:

* **SSL session reuse vulnerability:** The severity of this issue has been identified as medium. Common Vulnerabilities and Exposures (CVE), [CVE-2014-3616] (http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-3616 "CVE-2014-3616") was identified by [Antoine Delignat-Lavaud] (http://antoine.delignat-lavaud.fr/ "Antoine Delignat-Lavaud"). Ability to reuse a cached SSL session for an unrelated context meant potential "virtual host confusion" attacks. Though it was vulnerable to v0.5.6 - v1.7.4, it is not vulnerable to v1.7.5+ and v1.6.2+

     Following are some of the available Security Advisory links regarding this issue:
     - [Nginx security advisory (CVE-2014-3616)] (http://mailman.nginx.org/pipermail/nginx-announce/2014/000147.html "Nginx security advisory (CVE-2014-3616)")
     - [Debian Security Advisory] (http://www.debian.org/security/2014/dsa-3029 "Debian Security Advisory")
     
* **STARTTLS command injection:** This is also among the medium vulnerable security exploits. This issue caused the vulnerability of inserting commands into encrypted SMTP sessions by sending a cleartext command that is processed after TLS. According to its CVE([CVE-2014-3556] (http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-3556 "CVE-2014-3556")) this could also be related to a "plaintext command injection" attack and is similar to [CVE-2011-0411] (http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2011-0411 "CVE-2011-0411"). According to [nginx security advisory (CVE-2014-3556)] (http://mailman.nginx.org/pipermail/nginx-announce/2014/000144.html "nginx security advisory (CVE-2014-3556)") the issue was discovered by Chris Boulton. The [patch] (http://nginx.org/download/patch.2014.starttls.txt "patch") and [pgp] (http://nginx.org/download/patch.2014.starttls.txt.asc "pgp") documentation for this issue are also available. **STARTTLS command injection** is marked as vulnerable to v1.5.6 - v1.7.3 but it is not vulnerable to 1.7.4+ and 1.6.1+

    Following are some of the available Security Advisory links regarding this security elxploit:
    - [Nginx security advisory (CVE-2014-3556)] (http://mailman.nginx.org/pipermail/nginx-announce/2014/000144.html?_ga=1.135323249.1375076917.1431890626 "Nginx security advisory (CVE-2014-3556)")
    - [Red Hat Bugzilla – Bug 1126891] (https://bugzilla.redhat.com/show_bug.cgi?id=1126891 "Red Hat Bugzilla – Bug 1126891")
 
* **SPDY heap buffer overflow:** This enabled remote attackers to execute arbitrary code via a crafted request. While it is Vulnerable to v1.3.15 - v1.5.11, it is not vulnerable in v1.5.12+ and v1.4.7+. The patch for the problem could be found [here] (http://nginx.org/download/patch.2014.spdy2.txt "here"). The pgp could be found [here] (http://nginx.org/download/patch.2014.spdy2.txt.asc "here").
   
    Following are some of the available Security Advisory links regarding this security elxploit:
    - [Nginx security advisory (CVE-2014-0133)] (http://mailman.nginx.org/pipermail/nginx-announce/2014/000135.html?_ga=1.168482145.1375076917.1431890626 "Nginx security advisory (CVE-2014-0133)")
    - [OpenSUSE Security Update] (http://lists.opensuse.org/opensuse-updates/2014-03/msg00095.html "OpenSUSE Security Update")
     
* **SPDY memory corruption:** As per the official Nginx documents: A bug in the experimental SPDY implementation in nginx 1.5.10 was found, which might allow an attacker to corrupt worker process memory by using a specially crafted request, potentially resulting in arbitrary code execution. It was only identified in v1.5.10 and is not vulnerable to v1.5.11+. [Lucas Molas] (https://hackerone.com/lmolas "Lucas Molas") is the person behind the identification of this security exploit. The patch for the issue can be found [here] (http://nginx.org/download/patch.2014.spdy.txt "here"). The pgp can be dound [here] (http://nginx.org/download/patch.2014.spdy.txt.asc "here").

    Following are some of the available Security Advisory links regarding this security elxploit:
    - [Nginx security advisory (CVE-2014-0088)] (http://mailman.nginx.org/pipermail/nginx-announce/2014/000132.html?_ga=1.92405213.1375076917.1431890626 "Nginx security advisory (CVE-2014-0088)")
    - [SecurityTracker Alert ID: 1030150] (http://www.securitytracker.com/id/1030150 "SecurityTracker Alert ID: 1030150")
    
* **Request line parsing vulnerability:** This enabled an attacker to bypass security restrictions in certain
configurations by using a specially crafted request. [Ivan Fratric] (https://twitter.com/ifsecure "Ivan Fratric") of Google discovered this security exploit. It is vulnerable to v0.8.41 - v1.5.6 but not vulnerable to v1.5.7+ and 1.4.4+. The patch for the security exploit can be found [here] (http://nginx.org/download/patch.2013.space.txt "here") and the pgp can be found [here] (http://nginx.org/download/patch.2013.space.txt.asc "here").

    Following are some of the available Security Advisory links regarding this security elxploit:
    - [Nginx security advisory (CVE-2013-4547)] (http://mailman.nginx.org/pipermail/nginx-announce/2013/000125.html?_ga=1.160159485.1375076917.1431890626 "Nginx security advisory (CVE-2013-4547)")
    - [SUSE:openSUSE-SU-2013:1745] (http://lists.opensuse.org/opensuse-updates/2013-11/msg00084.html "SUSE:openSUSE-SU-2013:1745")
    
* **Memory disclosure with specially crafted HTTP backend responses:** The problem led to a denial of service or a disclosure of a worker process memory on a specially crafted response from an upstream proxied server. The severity of this issue is marked as medium. It is vulnerable to v1.1.4 - v1.2.8 and v1.3.9 - v1.4.0. But it is not vulnerable to v1.5.0+, v1.4.1+ and v1.2.9+. The patch and pgp to the security exploits are: [The patch for v1.3.9 - v1.4.0] (http://nginx.org/download/patch.2013.chunked.txt "The patch for v1.3.9 - v1.4.0"), [The patch for v1.1.4 - v1.2.8] (http://nginx.org/download/patch.2013.proxy.txt "The patch for v1.1.4 - v1.2.8"), [pgp for v1.3.9 - v1.4.0] (http://nginx.org/download/patch.2013.chunked.txt.asc "pgp for v1.3.9 - v1.4.0"), [pgp for v1.1.4 - v1.2.8] (http://nginx.org/download/patch.2013.proxy.txt.asc "pgp for v1.1.4 - v1.2.8").
 
    Following are some of the available Security Advisory links regarding this security elxploit:
    - [Nginx security advisory (CVE-2013-2070)] (http://mailman.nginx.org/pipermail/nginx-announce/2013/000114.html?_ga=1.59431405.1375076917.1431890626 "Nginx security advisory (CVE-2013-2070)")
    - [oss-security] (http://seclists.org/oss-sec/2013/q2/291 "oss-security")
    
* **Stack-based buffer overflow with specially crafted request:** The severity of this issue is major. This could occur in a worker process while handling a specially crafted request, potentially resulting in arbitrary code execution. The security exploit is a concern to v1.3.9 - v1.4.0. But it should be fine in v1.5.0+ and v1.4.1+. Greg MacManus of iSIGHT Partners Labs has been attributed with the credit of identifying this issue. The patch for this issue can be found [here] (http://nginx.org/download/patch.2013.chunked.txt "here") and the pgp can be found [here] (http://nginx.org/download/patch.2013.chunked.txt.asc "here").

    Following are some of the available Security Advisory links regarding this security elxploit:
    - [Nginx security advisory (CVE-2013-2028)] (http://mailman.nginx.org/pipermail/nginx-announce/2013/000112.html?_ga=1.89914971.1375076917.1431890626 "Nginx security advisory (CVE-2013-2028)")
    - [Packetstormsecurity] (http://packetstormsecurity.com/files/121675/Nginx-1.3.9-1.4.0-Denial-Of-Service.html "Packetstormsecurity")
    
* **Vulnerabilities with Windows directory aliases:** [Vladimir Kochetkov] (https://github.com/kochetkov/ "Vladimir Kochetkov") has identified this issue. The issue is related to security restrictions bypass via (1) a trailing . (dot) or (2) certain "$index_allocation" sequences in a request. While this issue is vulnerable to nginx/Windows 0.7.52-1.3.0, it is not vulnerable in v1.3.1+ and 1.2.1+. 

    Following are some of the available Security Advisory links regarding this security elxploit:
    - [Nginx security advisory] (http://mailman.nginx.org/pipermail/nginx-announce/2012/000086.html?_ga=1.165204735.1375076917.1431890626 "Nginx security advisory")
    - [PT-2012-06: Security restrictions bypass in nginx for Windows] (http://english.securitylab.ru/lab/PT-2012-06 "PT-2012-06: Security restrictions bypass in nginx for Windows")
    
* **Buffer overflow in the ngx_http_mp4_module:** The issue was discovered by [Matthew Daley] (https://github.com/mdaley "Mathew Daley"). This enabled a remote attacker overwrite memory locations in a worker process via crafted mp4 file if the ngx_http_mp4_module is used. This is vulnerable to v1.1.3-1.1.18 and v1.0.7-1.0.14. Not vulnerable in v1.1.19+ and 1.0.15+. The patch file can be found [here] (http://nginx.org/download/patch.2012.mp4.txt "here") and the pgp file can be found [here] (http://nginx.org/download/patch.2012.mp4.txt.asc "here").
 
    Following are some of the available Security Advisory links regarding this security elxploit:
    - [Nginx security advisory] (http://mailman.nginx.org/pipermail/nginx-announce/2012/000080.html?_ga=1.126557517.1375076917.1431890626 "Nginx security advisory")
    - [Exchange.xforce security advisory] (https://exchange.xforce.ibmcloud.com/vulnerabilities/74831 "Exchange.xforce security advisory")

* **Memory disclosure with specially crafted backend responses:** Matthew Daley is once again responsible for discovering  yet another major issue. This can lead to a disclosure of previously freed memory on specially 
crafted response. The issu is vulnerable to v0.1.0-1.1.16 but non-vulnerable to v1.1.17+ and 1.0.14+. The patch for the issue can be found [here] (http://nginx.org/download/patch.2012.memory.txt "here") and the pgp can be found [here] (http://nginx.org/download/patch.2012.memory.txt.asc "here").

    Following are some of the available Security Advisory links regarding this security elxploit:
    - [Nginx security advisory] (http://mailman.nginx.org/pipermail/nginx-announce/2012/000076.html?_ga=1.54645099.1375076917.1431890626 "Nginx security advisory")
    - [Openwall security advisory] (http://www.openwall.com/lists/oss-security/2012/03/15/5 "Openwall security advisory")
    
* **Buffer overflow in resolver:** Successful exploitation of this issue allows remote attackers to execute arbitrary code in context of the vulnerable application. This could be considered as a minor issue. While it is vulnerable to v0.6.18-1.1.7, it is not vulnerable in v1.1.8+ and v1.0.10+. Upgrading from vulnerable version will solve this problem. The changes can be traced [here] (http://trac.nginx.org/nginx/changeset/4268/nginx "here")

* **Vulnerabilities with invalid UTF-8 sequence on Windows:** This is yet another major security exploit in terms of severity. As per [CVE-2010-2266] (http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2010-2266 "CVE-2010-2266"): it can allow remote attackers to cause a denial of service (crash) via certain encoded directory traversal sequences that trigger memory corruption, as demonstrated using the "%c0.%c0." sequence. This is vulnerable to nginx/Windows 0.7.52-0.8.40. But the issue is ineffective in v0.8.41+ and v0.7.67+. More information about this issue can be found [here] (https://www.exploit-db.com/exploits/13818/ "here")

* **Vulnerabilities with Windows file default stream:** This is also marked as one of the major security exploits. Successful attack of this issue can allow remote attackers to obtain source code or unparsed content of arbitrary files under the web document root. It is vulnerable to nginx/Windows 0.7.52-0.8.39. But it is non velnerable in v0.8.40+ and v0.7.66+. 

    Following are some of the available Security Advisory links regarding this security elxploit:
    - [viernes, 11 de junio de 2010] (http://spa-s3c.blogspot.com/2010/06/full-responsible-disclosurenginx-engine.html "viernes, 11 de junio de 2010")
    - [Exploit Database Reference] (https://www.exploit-db.com/exploits/13822/ "Exploit Database Reference")
    
* **Vulnerabilities with Windows 8.3 filename pseudonyms:** The severity of this issue has been identified as major. According to [Coresecurity] (http://www.coresecurity.com/content/filename-pseudonyms-vulnerabilities "Coresecurity"): by abusing this weakness an attacker can bypass security options implemented in the web server. They exemplified by saying that file.shtml will become FILE~1.SHT resulting in unprocessed service of files. This issue is vulnerable to nginx/Windows 0.7.52-0.8.32 and non-vulnerable in v0.8.33+ and v0.7.65+.

* **An error log data are not sanitized:** According to [CVE-2009-4487] (http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2009-4487 "CVE-2009-4487") nginx 0.7.64 writes data to a log file without sanitizing non-printable characters, which might allow remote attackers to modify a window's title, or possibly execute arbitrary commands or overwrite files, via an HTTP request containing an escape sequence for a terminal emulator. The severity of this issue is yet to be identified. And it remains vulnerable to all the versions.
 
* **The renegotiation vulnerability in SSL protocol:** The severity is identified as major. While it is vulnerable to v 0.1.0-0.8.22, it is not vulnerable in v0.8.23+ and v0.7.64+. As the issue concerns with SSL and TLS, it threatens the privacy. The patch for this issue can be found [here] (http://nginx.org/download/patch.cve-2009-3555.txt “here”) and pgp can be found [here] (http://nginx.org/download/patch.cve-2009-3555.txt.asc “here”).
 
* **Directory traversal vulnerability:** The severity of this issue has been identified as minor being vulnerable to v0.1.0-0.8.16. But it is not vulnerable in v0.8.17+ and v0.7.63+. Using this weakness it was possible to overwrite arbitrary or authenticate unauthorized users without proper permission. More details could be found on [CVE-2009-3898] (http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2009-3898 “CVE-2009-3898”).
 
* **Buffer underflow vulnerability:** According to [Vulnerability Note VU#180065] (http://www.kb.cert.org/vuls/id/180065 “Vulnerability Note VU#180065”) this issue is such where a remote, unauthenticated attacker may be able to execute arbitrary code in the context of the worker process or cause the worker process to crash, resulting in a denial of service. The severity of this issue has been identified as major. It is vulnerable to v 0.1.0-0.8.14. But it is not vulnerable in v 0.8.15+, v0.7.62+, v0.6.39+ and v0.5.38+. The patch file for this security exploit can be found [here] (http://nginx.org/download/patch.180065.txt “here”) and the pgp can be found [here] (http://nginx.org/download/patch.180065.txt.asc “here”).
 
* **Null pointer dereference vulnerability:** The severity of this issue is major as well. According to [CVE-2009-3896] (http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2009-3896 “CVE-2009-3896”) this could lead to a denial of service via long URI. It is vulnerable to v0.1.0-0.8.13. But it is not vulnerable in v0.8.14+, 0.7.62+, 0.6.39+ and 0.5.38+. The patch for the security exploit can be found [here] (http://nginx.org/download/patch.null.pointer.txt “here”) and the pgp can be found [here] (http://nginx.org/download/patch.null.pointer.txt.asc “here”).

## Companies using Nginx

According to the [Netcraft May 2015 Web Server Survey] (http://news.netcraft.com/archives/2015/05/19/may-2015-web-server-survey.html “Netcraft May 2015 Web Server Survey”) though Nginx lost a little bit of overall market share, it is still doing well within the million busiest sites. Nginx is especially popular among the high volume traffic websites. Following are some of the popular platforms using Nginx:
 * [NETFLIX] (https://www.netflix.com/ "NETFLIX")
 * [box] (https://www.box.com/ "box")
 * [hulu] (www.hulu.com/ "hulu")
 * [Wordpress] (https://wordpress.com/ "Wordpress")
 * [MaxCDN] (https://www.maxcdn.com/ "MaxCDN")
 * [Yandex] (https://www.yandex.com/ "Yandex")
 * [Dropbox] (https://www.dropbox.com/ "Dropbox")
 * [Pinterest] (https://www.pinterest.com/ "Pinterest")
 * [Rambler] (http://www.rambler.ru/ "Rambler")
 
## Features

Nginx has a clear impact of serving people’s interest as a successful web server platform. Almost all the web servers which are in hunt with their existence and growth in the market have; and will have the basic features in common. But the proper use and tuning of each of these platforms will put one, ahead of another in some cases. Of course the expectancy of desired outcome from a web server will also play an important role in determining which one web server platform has the upper hand in a particular situation. But following are some of the features which have made Nginx popular among the users:

  * Nginx is capable of giving better performance in terms of stability and scalability.
  * Nginx can deliver remarkable speed with lower memory consumption without much of a tuning effort.
  * Nginx is Event based and asynchronous which allows a better FLV and MP4 streaming.
  * Load Balancing, Caching and Reverse Proxy services are delivered with ease.
  * Many would find Multiple SSL sites working  easily with Nginx.
  * As Nginx offers a premium product too, they can afford to run a team of full time top notch developers to give the best performance and maintain real time security. Having said that, the fact is: Nginx do have less security exploits as per the official and unofficial documentations.
   
Above features set high standards for Nginx. If you wish to go through a detailed documentation of features, here are some links for you:

  * [Official Documentation of Basic HTTP Server Features] (http://nginx.org/en/#basic_http_features “Official Documentation of Basic HTTP Server Features”)
  * [Other HTTP Server Features] (http://nginx.org/en/#other_http_features “Other HTTP Server Features”)
  * [Mail Proxy Server Features] (http://nginx.org/en/#mail_proxy_server_features “Mail Proxy Server Features”)
  * [TCP proxy server features] (http://nginx.org/en/#tcp_proxy_server_features “TCP proxy server features”)
  * You might also like the [Wikipidea Documentation of Nginx HTTP Proxy and Web Server Features] (http://en.wikipedia.org/wiki/Nginx#HTTP_proxy_and_Web_server_features “Wikipidea Documentation of Nginx HTTP Proxy and Web Server Features”)

## Major plugins

Top 5 to 10 major plugins for this, if available.

## Internals (Algorithms, Protocols, formats, etc)

For each of these sections, please try to link to GitHub for specific code examples whenever possible.

### Algorithms used by PRODUCT_NAME

### Data Structures used by PRODUCT_NAME

### Protocols used or supported by PRODUCT_NAME

### File or data formats used or supported by PRODUCT_NAME


## Articles


## Tutorials

### Installation


#### On Windows


#### On Mac OS X


#### On Ubuntu Linux


#### On Red Hat Linux


### Beginner Tutorials


### Advanced Tutorials


## Positive Reviews


## Negative Reviews
