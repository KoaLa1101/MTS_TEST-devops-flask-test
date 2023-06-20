# Тестовое задание

В коде изменен запуск фласка - добавлено прослушивание всех хостов.

Приложение завернуто в Docker.
Для запуска `docker-compose up -d --build`

Grafana: https://grafana-test.koala1101.ru/d/a135baa4-03fa-4846-95fe-0433b47643d1/

---

### Проверка, что сервис держит >100 rps

![](/Users/rinat.r.ahmethanov/Desktop/Снимок экрана 2023-06-20 в 16.10.53.png)
![](/Users/rinat.r.ahmethanov/Desktop/Снимок экрана 2023-06-20 в 16.11.00.png)

---
```name=promql
sum(rate(hello_world_counter[30s])) by (instance)
```

