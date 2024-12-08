To implement this:

1. Save this script as "/usr/local/sbin/ssh-country-check" with your changed config

2. Add this to /etc/ssh/sshd_config:
ForceCommand /usr/local/sbin/ssh-country-check

3. Make the script executable:
chmod +x /usr/local/sbin/ssh-country-check

4. Restart SSH service:
systemctl restart sshd
