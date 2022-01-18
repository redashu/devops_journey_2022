## checking current shell

```
root@1f4a993d950f:/# x=10
root@1f4a993d950f:/# 
root@1f4a993d950f:/# echo $x
10
root@1f4a993d950f:/# echo hello
hello
root@1f4a993d950f:/# echo hello world
hello world
root@1f4a993d950f:/# echo x          
x
root@1f4a993d950f:/# echo $x
10
root@1f4a993d950f:/# 
root@1f4a993d950f:/# echo $SHELL
/bin/bash
root@1f4a993d950f:/# 


```

## Features of shell 

### alias  

```
date
Tue Jan 18 02:07:06 UTC 2022
root@1f4a993d950f:/# 
root@1f4a993d950f:/# 
root@1f4a993d950f:/# alias  d='date'
root@1f4a993d950f:/# 
root@1f4a993d950f:/# d
Tue Jan 18 02:07:20 UTC 2022
root@1f4a993d950f:/# 
root@1f4a993d950f:/# date
Tue Jan 18 02:07:39 UTC 2022
root@1f4a993d950f:/# 
root@1f4a993d950f:/# 
root@1f4a993d950f:/# alias  ashutoshh='cal 2 2022'
root@1f4a993d950f:/# 


```

### each user can have diff shell 

<img src="shell.png">

### changing shell for current temporary 

```
SHELL=/bin/sh 
root@1f4a993d950f:/# 
root@1f4a993d950f:/# 
root@1f4a993d950f:/# echo $SHELL
/bin/sh
root@1f4a993d950f:/# SHELL=/bin/bash
root@1f4a993d950f:/# 
root@1f4a993d950f:/# echo $SHELL
/bin/bash

```


### adjusting History size 

```
 echo $HISTSIZE
1000
root@1f4a993d950f:/# 
root@1f4a993d950f:/# HISTSIZE=2
root@1f4a993d950f:/# 
root@1f4a993d950f:/# date
Tue Jan 18 02:16:34 UTC 2022
root@1f4a993d950f:/# cal
bash: cal: command not found
root@1f4a993d950f:/# whoami
root
root@1f4a993d950f:/# history 
   34  whoami
   35  history 
root@1f4a993d950f:/# HISTSIZE=1000

```



