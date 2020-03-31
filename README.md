# Тестовое задание

Приложение `app.py` написано с использованием фрэймворка Flask. По запросу

    curl http://localhost:5000/

показывает номер текущего посещения. По запросу

    curl http://localhost:5000/metrics

отдает метрику `hello_world_counter` в формате Prometheus.

Все пункты задания опциональны, Вы можете остановиться на любом пункте,
например, если Вы не укладываетесь по времени, просто пришлите результат.
   1. Создайте Dockerfile для приложения `app.py`;
   2. Создайте конфигурацию (на выбор) docker-compose, Docker swarm или
      Kubernetes, запускающую контейнеры:
      * приложения `app.py`;
      * Prometheus с настройкой сбора метрики приложения `app.py`;
      * Grafana;
   3. В Grafana создайте дэшборд, отображающий количество посещений в секунду
      на графике, экспортируйте его в Json-файл;
   4. Любым удобным инструментом (например Apache bench) проверьте,
      справляется-ли приложение `app.py` с нагрузкой в 100 запросов в секунду.
      Соберите вывод тестового инструментария и снимите скриншот графика
      количества посещений, если он есть;

Отправьте все результаты любым удобным способом.
