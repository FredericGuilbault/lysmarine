
# Set local time
By default, lysmarine time is set on GMT.
To choose your location, navigate to `/usr/share/zoneinfo/`
Find the file corresponding to your location (`America/Montreal` in this example)
Then copy it to `/etc/localtime`  
```
sudo cp /usr/share/zoneinfo/America/Montreal /etc/localtime
```

# Passwords
> lysmarine come with default password. You are strongly advised to change them.

 - Change the default user (pi) password with the `passwd` command.
 - Il you plan to use VNC, change the default password with the command `vncpasswd`.
 - Create signalk a administrative account: Go to Menu > Signal K   In the browser, Press Login button upper right.


### Aditional configurations
 - There is no root password set by default. You are expected to do everything through sudo.
   But if you need one, you can set it with `sudo passwd root`

 - [Enable SSH](doc/userdoc/vnc.md)
 - [Enable VNC](doc/userdoc/ssh.md)



Firewall ?   **__TODO__**
Sudo with no password ? **__TODO__** conflicting with openplotter
