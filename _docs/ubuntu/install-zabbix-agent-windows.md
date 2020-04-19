# Установка (install) Zabbix Agent

[Zabbix Агенты](https://www.zabbix.com/ru/download_agents)

## Windows

- Создать папку c:\zabbix_agentd
- Распаковать файлы

### Скачать Windows - i386 - OpenSSL
[Zabbix Агенты](https://www.zabbix.com/ru/download_agents)

### Настроить
в файле
```
C:\zabbix_agentd\zabbix_agentd.conf
```
указать
```
Server=[IP-ADDRESS]
ServerActive=[IP-ADDRESS ZABBIX Сервера]
Hostname=[HOSTNAME]
```
где [IP-ADDRESS] - адрес zabbix сервера;
    [HOSTNAME]   - имя компьютера где запущен агент

Важно! [HOSTNAME] должен совпадать с [Имя узла сети] в zabbix

### Установить службу
```
zabbix_agentd.exe -c c:\zabbix_agentd\zabbix_agentd.conf --install
```

### Запустить службу
```
zabbix_agentd.exe --start
```