# AB_test_Karpov
Проведение АB-теста для нескольких наборов выборок, используя различные модификации метрики и методы сравнения групп.
_______
## Подробное описание задачи:  
Задача 2:   
(задачей 1 являлось проведение АА-теста, в отдельном репозитории)  
Необходимо проанализировать результаты эксперимента, который был проведен вместе с командой дата сайентистов. Эксперимент проходил с 2022-09-03 по 2022-09-09 включительно. Для эксперимента были задействованы 2 и 1 группы. В группе 2 был использован один из новых алгоритмов рекомендации постов, группа 1 использовалась в качестве контроля. Основная гипотеза заключается в том, что новый алгоритм во 2-й группе приведет к увеличению CTR. Задача — проанализировать данные АB-теста.  

Задача 3:  
Относительно недавно (в 2018-м году) исследователи из Яндекса разработали метод анализа тестов над метриками-отношениями, который в контексте нашей задачи можно назвать методом линеаризованных лайков. Проанализируйте тест между группами 0 и 3 по метрике линеаризованных лайков. В чем отличие? По аналогии проведите анализ по группами 1 и 2.  

## Использованные методы принятия решения по АВ-тесту:
- t-тест; 
- Пуассоновский бутстреп;
- тест Манна-Уитни;
- t-тест на сглаженном ctr (α=5);
- t-тест и тест Манна-Уитни поверх бакетного преобразования.

## Стек технологий и технические характеристики хранения данных:
- Jupiter Notebook, Python.
- Библиотеки numpy, pandas, pandahouse, seaborn, scipy.
- Загрузка данных с использованием SQL запроса, используя подключение к серверу с БД на Clickhouse.

## Оценка решения от преподавателей karpov.courses:
Задача 2:  
10 из 10 баллов.  
"Верно, выкатывать этот алгоритм явно не стоит! Но стоит потом провести дополнительный анализ того, почему вдруг возникла такая бимодальность."   

Задача 3:  
10 из 10 баллов.  
"В целом верно! Можно заметить, что линеаризация увеличивает чувствительность нашего теста к различиям."
