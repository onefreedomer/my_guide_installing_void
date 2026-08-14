Рекомендуемые настройки дисплея:
![Пример настроек](vbox_display_settings.png)

Подключение образа дополнительной гостевой ОС:
![Расположение кнопки для подключения образа дополнительной гостевой ОС](guest_cd.png)

Установка `base-devel` и `linux-headers`:
```bash
sudo xbps-install base-devel linux-headers
```

Монтирование образа и запуск установки драйвера:
```bash
sudo mount /dev/cdrom /mnt
sudo /mnt/VBoxLinuxAdditions.run
sudo reboot
```

Запуск сервисов VirtualBox:
```bash
# для просмотра статуса сервиса: rcvboxadd status
sudo rcvboxadd start
sudo rcvboxadd-service start
```