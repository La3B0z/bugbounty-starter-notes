# Books
1. The web application hacker's handbook
2. owasp testing guide
3. web hacking 101
4. breaking into infromation security
5. mastering mordern web peneteration testing

# Recon
* [ASN's(autonomous system numbers)](http://bgp.he.net) - (ip ranges , keyword searches)
* ARIN & RIPE - [arin](http://whois.arin.net/ui) 
                 [ripe](http://apps.db.ripe.net/db-web-ui/#/fulltextsearch)  whoislookups all
* Rev whois - [rev](http://reverse.report)
* shodan - [shodan](shodan.io)
* we cannot miss out on **burp**
* domlink [domlink](https://github.com/vysecurity/DomLink)
* [builtwith](https://builtwith.com/) - they also has a browser plugin it tells about stack that site is bult on and analytics
  
     #### Subdomain scraping enumeration
       
     * google dorks
     * [robtex](https://robtex.com)
     * waybackmachine
     * [sublist3r](https://github.com/aboul3la/Sublist3r)
     * [Amass](https://github.com/caffix/amass)
     * [subfinder](https://github.com/ice3man543/subfinder)
     * [Cloudflare Enumeration Tool](https://github.com/mandatoryprogrammer/cloudflare_enum)
     #### subdomain bruteforcing
     
     * massdns
     
        ex:
        `.subbrute.py /root/work/bin/all.txt $TARGET.com | ./bin/massdns -r resolvers.txt -t A -a -o -w massdns_output.txt -`
     * gobuster
     
        ex
        `gobuster -m dns -u  $TARGET.com -t 100 -w all.txt`
     * best dictonary file : [all.txt](https://gist.github.com/jhaddix/f64c97d0863a78454e44c2f7119c2a6a)
     * [scans.io](https://scans.io/)
     * [commonspeak](https://github.com/pentester-io/commonspeak)
   
  # Enumeration
  * masscan
  
      ex: `masscan -p1-65535 -iL $TARGET_LIST --max-rate 10000 -oG $TARGET_OUTPUT`
  * nmap
  * [brutespray](https://github.com/x90skysn3k/brutespray) 
  
       masscan output => map services scan -oG => brutespray credential bruteforcing.
      
       ex: `python brutespray.py --file nmap.gnmap -U /usr/share/wordlist/user.txt -P /usr/share/wordlist/pass.txt --threads 5 --hosts 5`
  * Eyewitness
  * [waybackursls](https://github.com/tomnomnom/waybackurls) enumeration using wayback
        
 #  Keeping track of all this 
      Xmind organization
      
   ![xmind.png](https://imgbbb.com/images/2019/07/09/xmind.png)
     
 # Identification and cve searching
 * buldwith 
 * retire.js 
 * [burp-vulners-scanner](https://github.com/vulnersCom/burp-vulners-scanner) 
 * wappanalyzer 
 # Parsing Heavy javascript sites 
 * zap Ajax spider - owasp zap 
 * [Linkfinder] 
 * [jsparser]
 
 # Content Discovery
 * Gobuster
 * Burp content discovery
 * Robots disallowed
 * wpscan
 * Seclists / RAFT / Digger wordlists
 * cmsmap
 * [custom wordlist](https://gist.github.com/jhaddix/b80ea67d85c13206125806f0828f4d10)
 
# XSS
* blind xss frameworks 
    * [bXSS](https://github.com/LewisArdern/bXSS)
    * [ezXSS](https://github.com/ssl/ezXSS)
    * XSS hunter
    * KnoXSS
    * Sleepy Puppy
* XSS polyglot
    *

# SSRF
* for testing in cloud https://gist.github.com/jhaddix/78cece26c91c6263653f31ba453e273b

# Subdomain Takeover  [info](https://github.com/EdOverflow/can-i-take-over-xyz)

