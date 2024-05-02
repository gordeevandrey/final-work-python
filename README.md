## Моделирование движения тела

#### Цели работы: 
- Смоделировать движение тела, брошенного под углом к горизонту,
с помощью языка программирования Python
- Закрепить умение работать с основными конструкциями языка Python
- Попрактиковаться в моделировании реальных физических процессов

#### Описание работы
##### 1. Построение аналитической модели без учёта сопротивления воздуха.
Реализован интерактивный график траектории тела, который динамически отрисовывается при каждом изменении угла броска и начальной скорости.
##### 2. Анализ выборки параметров а и b в зависимости от начальной скорости v из файла dataset.csv
Найдены квартили выборки измерений скорости из столбца v набора данных, записаны в файл quartiles.csv
Найдены параметры линейной регрессии между параметром a и скоростью, построен график со значениями из датасета и линия полученной регрессии.
 Найдены параметры регрессии между параметром b и скоростью, построен график.
Коэффициенты полученных уравнений записаны в coeff.csv


##### 3. Построение численной модели с учётом сопротивления воздуха.
Реализована функция, которая по заданным параметрам находит решение системы ОДУ.
Найдено решение системы ОДУ при при отсутствии сопротивления воздуха, а также при параметрах, полученных из третьего квартиля выборки прошлого задания.
Построены графики с размерными и безразмерными величинами
Найдены дополнительные параметры полета (дальность, время, высота подъема), записаны в файл results.txt