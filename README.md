# Message of the Day

Collection of my 'Message of the Day' scripts.

![motd](motd.png)


### Requirements

  * update-motd
  * figlet & lolcat (for `10-display-name`)


### How do I set it up?

Copy the files you want in your MOTD to `/etc/update-motd.d/`. Make sure you have the `PrintMotd`
option set to `yes` in your sshd config.

The duplicate files are different versions of the same, use either one of them. E.g. `30-zpool-simple`
will not print usage bars.

If you use `50-fail2ban` you should comment out the `compress` option in `/etc/logrotate.d/fail2ban`,
s.t. the logs are not compressed and can be grepped.
