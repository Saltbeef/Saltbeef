# Shell setup


## Extra packages:

* `apt install -y zsh curl git screen vim direnv tree mc whois python3-distutils python3-apt`


## OhMyZSH

* `sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`
* edit zsh theme to dieter
* add direnv to .zshrc plugins


## edit .vimrc

```
set ts=4
set expandtab
```


## Terraform

```
apt-get update && apt-get install -y gnupg software-properties-common curl
curl -fsSL https://apt.releases.hashicorp.com/gpg | apt-key add -
apt-add-repository "deb [arch=amd64] https://apt.releases.hashicorp.com $(lsb_release -cs) main"
apt-get update && apt-get install terraform
```


## .screenrc

```
attrcolor b ".I"
bind F eval "hardstatus alwayslastline"
bind f eval "hardstatus ignore"
caption always
defbce "on"
defflow off
defscrollback 30000
hardstatus alwayslastline
hardstatus string '%{= Kd} %{= Kd}%-w%{= Kr}[%{= KW}%n %t%{= Kr}]%{= Kd}%+w %-= %{KG} %H%{KW}|%{KY}%101`%{KW}|%D %M %d %Y%{= Kc} %C%A%{-}'
msgminwait 2
msgwait 15
startup_message off
term xterm-256color
termcapinfo xterm 'Co#256:AB=\E[48;5;%dm:AF=\E[38;5;%dm'
termcapinfo xterm|xterms|xs|rxvt ti@:te@
vbell on
```


## Poetry

* `curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python -`

