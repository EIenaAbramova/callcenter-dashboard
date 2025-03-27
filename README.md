# 📞 Дашборд для анализа работы колл-центра

## 📝 Описание  
Данный дашборд в Power BI предназначен для анализа эффективности работы колл-центра за 3 месяца. 
Визуализация охватывает вклад команд супервайзеров, ключевые количественные и качественные показатели, 
а также обеспечивает возможность фильтрации по месяцам.
- Процент звонков, обработанных командами супервайзеров.
- Общее количество поступивших звонков — общее количество входящих обращений за 3 месяца.
- Общее количество принятых звонков — число звонков, на которые операторы ответили.
- Суммарное время обработки звонков — отображается в формате ЧЧ:ММ:СС, помогает оценить нагрузку и эффективность.
- Фильтры по месяцам (Месяц-6, Месяц-7, Месяц-8) — июнь, июль, август, позволяют сравнивать динамику по временным периодам.

## 📂 Состав проекта  
- `callcenter-performance-dashboard.pbix` – Файл дашборда Power BI  
- `README.md` – Описание проекта  
- `data/` – (опционально) Исходные файлы данных  

## 📊 Ключевые показатели:
- Общее количество поступивших и принятых звонков  
- Общее и среднее время обработки звонков  
- Количество повторных звонков и переводов  
- Конверсия по предложенным услугам  
- Процент отказов (показатель потерь)  
- Распределение звонков по супервайзерам  
- Фильтрация по месяцам (Месяц-6, Месяц-7, Месяц-8)

## 🧮 Логика расчёта метрик / Metric Calculation Logic

**1. Процент звонков по супервайзерам / Percentage of Calls by Supervisor**  
Показывает долю звонков, обработанных каждой командой:
% звонков = (Принятые звонки командой) / (Общее количество принятых звонков) * 100

**2. Общее количество звонков / Total Incoming Calls**  
Сумма всех звонков, поступивших в контактный центр.

**3. Общее количество принятых звонков / Total Answered Calls**  
Сумма звонков, на которые операторы ответили.

**4. Общее время обработки звонков / Total Call Handling Time**  
Суммарная длительность всех звонков (в секундах), затем может быть переведена в формат hh:mm:ss.

**5. Фильтрация по месяцам / Monthly Filtering**  
Данные разбиты по месяцам для анализа динамики.

## 🖥️ Как использовать дашборд?  
1. Скачайте файл `callcenter-performance-dashboard.pbix`  
2. Откройте его в Power BI Desktop  
3. Загрузите или обновите свои данные через Power Query  
4. Используйте фильтры и элементы управления для изучения показателей

## 🚀 Используемые технологии  
- Power BI (визуализация, DAX, Power Query)  
- Excel (предобработка данных)  
- SQL / Python (опционально — для агрегации данных)

## 🎨 Примеры визуализаций  
Вот так выглядит дашборд:  
![Call Center Dashboard](./3.jpg)  


## 📜 Лицензия  
Проект распространяется под лицензией MIT — свободное использование с указанием авторства.  
См. файл `LICENSE`.
