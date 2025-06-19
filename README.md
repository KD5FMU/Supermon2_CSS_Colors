# The Finished Product - *note this is for ASL3 only
![HRC Logo](https://github.com/KD5FMU/KD5FMU/blob/main/full-supermon.jpg)

# Have the ability to change these custom colors
![HRC Logo](https://github.com/KD5FMU/KD5FMU/blob/main/text-colors.jpg)

# Awesome Color effects when you are transmitting into the NODE
![HRC Logo](https://github.com/KD5FMU/KD5FMU/blob/main/background-color1.jpg)

# Cool Colors when the NODE is transmitting and receiving 
![HRC Logo](https://github.com/KD5FMU/KD5FMU/blob/main/background-color2.jpg)


# Prerequisite Install
Before you make these changes you need to install the Supermon2 MOD from Jory - W5GLE's GitHub page
```
https://github.com/hardenedpenguin/asl3_scripts
```

# Supermon 7.4 w/Supermon2 MOD css file & Python Script

These are my preferred supermon.css file and accompanying ast_node_status_update.py Pythin Script.

Goto the /var/www/html/supermon/ folder 
```
cd /var/www/html/supermon
```
Then rename the existing supermon.css file so that we can download the new one. We can do this with this command.
```
sudo mv supermon.css supermon.css.bak
```

Once this is done you can download this file

```
sudo wget https://raw.githubusercontent.com/KD5FMU/Supermon2_CSS_Colors/refs/heads/main/supermon.css
```


Then you can change the folder to the location we need to be in to get the updated python script.
```
cd /usr/local/sbin
```

Then we need to rename the existing file if it has already been installed
```
sudo mv ast_node_status_update.py ast_node_status_update.py.bak
```

Once this is done we can download the new file
```
sudo wget https://raw.githubusercontent.com/KD5FMU/Supermon2_CSS_Colors/refs/heads/main/ast_node_status_update.py
```

Then we need to make it executable
```
sudo chmod +x ast_node_status_update.py
```

No if you crontab entry is still in place with the ast_node_status_update.py entry it will update your Supermon page accordingly.

