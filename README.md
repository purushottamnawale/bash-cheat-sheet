# Shell/Bash/Terminal Cheat Sheet

##### Go to a folder/directory
```
cd “path/to/directory/"
```
##### Go back to previous folder
```
cd ..
```

##### List files in particular folder
```
ls “path/to/directory/"
```

#### List files in current folder
```
ls
```

##### Install or Update modules from requirements.txt
```
pip3 install -r requirements.txt
```


##### Install or Update requirements.txt
```
pip3 freeze > requirements.txt
```

##### Switch User
```
sudo -u <user_name>
```


##### Install a tar.xz file
```
tar xf <filename.tar.xz>
cd <filename>
./configure
make
sudo make install
```




### Create a Bash Profile with Aliases
```bash
# Open Bash Profile
nano ~/.bashrc

alias sysupdate="snap refresh && sudo apt update -y && sudo apt upgrade -y && sudo apt autoremove -y"
alias open_higher_studies="cd /mnt/A0EA88F2EA88C5CE/Data/higher-studies && code ."
alias open_latex="cd /mnt/A0EA88F2EA88C5CE/Data/latex && code ."
alias open_firefox="(firefox 2>/dev/null & disown)"
alias open_all="sysupdate && open_higher_studies && open_latex && open_firefox"

# Refresh the bash profile
source ~/.bashrc
```