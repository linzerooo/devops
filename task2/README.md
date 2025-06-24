Задание по Ansible:

Написать playbook который должен будет:
- Создать пользователя на удаленной машине.
- Дать пользователю права sudo.
- Сделать авторизацию ssh по ключам для пользователя.
- Отключить авторизацию по паролю при ssh подключении.
- Создать директорию в /opt/ с правами 660 для пользователя.


Установка Ansible выполнена стандартным способом:
```
sudo apt update
sudo apt install ansible -y 
ansible --version 
```

<img width="775" alt="image" src="https://github.com/user-attachments/assets/9d92546c-7279-4eee-ba28-7be80992e90d" />

Для безопасного доступа создан SSH-ключ 

```
ssh-keygen -t ed25519 -f ~/.ssh/russia_fb_ed25519 -C "ansible-admin-key"```

Файл inventory.txt содержит детали подключения:

```
ssh-keygen -t ed25519 -f ~/.ssh/russia_fb_ed25519  ```

Playbook выполняется командой:
``` ansible-playbook -i inventory.txt playbook.yml hw2.yml ```
<img width="1046" alt="image" src="https://github.com/user-attachments/assets/5329a6c7-1ae3-4577-aa49-887444bf4c6e" />