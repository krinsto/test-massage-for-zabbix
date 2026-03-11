# RU


### Это тестовый узел сети Zabbix для проверки оповещений. Простой способ протестировать систему уведомлений.


1. Импортируйте узел сети "Zabbix-test-massage.yaml".


2. Назначьте ему группу узлов, на которую настроены оповещения.


3. В командной строке выполните:

```
zabbix_sender -z 127.0.0.1 -s "TEST" -k test.alert -o 1
```

1 — создаёт проблему.
0 — закрывает проблему.


После выполнения команда создаст проблему на указанном узле.


#### ВАЖНО: оповещения должны быть уже правильно настроены, иначе уведомления отправляться не будут.


# ENG


### This is a Zabbix test host used to verify alert notifications. It is a simple way to test the notification system.


1. Import the host "Zabbix-test-massage.yaml".


2. Assign it to the host group where alerts are configured.


3. Run the following command in the terminal:

```
zabbix_sender -z 127.0.0.1 -s "TEST" -k test.alert -o 1
```

1 — creates a problem.
0 — resolves the problem.


After running the command, a problem will appear on the specified host.


#### IMPORTENT: alerts must already be configured correctly, otherwise notifications will not be sent.
