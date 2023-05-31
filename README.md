# Предсказание зарплаты по описанию вакансии

## Задача
В рамках настоящего соревнования вам предлагается решить задачу предсказания зарплаты по описанию вакансии. Соревнование проходит в рамках буткемпа "Second Step In NLP", проводимого онлайн-магистратурой "Машинное обучение и высоконагруженные системы", ФКН ВШЭ.

## Данные
- Опыт работы <br><br>
![exp](img/exp.png) <br><br>
- Расписание <br><br>
![schedule](img/sch.png) <br><br>
- Вид занятости <br><br>
![employment](img/emp.png) <br><br>
- Распределение зарплаты <br><br>
![target](img/salary.png)

## Решение
Для решения сначала я чистил текст с помощью библиотеки nltk. <br>
После этого я решил использовать word2vec для векторного представления слов и на этих данных обучить ансамбль бустингов: CatBoost, LightGBM, XGBoost.

## Результат
Данное решение на приватном лидерборде по метрике R2 набрало 0.43.