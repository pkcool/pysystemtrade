# Application Monitoring

## Crontab logs

On a default installation the cron jobs get logged to
```
/var/log/syslog
```
To see just cron jobs in that logfile, run
```
grep CRON /var/log/syslog
```
To continuously monitor it, run
```
tail -F /var/log/syslog | grep CRON
```

could also view the logs using:
```
journalctl -u cron.service
```
