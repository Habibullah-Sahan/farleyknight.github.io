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
    
## Companies using PRODUCT_NAME

List 3 to 5 companies that use this product. Make sure to find a reputable page on the web that has this information. You should directly quote them somehow. If all you have are a set of slides by some guy that worked at the company that made the software, then take a screenshot and use the image as proof.

## Features

Top 3 to 5 features it has some of it's peers don't. In other words, these should be the 3 to 5 features that make the product stand out from it's competitors.

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
