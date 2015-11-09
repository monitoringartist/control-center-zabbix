Zabbix server Control Center template
=====================================

[Dockerized Zabbix Server 2.4](https://github.com/zabbix/zabbix-community-docker/) 
template for [Zenoss Control Center](http://controlcenter.io/) (Docker orchestration tool)

[![Paypal donate button](http://jangaraj.com/img/github-donate-button02.png)]
(https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=8LB6J222WRUZ4)

Installation
============

- Import provided template
- Deploy Zabbix Application
- Start and use it, note: first start can take 2-3 minutes, because default 
database must be imported
- Default Zabbix web credentials: Admin/zabbix

Known issues
============

- health checks are failing

Troubleshooting
===============

Check if app is running:

```
[ccuser@ccmaster]  curl -sk --header 'Host: zabbix.local' 'https://127.0.0.1:443' | grep 'by Zabbix SIA'
                                                                Zabbix 2.4.6 (2015-11-03) Copyright 2001-2015 by Zabbix SIA
```

If you can see this output in command line '*by Zabbix SIA' and you are not able to see app in your browser, then you have some problem with DNS records/hosts file.

Author
======

[Devops Monitoring zExpert](http://www.jangaraj.com 'DevOps / Docker / Zabbix / Zenoss / Monitoring'), who loves monitoring 
systems, which start with letter Z. Those are Zabbix and Zenoss.

Professional monitoring services:

[![Monitoring Artist](http://monitoringartist.com/img/github-monitoring-artist-logo.jpg)]
(http://www.monitoringartist.com 'DevOps / Docker / Zabbix / Zenoss / Monitoring')
