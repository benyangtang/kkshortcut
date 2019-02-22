# kkshortcut
linux directory shortcuts, for easy navigation of directories.

```
== inistallation
Pretty easy. 
1. Put the file kkcmd into a directory in command path, e.g., /usr/bin, or $HOME/bin.
2. Source the file bashrckk. You can put this into the bash initialization source:
echo '. bashrckk' >> .bashrc

== command list
kk -- change dir
kka -- assign a shortcut to a dir
kkd -- delete a shortcut
kkl -- list shortcuts
kkg -- search shortcuts
kkv -- set environment variables for shortcuts
kku -- unset the environment variables

== examples
Suppose you are in your home directory /home/myname
mkdir -p aazz/bbzz/cczz/ddzz/eezz
cd aazz/bbzz/cczz
kka cc # assigns shortcut 'cc' to /home/myname/aazz/bbzz/cczz
cd ddzz/eezz
kka aa  # assign shortcut 'aa' to /home/myname/aazz/bbzz/cczz/ddzz/eezz
kk cc  # change to directory /home/myname/aazz/bbzz/cczz
kk aa  # change to directory /home/myname/aazz/bbzz/cczz/ddzz/eezz
kkl    # list all shortcuts
kkl a c # list shortcuts whose first letter is from 'a' to 'c'
kkg ee # search shortcuts whose dirs contain 'ee'
kkv aa  # assign an environment variable kkaa whose value is the dir path.
cp myFile $kkaa # copy myFile to the dir represented by the shortcut aa
kku aa # unset the environment variable kkaa.
```

