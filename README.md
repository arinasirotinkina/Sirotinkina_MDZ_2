# Сиротинкина Арина Дмитриевна, БПИ-234

**Мини дз 2**

## Описание проекта

Веб-приложение для автоматизации бизнес-процессов зоопарка:
Реализовано на ASP.NET Core 8.0 с in-memory хранением данных


## Архитектура

  Zoo.Domain/           # Модели предметной области
  
  Zoo.Application/      # Сервисы и интерфейсы бизнес-логики
  
  Zoo.Infrastructure/   # In-memory репозитории
  
  Zoo.Presentation/     # ASP.NET Core Web API

### Domain

- Сущности
- Value Objects
- Общие базовые классы
- Доменные события

### Application

- Интерфейсы репозиториев и событий
- Сервисы

### Infrastructure 

- In-memory реализации репозиториев  
- хранение и публикация доменных событий в консоль  

### Presentation 

- ASP.NET Core Web API  
- AnimalsController, EnclosuresController, FeedingController, StatisticsController 
- Program.cs

## Domain-Driven Design

- Содержательная модель предметной области  
- Инкапсуляция бизнес-правил
- Использование Value Objects
- Публикация доменных событий при изменении состояния

## Clean Architecture

- Разделение на слои: Domain → Application → Infrastructure → Presentation  
- Зависимости только внутрь через интерфейсы  
- Изоляция бизнес-логики от инфраструктуры и UI

## Запуск проекта

cd Zoo.Presentation
dotnet run
