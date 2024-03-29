# **Исследование надёжности заёмщиков — анализ банковских данных**
**Описание проекта**

Заказчик — кредитный отдел банка. Нужно разобраться, влияет ли семейное положение и количество детей клиента на факт погашения кредита в срок. Входные данные от банка — статистика о платёжеспособности клиентов.
Результаты исследования будут учтены при построении модели кредитного скоринга — специальной системы, которая оценивает способность потенциального заёмщика вернуть кредит банку.

**Что было сделано в ходе проекта**

Используя инструменты библиотеки Pandas, я обнаружила закономерности между семейным положением, количеством детей у заемщиков и своевременным погашением кредита. 

**Ценность проекта для бизнеса**

Эти выводы оказались значимыми для бизнеса, помогая банку при построении модели кредитного скорингa


**Инструменты**
* python
* pandas
* matplotlib

**Навыки**

Обработка данных, работа с дубликатами и пропусками, категоризация, декомпозиция

**Структура проекта:**

- [Описание данных;](#review)
- [Загрузка данных;](#loading_data)
- [Предобработка данных;](#preprocessing)
- [Исследовательский анализ данных;](#analysis)
- [Выводы](#results)

**Выводы**

**При анализе данных были выявлено, что зависимость между рассматриваемыми категориями и возвратом кредита в срок есть.** 

Были отмечены наименее надежные категории клиентов это: 
- клиенты с 1 или 2 детьми, 
- не женатые клиенты, 
- клиенты с низким доходом. 
- Хуже всего выплачивают кредиты на операции с автомобилем и получение образования.

Стоит отметить, что доли просрочек по каждой из категорий не сильно отличаются друг от друга (на 2-3 ед.). 

Из-за не репрезентативности выборок по некоторым категориям клиентов, возможно эти категории следует исследовать отдельно и более детально по большему количеству признаков (возраст, уровень образования, тип занятости и т.д.).

**Рекомендации, по улучшению сбора данных и настройке системы скоринга:**
- Рекомендовано отрегулировать систему валидации при выгрузке данных во избежание возникновения дубликатов. 
- Сделать все поля анкеты обязательными к заполнению клиентом, чтобы не допустить возникновения пропусков 
- Установить лимит для вводимых значений (например, чтобы пользователь не смог записать в анкете, что у него стаж более 1000 лет или -1 ребенок)
- Сделать автоматическую замену регистра, при заполнении полей со строковыми значениями, чтобы в анкете не было неявных дубликатов.
