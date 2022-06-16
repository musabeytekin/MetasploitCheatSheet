# Metasploit Cheat sheet

## metasploit commands

- msfconsole : start metasploit

- msfdb run : start db of metasploit

- msfdb init: Prepares the database for metasploit

- db_status: check the metasploit db status

- search : search a module ⭐️⭐️

- info (or advanced): information about the module

- show : list modules or settings of modules

- use : use a module ⭐️⭐️

- options : show the settings of the module ⭐️⭐️

- set : set the configuration of the module ⭐️⭐️

- check: performs a preflight on the target via the relevant module.(ilgili modul araciligi ile hedefte on kontrol gerceklestirir.)

- run (or exploit): run the module or an operation

- sessions : show the received shell. passes between shells

- jobs : show the shells in backgorund

- back : back the selected modules 

- exit: stop metasploit


## Use of the search command

- search -key- : lists modules related to the given key
```
msf6> search ftp
```

- search -modulename- rank:good(or others) : lists modules related to the given key and given rank
```
msf6> search ftp rank:good
```

- search -modulename- cve:2019(or others) : lists modules related to the given key and given cve
```
msf6> search ftp cve:2018
msf6> search cve:2018

```

- search -modulename- type:excellent(or others) : lists modules related to the given key and given type
```
msf6> search ftp type:good
msf6> search type:good
```

- search -modulename- check:yes(or no) : lists modules related to the given key and given check type
```
msf6> search ftp check:no
msf6> search check:yes
```

## Use command

- use -modulename or modul number- 
```
msf6> use 114
msf6> use exploit/windows/ftp/sasser_ftpd_port
```

## Options Command
-  show module options after use module
```
msf6> use 114
msf6> options
```

## Show command
- Payloads that can be used in the module.
```
msf6 auxiliary(admin/http/gitstack_rest) > show payloads (or others)
```

