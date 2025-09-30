# ДОКУМЕНТАЦИЯ СИСТЕМЫ AS/400 (Insurance Claims & Billing System)

## 📋 ОБЗОР

Бизнес-документация системы обработки страховых полисов и претензий AS/400. Система включает 32 модуля MOB для управления страховыми полисами, претензиями, биллингом и защитой от долгов.

> **📖 Полный индекс документации:** [INDEX.md](./INDEX.md)

## 📁 СТРУКТУРА ДОКУМЕНТАЦИИ

### 🏗️ Основные документы

1. **[BUSINESS_DOCUMENTATION.md](./BUSINESS_DOCUMENTATION.md)** - Полная бизнес-документация
   - Бизнес-процессы системы
   - Описание всех модулей MOB
   - Интеграции и отчетность
   - Планы миграции

2. **[MODULES_REFERENCE.md](./MODULES_REFERENCE.md)** - Справочник модулей
   - Полный список 32 модулей MOB
   - Детальное описание каждого модуля
   - Классификация по категориям
   - Статистика и планы миграции

3. **[BRD_INSURANCE_SYSTEM.md](./BRD_INSURANCE_SYSTEM.md)** - Бизнес-требования
   - Цели и задачи системы
   - Заинтересованные стороны
   - Критерии успеха
   - Соответствие требованиям

### 📊 Дополнительные файлы

4. **[PROJECT_DOCUMENTATION.md](./PROJECT_DOCUMENTATION.md)** - Общая документация проекта
   - Архитектура системы
   - Функциональные области
   - Хронология разработки

5. **[MODULE_DOCUMENTATION.md](./MODULE_DOCUMENTATION.md)** - Детальная документация модулей
   - Технические характеристики модулей
   - Статистика по сложности

6. **[SYSTEM_OVERVIEW.md](./SYSTEM_OVERVIEW.md)** - Краткий обзор системы
   - Основные характеристики
   - Статус и планы
   - Ключевые показатели

## 📁 ИСХОДНЫЕ ФАЙЛЫ

### Архитектурные диаграммы
- **[AS400ReplacementFlowChart.pdf](./AS400ReplacementFlowChart.pdf)** - Диаграмма архитектуры системы
- **[AS400 to FourPoint Export_Manual.pdf](./AS400%20to%20FourPoint%20Export_Manual.pdf)** - Руководство по экспорту данных

### Бизнес-процессы (Excel)
- **[DCC Coverage.xls](./DCC%20Coverage.xls)** - Покрытие DCC
- **[DCC New Business Process.xls](./DCC%20New%20Business%20Process.xls)** - Процесс новых бизнес-процессов
- **[DCC Premium Allocation Process.xls](./DCC%20Premium%20Allocation%20Process.xls)** - Процесс распределения премий
- **[DCC Premium Process.xls](./DCC%20Premium%20Process.xls)** - Процесс премий
- **[Sovereign DCC Claims Export Process.xls](./Sovereign%20DCC%20Claims%20Export%20Process.xls)** - Экспорт претензий
- **[Sovereign DCC Premium Export Process.xls](./Sovereign%20DCC%20Premium%20Export%20Process.xls)** - Экспорт премий
- **[Sovereign DCC Premium Import Process.xls](./Sovereign%20DCC%20Premium%20Import%20Process.xls)** - Импорт премий

### Техническая документация
- **[Greg_s notes on Premium Allocation Processing.pdf](./Greg_s%20notes%20on%20Premium%20Allocation%20Processing.pdf)** - Заметки по обработке премий
- **[as400 tables by pgm.xlsx](./as400%20tables%20by%20pgm.xlsx)** - Таблицы AS/400 по программам
- **[iSeries Job Scheduler (2).xls](./iSeries%20Job%20Scheduler%20(2).xls)** - Планировщик заданий iSeries

## 🚀 БЫСТРЫЙ СТАРТ

### Основные характеристики
- **Система:** AS/400 (Insurance Claims & Billing System)
- **Модулей MOB:** 32
- **Функциональность:** Обработка страховых полисов и претензий, биллинг, защита от долгов
- **Статус:** В эксплуатации (планируется миграция на C#)

### Функциональные области
- **Страховой биллинг** - MOB265, MOB266, MOB267
- **Обработка претензий** - MOB269X, MOB269XP, MOB269XP2
- **Защита от долгов** - MOB290-295
- **Пакетная обработка** - MOB201, MOB258
- **Коммуникация данных** - MOB206OB-209ENC

## 📚 ИСПОЛЬЗОВАНИЕ ДОКУМЕНТАЦИИ

### Для бизнес-пользователей
1. Начните с [BUSINESS_DOCUMENTATION.md](./BUSINESS_DOCUMENTATION.md) для понимания процессов
2. Используйте [MODULES_REFERENCE.md](./MODULES_REFERENCE.md) как справочник по модулям
3. Изучите [BRD_INSURANCE_SYSTEM.md](./BRD_INSURANCE_SYSTEM.md) для понимания требований

### Для аналитиков
1. Используйте [MODULES_REFERENCE.md](./MODULES_REFERENCE.md) для анализа функциональности
2. Обратитесь к [PROJECT_DOCUMENTATION.md](./PROJECT_DOCUMENTATION.md) для архитектуры
3. Изучите планы миграции в бизнес-документации

## ⚠️ ВАЖНАЯ ИНФОРМАЦИЯ

### Планы миграции
- **AS/400 помечена как "Decommissioned long ago"**
- **Планируется замена модулей Debt Protection (MOB290-295) на C# Window Service**
- **Остальные модули продолжают работать на AS/400**

---

**Дата создания документации:** 30 сентября 2024  
**Версия:** 1.0  
**Статус:** Актуально

## 🏷️ ТЕГИ

`AS/400` `Insurance System` `Claims Processing` `Billing Management` `Debt Protection` `MOB Modules` `Business Documentation`
