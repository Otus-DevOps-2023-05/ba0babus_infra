# ba0babus_infra
ba0babus Infra repository

1) ssh -J denis@51.250.74.234 denis@10.130.0.20 - подключение через бастион одной командой


2) Подключение одной командой: в ~./ssh/config - добавил:

Host someinternalhost
        HostName 10.130.0.20
        ProxyJump denis@51.250.74.234
        User denis

Подключаться через алиас 'ssh someinternalhost'

3) Подпись LE - Адрес pritunl - https://51.250.74.234.sslip.io/


4)
bastion_IP = 51.250.74.234
someinternalhost_IP = 10.130.0.20
