Отчет по практической работе с виртуальными машинами на ОС Linux Ubuntu 24.04.2

Работа начинается с создания и настройки виртуальных машин А, Б и С - сервера, шлюза и клиента соответственно.
Ниже предствлены скрины настройки виртуальных машин и их состояние:
![3 VM C](https://github.com/user-attachments/assets/aea185b9-502e-4e87-8646-738c90d8d457)
![2 VM B](https://github.com/user-attachments/assets/da9744cf-cc18-4d5b-8a47-9d854e0ad308)
![1 VM A](https://github.com/user-attachments/assets/e800ffc2-1e71-4821-8a16-a0d3fe862c1b)

---

На всех трех виртуальных машинах был изменён 'hostname' в соответствии с заданием:
![1 hostname and add user](https://github.com/user-attachments/assets/b6477e76-06de-4855-bf62-1acdab0898a2)
![2 hostname and add user](https://github.com/user-attachments/assets/342684de-5ae1-4ea0-a460-dcbc3a8738ae)
![3 hostname and add user](https://github.com/user-attachments/assets/70036e6b-164f-47d0-b8a6-ed1d698f2d61)

В итоге получилось присвоить виртуальным машинам новые 'hostname':
ВМ А - asowslaserver <br> ВМ Б - asowslagateway <br> ВМ С - asowslaclient

А так же на всех трех виртуальных машинах успешно были добавлены новые пользователи 'not_asowsla' и присвоены пароли для авторизации

---

Далее была произведена конфигурация виртуальных интерфейсов на всех трех виртуальных машинах:
![1 configuration](https://github.com/user-attachments/assets/2185bfec-72ec-4fa8-87de-5b413970cd0f)
![2 configuration](https://github.com/user-attachments/assets/dd83cf2e-5b1b-45fd-a64d-f67c447ec4c0)
![3 configuration](https://github.com/user-attachments/assets/f7e060b5-3731-4e7a-80a8-c7a007a3dd23)

На ВМ А был для 'enp0s3' был выставлен автоматический айпи-адрес, а для 'enp0s8' - 192.168.31.10/24 в соответствии с заданием; <br>
На ВМ Б был для 'enp0s3' был также выставлен автоматический айпи-адрес, для 'enp0s8' - 192.168.31.1/24, а для enp0s9 - 192.168.3.1/24 в соответствии с заданием; <br>
На ВМ С был для 'enp0s3' выставлен автоматический айпи-адрес, а для 'enp0s8' - 192.168.3.1/24 в соответствии с заданием;
