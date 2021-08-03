# Demo REST API for SML
[![Build Status](https://travis-ci.com/dziuzin/SmlTestTask.svg?branch=main)](https://travis-ci.com/dziuzin/SmlTestTask)

для запуска: 

1. Из скрипта v1 инициализировать структуру БД (PostgreSql)
2. Поменять в appsettings.json строку подключения под свою БД
3. Запустить проект
4. Описание API доступно по пути /swagger


Структура проекта: 

* BLL - слой логики
* DAL - слой доступа к данным
* ReactApplication - API


Суффиксы: 

* Interface - абстракции части 
* Local - локальные реализации
* Test - тесты слоя. Включены юниты
* Stub - заглушки слоя для юнитов верхних слоёв

Используется DI на уровне класса-координатора через стандартный механизм (файл Startup.cs)
