# E-Commerce Order Value Classification

Проект машинного обучения и анализа [транзакционных данных](https://www.kaggle.com/datasets/carrie1/ecommerce-data) интернет-магазина в Великобритании и других странах в период 2010-2011 гг.

---
###  Цели проекта

- Провести исследовательский анализ транзакций e-commerce.
- Проверить статистические гипотезы, влияющие на поведение покупателей.
- Построить ML-модель для классификации заказов как "высоких" или "обычных".
- Продемонстрировать владение Pandas, статистикой, визуализациями и ML-инструментами.

---
### Проведённый анализ

### Статистика и EDA:
- Распределения и выбросы по цене и количеству товаров
- Анализ чеков по странам, категориям товаров, дням недели
- Построены доверительные интервалы и проведены:
  - t-тесты и U-тесты для UK vs non-UK
  - сравнение новых и постоянных клиентов
  - оценка разброса по типам товаров


###  Машинное обучение

 *Используемые модели:*
- Logistic Regression (baseline)
- Decision Tree Classifier
- Random Forest Classifier
- XGBoost Classifier

###  Результаты (F1-score для класса "высокий заказ"):

| Модель            | Accuracy | F1-score (HighValue) |
|-------------------|----------|-----------------------|
| LogisticRegression| 0.82     | 0.81                  |
| Decision Tree     | 0.87     | 0.88                  |
| Random Forest     | 0.87     | 0.87                  |
| XGBoost           | **0.88** | **0.88**              |

### Feature importance (XGBoost):

- Значимые признаки: Quantity, UnitPrice, Country, Weekday, Month



