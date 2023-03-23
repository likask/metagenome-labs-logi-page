# Metagenome Labs Hub

![figures/meta-genome-logo.png](figures/meta-genome-logo.png)

### Password and login

- On the first login, select the password
- The shell password on the SSH login is different than the JupyterHub password
- Ask admin for SSH password
- Change password in the shell using [passwd](https://man7.org/linux/man-pages/man1/passwd.1.html){:target="_blank" rel="noopener"} command
- Set up your shell with the command (e.g. bash):
~~~~
$ usermod --shell /bin/bash your_login_name
~~~~

### SSH config if you have account on cactus

You can lunch ssh server in container, and login to it in terminal or VSCode.

Copy the following code into .ssh/config on your laptop or desktop.
~~~~
Host metmateroal-lab
  HostName YOUR_HOST_NAME
  ForwardX11 yes
  Compression yes
  User YOUR_LOGIN_ON_HUB
  Port 2222
~~~~

Use *forward_greenstick* when you login in VSCode. Note tha you are connecting to *cactus* from which is tunnel to *geenstick*.

### Video on JuputerHub, SSH and MoFEM

[![Watch the video](https://img.youtube.com/vi/xL3J8VHig68/hqdefault.jpg)](https://youtu.be/xL3J8VHig68){:target="_blank" rel="noopener"}
