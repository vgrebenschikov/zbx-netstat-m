# Zabbix template for FreeBSD netstat -m report

## Prerequisites

Following pors are required:

- textproc/jq
- net-mgmt/zabbix?-agent

## Install 

1. Copy script to etc/zabbix.agent.d

```sh
  # cp netstat-m.conf /usr/local/etc/zabbix6/zabbix_agentd.conf.d/
  # service zabbix_agentd restart
```

2. Import template to Zabbix

Import zbx-netstat-m-template.json in zabbix template list with UI

## Rebuild template file

```sh
  # ./mk-zabbix-template
```
