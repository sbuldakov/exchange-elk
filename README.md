# Основные статьи
Статьи, в которых собираются и объясняются залитые конфиги можно посмотреть тут:
- https://habr.com/ru/company/raiffeisenbank/blog/516694/
- https://habr.com/ru/company/raiffeisenbank/blog/520378/

# filebeat
Используется исключительно для сбора логов. Парсинг на месте выполняется по минимуму.
Проверить синтаксис конфига можно через:

    .\filebeat.exe test config
    
# logstash
Весь разбор логов происходит в logstash. Сделано это сознательно для упрощения разбора разноформатных логов.
Проверить синтаксис конфига можно через:

    .\logstash.bat --config.test_and_exit -f .\logstash.conf
