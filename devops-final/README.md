## Dockerfile

![img.png](img.png)

- Сборка зависимостей на стадии сборки.
- Перенос зависимостей и кода на финальную стадию.
- Настройка окружения и запуск Django-приложения.


## docker-compose.yml

![img_1.png](img_1.png)
![img_2.png](img_2.png)
![img_3.png](img_3.png)

- Сборка и запуск веб-приложения.
- Настройка Loki для сбора логов.
- Настройка Grafana для визуализации логов из Loki.

## grafana/provisioning/datasources/loki.yaml

![img_4.png](img_4.png)

- Этот YAML файл настраивает Loki как источник данных в Grafana:
- Grafana будет использовать Loki для сбора и отображения логов.

## build.sh

![img_5.png](img_5.png)

- Убеждаемся, что пользователь передал необходимый аргумент (тег) при запуске скрипта. Если тег не передан, скрипт выводит подсказку и завершает работу

## run.sh

![img_7.png](img_7.png)

- запуск Docker Compose с указанным тегом для сборки и запуска контейнеров в фоновом режиме.


### запускаем 
![img_8.png](img_8.png)

![img_9.png](img_9.png)

![img_13.png](img_13.png)

### контейнер

![img_12.png](img_12.png)

### образы 

![img_11.png](img_11.png)


### сайт
-- все работает как и раньше
![img_14.png](img_14.png)

### Loki

![img_15.png](img_15.png)

![img_16.png](img_16.png)

![img_17.png](img_17.png)

![img_18.png](img_18.png)

![img_19.png](img_19.png)


