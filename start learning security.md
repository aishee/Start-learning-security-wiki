# How to start learning security
I frequently get questions about how to get started in the field
of cybersecurity, if you're looking for some extra material, here are some good resources:

- Web Security
   - [The Tangled Web](http://www.amazon.com/Tangled-Web-Securing-Modern-Applications-ebook/dp/B006FZ3UNI) by Michal Zalewski
   - [The OWASP Top Ten](https://www.owasp.org/index.php/Category:OWASP_Top_Ten_Project)
- Exploitation
   - [Hacking: The Art of Exploitation](http://www.amazon.com/Hacking-The-Art-Exploitation-Edition/dp/1593271441) by Jon Erickson
   - [SkullSecurity](https://blog.skullsecurity.org/)
- Malware
   - [Contagio](http://contagiodump.blogspot.com/)
   - [Offensive Computing](http://www.offensivecomputing.net/)
- Cybercrime
   - [Krebs on Security](http://krebsonsecurity.com/)

Above all, the best way to learn security is by doing it. Read
some of the above materials, find an attack or defense you'd like
to try, set up a test environment (don't attack anyone else's
stuff), and have at it!

# How to get started

## Basics
* Setup a virtual machine with your favorite operating system. If you haven’t used Linux yet, the latest Ubuntu LTS is a good start: http://www.ubuntu.com/download/desktop
* Feel comfortable in a linux or windows shell
* Having one VM running Kali Linux (https://www.kali.org/) can be useful because it comes with a lot of useful tools, but is not necessary.
* This youtube channel has a great introduction to “hacking” and also has some very nice video “write-ups” of past CTFs so you can get a feel of what to expect: https://www.youtube.com/playlist?list=PLhixgUqwRTjxglIswKp9mpkfPNfHkzyeN

## Getting started
You can go through the materials: Computer Security.
* http://www.icir.org/vern/cs161-sp13/
* http://speed.cis.nctu.edu.tw/~ydlin/course/cn/ics.html

A huge list of additional readings is available at http://dfir.org/?q=node/8/.


## Hacking tutorials and Challenges

The [CyberQuests](http://uscc.cyberquests.org/) challenges happen on a monthly basis and involve various types of computer security puzzles.

The Youtube channel [liveoverflow](https://www.youtube.com/channel/UClcE-kVhqyiHCcjYwcpfj9w) has an awesome [series](https://www.youtube.com/watch?v=iyAyN3GFM7A&list=PLhixgUqwRTjxglIswKp9mpkfPNfHkzyeN) on reverse engineering and low-level exploitation.

https://exploit-exercises.com/ provides a variety of virtual machines, documentation and challenges that can be used to learn about a variety of computer security issues such as privilege escalation, vulnerability analysis, exploit development, debugging, reverse engineering, and general cyber security issues.

https://ctftime.org/ is a website that lists many CTF competition. There is one almost every weekend. Just participate! Don't now where to start? Search for CTF write-ups or have a look at liveoverflow.

PIVOT seems to have a challenge where you have extract data from network traffic and other
formats: http://pivotproject.org/challenges/digital-forensics-challenge and http://pivotproject.org/challenges/file-carving. Instead of Wireshark you can also use Bro.

__This Wiki__ provides several guides which you should have a look at.

## Network Intrusion Detection and Forensics
We have good experiences using Bro
* http://www.bro.org
* Bro Exercise: https://www.bro.org/community/exchange2013.html


## CCDC Resources
* National CCDC Preparation
   * http://blog.spiderlabs.com/2013/04/web-application-defenders-cookbook-ccdc-blue-team-cheatsheet.html
   * http://blog.strategiccyber.com/2013/04/24/national-ccdc-red-team-fair-and-balanced/
   * http://blog.strategiccyber.com/2012/10/04/dirty-red-team-tricks-ii-at-derbycon-2-0/
* CCDC
   * [Description of event from red team perspective](http://www.reddit.com/r/netsec/comments/17dfqf/red_teaming_a_ccdc_practice_event/)
   * [Finding malware with Sysinternals tools](http://channel9.msdn.com/Events/TechEd/NorthAmerica/2012/SIA302)
   * [Hunting rootkits on Linux](http://cayfer.bilkent.edu.tr/~cayfer/linux/Detecting_and_Removing_Rootkits.html)


## Unix System Admin
As a challenge, pick a Linux distribution or a BSD you are not familiar with (how about CentOS or FreeBSD) and get the following services running:
* nginx webserver with PHP over fastcgi
* PostgreSQL and MySQL database
* Some web applications (e.g. Joomla, Wordpress, ...)
* Postfix Mailserver with virtual user management in MySQL
* Dovecot IMAP server
* TLS Certificates for HTTPS, SMTPS, IMAPS
* Apache with mod_security as reverse proxy in front of nginx (you would probably not do this in production but see it as an exercise)
* Compile and install some of the software above from source

## Windows
First we're going to cover some of the most magnificent tools in the Windows sysadmin's arsenal, the Sysinternals suite. This a set of tools written by some Windows experts that give you an incredible level of access to a lot of low-level Windows APIs, which allow you to find malicious stuff really effectively. The best place to grab these tools is from http://live.sysinternals.com/tools/

As soon as you visit that URL, you'll notice that there are a lot of tools in the suite. Not all of them are particularly relevant to us, but there are a few that are essential. In particular: Process Explorer (like a more powerful task manager), Autoruns (like a more powerful msconfig), and TcpView (a netstat-like tool). When I was learning these, the best resource I used was a video by the main creator, Mark Russinovich, about how to use them to manually fight malware. The latest version of that talk is available here: https://www.youtube.com/watch?v=xxf8Tz7QGjU.
