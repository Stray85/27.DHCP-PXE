# Настройка PXE сервера для автоматической установки

## Цель: Отрабатываем навыки установки и настройки DHCP, TFTP, PXE загрузчика и автоматической загрузки

Описание/Пошаговая инструкция выполнения домашнего задания:
Для выполнения домашнего задания используйте методичку
https://docs.google.com/document/d/1f5I8vbWAk8ah9IFpAQWN3dcWDHMqXzGb/edit?usp=share_link&ouid=104106368295333385634&rtpof=true&sd=true
Что нужно сделать?

Следуя шагам из документа https://docs.centos.org/en-US/8-docs/advanced-install/assembly_preparing-for-a-network-install установить и настроить загрузку по сети для дистрибутива CentOS8.
В качестве шаблона воспользуйтесь репозиторием https://github.com/nixuser/virtlab/tree/main/centos_pxe.
Поменять установку из репозитория NFS на установку из репозитория HTTP.
Настроить автоматическую установку для созданного kickstart файла (*) Файл загружается по HTTP.

Указанного в методичке файла https://mirror.sale-dedic.com/centos/8.4.2105/isos/x86_64/CentOS-8.4.2105-x86_6 не существует, поэтому я заменил его на  
https://vault.centos.org/8.4.2105/isos/x86_64/CentOS-8.4.2105-x86_64-dvd1.iso

Так же в методичке ошибка - не хватает #</Directory> в конце pxeboot.conf
