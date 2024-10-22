OSSEC

sudo cat /var/ossec/logs/alerts/alerts.log | grep rootcheck
sudo /var/ossec/bin/active-response -l

sudo /var/ossec/bin/ossec-control start
sudo /var/ossec/bin/ossec-control restart
sudo /var/ossec/bin/ossec-control stop

Fail2ban
sudo fail2ban-client status sshd

sudo systemctl enable fail2ban
sudo systemctl start fail2ban

