# Домашнее задание к занятию 4 «Оркестрация группой Docker контейнеров на примере Docker Compose»
## Задача 1
https://hub.docker.com/r/borbul2007/custom-nginx
## Задача 2
![virt-03-docker-intro-task2](https://github.com/user-attachments/assets/14de21b3-2d87-4dcf-bff1-9eebad07dd2a)
## Задача 3
![virt-03-docker-intro-task3](https://github.com/user-attachments/assets/7b88889f-de15-4434-935e-020588eb13bf)
Для внимательных ответ есть на снимке экрана. Выделен зеленым цветом. Дублирую:\
Удалили единственный запущенный процесс, контейнер завершил своё выполнение.
## Задача 4
![virt-03-docker-intro-task4](https://github.com/user-attachments/assets/db2234c1-3b18-43b0-a99c-1e6ee3c2c9d8)
## Задача 5
![virt-03-docker-intro-task5](https://github.com/user-attachments/assets/7056e6ad-7415-485c-95e0-2ae39419847e)
Для внимательных ответ есть на снимке экрана. Выделен зеленым цветом. Дублирую:\
Если присутствуют оба файла, будет использован compose.yaml\
WARN[0000] Found orphan containers ([task5-portainer-1]) for this project. If you removed or renamed this service in your compose file, you can run this command with the --remove-orphans flag to clean it up.\
docker-compose принимает имя каталога, в котором он находится, в качестве имени проекта по умолчанию и предупреждение возникает из-за того, что docker compose при запуске обнаруживает контейнеры, которые принадлежат другому проекту с таким же именем.\
\
![virt-03-docker-intro-task5-portrainer-containers-inspect](https://github.com/user-attachments/assets/e868e785-6c52-4903-8d58-b11dc1d6c7e1)
Если выполнить "docker compose up -d" в контексте выполнения задания выдает "no configuration file provided: not found" - ожидаемо, т.к. мы только, что удалили файл на предыдущем шаге.

## Моё мнение (можно не читать)
> В целом норм. Есть ошибки и не однозначности.\
>  Задача 1 - Если задача про пуш, то сделать легко, url предоставлен, если про url - непонятно, как делать.\
>  Задача 5 - п.4 - "https://127.0.0.1:9000"  - ожидаемо не работает;\
>  Задача 5 - п.7 - выполнение "docker compose up -d" в контексте выполнения задания выдает "no configuration file provided: not found" - ожидаемо. Оказавается не надо было переименовывать docker-compose.yam перед include, что логично на мой взгяд )
