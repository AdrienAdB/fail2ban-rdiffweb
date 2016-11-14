# fail2ban-rdiffweb
Fail2Ban filter for rdiffweb

1) Add rdiffweb.conf file to /etc/fail2ban/filter.d/

2) Add below lines to /etc/fail2ban/jail.local

[rdiffweb]
enabled  = true
filter   = rdiffweb
logpath  = /var/log/rdiffweb.log
bantime = 600
findtime = 600
maxretry = 5
