## Задание 1
0 На снимке экрана есть версия\
2 personal.auto.tfvars\
3 "result": "EjoJQbO2ylC3O5mM"\
4 Имя ресурса должно начинаться с _ или буквы и должно быть - nginx.\
  Неправильное имя ресурса и должно быть resource "docker_image" "nginx"\
  Неверное имя должно быть "example_${random_password.random_string.result}"\
5\
![ter-homeworks-01-task1-1](https://github.com/user-attachments/assets/e399893b-d5a3-4227-a83e-52c807f61daf)

6 -auto-approve - автоматическое подтверждение\
7\
![ter-homeworks-01-task1-2](https://github.com/user-attachments/assets/69705c6a-9fbe-4bc4-b7d0-59447f7dc6e8)

8 keep_locally (Boolean) If true, then the Docker image won't be deleted on destroy operation. If this is false, it will delete the image from the docker local storage on destroy operation
