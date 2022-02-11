# ***Lab report 3***
***

# Streamlining ssh connection

The config file we need to edit is in the home dir in . file called .ssh

$ ```cd ~/.ssh```
![Image](cd_to_.ssh_file.png)

Since were not making a huge edit to the file I just used the built in editor called nano and copypasta the highlighterd text with the User that is connected to my school account.

$ ```nano config```
![Image](nano_config.png)

Since we already setup a public private key pair with ieng6 in a past lab, we only need to type

$ ```ssh ieng6``` 

to log in.
![Image](sshieng6.png)

If I want to I can change the login alias to anything I want by changing the name after ```Host``` in the config file.

This also works for ```scp```.
![Image](test_scp.png)

![Image](check_scp.png)

easy peasy 