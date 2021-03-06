## Материалы к лабораторным работам по дисциплине "Интеллектуальные системы"
Для выполнения работ потребуется "Python 2.7 + Jupyter Notebook"

### Задание ЛР1: 
Ознакомиться с методическими материалами и примерами выполнения команд.
Последовательно выполнить следующие шаги применительно к выборке данных, согласно варианту задания:
1. Провести первичный анализ всех данных
2. Обработать пропуски и привести нужные для работы признаки к числовому типу
3. Проверить взаимозависимость всех числовых признаков (корреляция)
4. Выбрать целевую переменную и признаки, оказывающие на нее влияние (целевая - 1 шт., признаки>=2 шт.) 
5. Подготовить данные выбранных признаков (выбросы, исключения, разделение на обучающую и проверочную части)
6. Построить  регрессионную модель для каждого выбранного признака:

    6.1) Получить коэффициенты линейной регрессии y(x) = K*x + B

    6.2) Получить оценку точности r2(MSE)

    6.3) Нанести график прямой y(x) = K*x + B поверх точечной диаграммы (выбранный признак, целевая переменная)

<br>
# Оформление отчета по ЛР-1

Тема письма: ИСиТ, группа, Фамилии 
Имя файла: LabIS_1_618_IvanovPetrov.ipynb


### Содержание отчета:

1. Результаты первичного анализа исходных данных

    1.1. Количество записей и признаков
    
    1.2. Смысловое описание признаков
    
    1.3. Типы данных столбцов и информация о пропусках
    
    1.4. Результат замены категориальных или ранговых данных на числовые
    
    1.5. Результат обработки пропущенных значений

2. Обоснование выбора целевой переменной и признаков для анализа

    2.1. Перечень вариантов целевых переменных, исходя из п. 1.2.

    2.2. Матрица коэффициентов корреляции
    
    2.3. Матрица смежности (графический вариант интерпретации взаимосвязей переменных)
    
    2.4. Информация о целевом значении и признаках на него влияющих 
    
    2.5. Результат отчистки выбранных признаков исходного массива от выбросов

3. Построение регрессионных моделей для всех выбранных признаков
    3.1. Уравнение линейной регрессии
    
    3.2. Оценка точности r2(MSE)

    3.3. График полученной линейной зависимости y(x) = K*x + B поверх точечной диаграммы (y: выбранный признак, x: целевая переменная)
    
    3.4. График плотности распределения ошибок

4. Выводы по результатам сравнительного анализа полученных регрессионных моделей 
<br>

# Установка Python 2.7 + Jupyter Notebook (для Windows)

#### Вар.1. Установка Anaconda
1. Перейти на страницу [https://www.anaconda.com/distribution/#download-section](https://www.anaconda.com/distribution/#download-section)
2. Cкачать установочный файл Anaconda Python 2.7 для выбранной системы Win/Mac/Linux 32/64-бит и пройти все шаги установки
3. Запустить через меню  пункт меню "Пуск -> Все программы -> Ananconda -> jupyter-notebook"

#### Вар.2. Установка Python 2.7 с ручной загрузкой пакетов
1. Перейти на страницу [https://www.python.org/downloads/release/python-2716/](https://www.python.org/downloads/release/python-2716/)
2. Cкачать установочный файл Python 2.7 для выбранной системы Win/Mac/Linux 32/64-бит и пройти все шаги установки
3. Открыть консоль команд "cmd" 

    3.1) перейти в папку с менеджером пакетов pip.exe
        - пример: >cd "c:\Program Files\Python27\Scripts\"

    3.2) перейти в папку с менеджером пакетов pip.exe

    3.3) выполнить команды установки дополнительных библиотек:

        - пример: >pip.exe install numpy scipy pandas sklearn seaborn matplotlib
        - пример: >pip.exe install pandas pandoc pydot pydot-ng pydotplus
        - пример: >pip.exe install jupyter jupyter_nbextensions_configurator jupyter_contrib_nbextensions
 
    3.4) выполнить команду запуска модуля Jupyter Notebook:
        - пример: >jupyter-notebook.exe