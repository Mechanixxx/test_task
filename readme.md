#### Задание-навыки использования Bash


1. Скрипт "date.sh" в корне

##### Вывод списка файлов существующей директории
```
ls -la | tee /tmp/ls_exist_dir.txt
```
##### Попытку вывода списка файлов НЕ существующей директории
```
ls -la /noexist_dir | tee /tmp/ls_none_exist_dir.txt
```
##### Сгенерировать пары ключей, и научиться ходить с клиента на сервер по ssh без использования пароля
```
 	a) ssh keygen (создаем пару ключей id_rsa и id_rsa.pub, для примера директория будет /home/<username>/.ssh, пароль задавать не будем)
	b) ssh-copy-id -i /home/<username>/.ssh/id_rsa.pub <username>@server-one - прописываем id ключа на удаленном сервере в файл authorized_keys
	с) ssh <username>@server-one - подключаемся
```

#### UPD: Добавлен сервис монтиторинга погоды (использовал API Open Weather)  

Cтек Telegraf, InfluxDB, Grafana + дашборд Open Weather.
