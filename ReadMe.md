# Лабораторна робота

## Установка

Відкрити головну папку в терміналі і запустити

```bash
docker run --name=riak -d -p 8087:8087 -p 8098:8098 basho/riak-kv
```
## Налаштування
Далі зайти в консоль через докер

```bash
docker exec -it riak /bin/bash
```
Ствроимо ДБ

```bash
riak-admin bucket-type create test_db
```
Та активуємо
```bash
riak-admin bucket-type activate  test_db
```

Далі для роботи

Треба встановити PostMan та імпортувати в постман файл riak.postman_collection.json

[Documentation](https://linktodocumentation)

В Постмані є запити
 - Список всіх бикетів
 - Додати просто текст
 - Додати Json
 - Отримати по ключу
 - MapReduce








