# Fix when WiFi Networks do not appear in Ubuntu MATE

Note sure wy this is a problem, but on my Ubuntu MATE 16.04 install the WiFi networks sometimes do not show up in the pull-down menu. To fix, do the following:

```
sudo touch /etc/NetworkManager/conf.d/10-globally-managed-devices.conf
sudo service network-manager restart
```

