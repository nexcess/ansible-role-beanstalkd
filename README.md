# Beanstalkd Ansible Role
This role was developed to work with Centos7, Centos6, Ubuntu 12.04, Ubuntu 14.04, Debian 7.4, Debian 6.4 and RHEL.

## Settings

There are not a lot of variables for this. Currently `binlog_dir` doesn't appear to be working with Ubuntu.

```
# basic preferences
beanstalkd_user: beanstalkd
beanstalkd_port: 11300
beanstalkd_address: 0.0.0.0
beanstalkd_job_size: 65535

# setup persistence and binlog
beanstalkd_binlog: yes
beanstalkd_binlog_dir: /var/lib/beanstalkd/binlog
beanstalkd_binlog_sync: 0
beanstalkd_binlog_size: 10485760
``` 