# subDomain-Enum-Notes
* ctrl f (*) \*. \s.+ //for filter subdomains in vs سهم لتحت replace all
* when use any go lang tool use | cp ~/go/bin/toolname /usr/local/bin
* anew for remove dups // cat sudomains.txt | anew
## web sites to get subdomains :
1. https://securitytrails.com/  Apikey{-0zPXIrzTVvMrOv51YWuIODU8FgksRk-}
2. https://subdomainfinder.c99.nl/
3. https://shrewdeye.app/
4. assetnote worldlist >> best dns wordlist.txt 
## Tools :
1. subfinder
   - subfinder -d domain.com -all -recursive
2. assetfinder
    - echo "domain.com" | assetfinder --subs-only
3. ffuf
    - fuff http://FUZZ.domain.com -w wordlist or  name -fc 403,500 -v -t threads number
    - ffuf -w ~/wordlists/subdomains.txt -H "Host: FUZZ.ffuf.me" -u http://ffuf.me (virtual host attack)
4. amass
      - the path yo add apikeys ~/.config/amass/confing.yaml
      - amass intel -org "tesla" >> to get ASN num and cidr
      - amass intel -active -asn asnNum
      - amass intel -active -cidr cidrNum
##SSL / TLS :
   - First ou should get the name of company
   - then , go to https://crt.sh
