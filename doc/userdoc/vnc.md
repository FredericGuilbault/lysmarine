Lysmarine use provide the x11vnc server to allow desktop sharing of the pi user.

The service is disabled by default for security reason. Prior to enable it you should :

 - set a VNC password with the command `vncpasswd`.

 To start for the service only for the current runtime:
 ```
 sudo systemctl start x11vnc.service
 ```

 If you want VNC to start automatically at boot:
 ```
 sudo systemctl enable x11vnc.service
 ```

To prevent dissable the automatic launch at boot :

```
sudo systemctl stop x11vnc.service
```

By default, vnc is listening on the port **5900**. You can find your local IP with the command `ip addr`
