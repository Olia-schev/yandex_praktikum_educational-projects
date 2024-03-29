# **Исследование поведения пользователей сервиса аренды самокатов**

**Описание проекта**

Популярному сервису аренды самокатов GoFast требуется помощь в проверке некоторых гипотез для увеличения выручки. Есть данные о некоторых пользователях из нескольких городов, а также об их поездках. 

**Задачи**

Проверить гипотезы:
* Тратят ли пользователи с подпиской больше времени на поездки? 
* Можно ли сказать, что расстояние, которое проезжают пользователи с подпиской за одну поездку, не превышает 3130 метров? 
* Будет ли помесячная выручка от пользователей с подпиской по месяцам выше, чем выручка от пользователей без подписки. 
* Снизилось ли количество обращений в поддержку после обновления сервера, с которым взаимодействует мобильное приложение?

Решить задачи с помощью распределений:
* Какое минимальное количество промокодов нужно разослать, чтобы вероятность не выполнить план была примерно 5 %. Подобрать параметры распределения, описывающего эту ситуацию.
*  С помощью аппроксимации построить примерный график распределения и оценить вероятность того, что уведомление откроют не более 399,5 тыс. пользователей.


**Что было сделано в ходе проекта**

Проведен анализ общей информации о пользователях сервиса аренды самокатов GoFast, включая статистические тесты для проверки нескольких гипотез относительно поведения пользователей с подпиской и без нее. 


**Ценность проекта для бизнеса**

Полученные выводы в результате исследования помогли компании GoFast улучшить их маркетинговые стратегии, оптимизировать условия подписки и улучшить пользовательский опыт


**Инструменты**
* python
* pandas
* matplotlib
* numpy
* math
* scipy

**Навыки**

Обработка данных, histogram, boxplot, статистический тест, критерий Стьюдента


**Структура проекта:**
- [Описание данных;](#review)
- [Загрузка данных;](#loading_data)
- [Предобработка данных;](#preprocessing)
- [Исследовательский анализ данных;](#analysis)
- [Объединение данных;](#merging)
- [Подсчёт выручки;](#revenue)
- [Проверка гипотез;](#hypotheses)
- [Распределения;](#distribution)
- [Общий вывод.](#results)


**Выводы**

**При исследовательском анализе и  проверке гипотез были сделаны следующие выводы:**
* Количество пользователей из разных городов в выборке от 168 до 219;
* Основная возрастная категория пользователей — это люди от 25 до 28 лет;
* В среднем продолжительность поездки составляет 15-20 минут;
* Пользователи с подпиской являются наиболее "выгодными" для компании так как они тратят больше времени на поездки и приносят больше прибыли, чем пользователи без подписки;
* Пользователи без подписки чаще передвигаются на самокате на малые расстояния ( до 1000 метров);
* Так же было выявлено, что в среднем пользователи проезжают около 3130м и более, что является критичным значением для износа самокатов.


**При решении задач для отдела маркетинга GoFast были получены следующие результаты:**
*  В ходе акции с раздачей промокодов на один бесплатный месяц чтобы как минимум 100 существующих клиентов продлили подписку необходимо разослать не менее 120 промокодов. 
* Вероятность того, что  push-уведомления в мобильном приложении откроют не более 399,5 тыс. пользователей составляет 15,37%

**Рекомендации для бизнеса**
1. Учитывая, что пользователи с подпиской приносят больше прибыли, рекомендуется активно продвигать подписочную модель. Это может включать в себя предложения, целенаправленные на увеличение числа подписчиков через бонусные программы, персонализированные предложения и улучшение условий для подписчиков.

2. Учитывая, что пользователи без подписки чаще используют самокаты на небольшие расстояния, компания может сосредоточить усилия на оптимизации использования самокатов в городах, где это актуально. Например, расширение зон обслуживания, снижение тарифов на короткие поездки и т.д.

3. На основе результатов о критичном значении среднего пробега пользователей рекомендуется уделить внимание управлению износом самокатов. Это может включать в себя планы по обновлению парка самокатов, ремонт и техническое обслуживание для предотвращения выхода самокатов из строя.
