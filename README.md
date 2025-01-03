# Проект по созданию модели для прогнозирования оттока клиентов из банка
Из «Бета-Банка» стали уходить клиенты. Каждый месяц. Немного, но заметно. Банковские маркетологи посчитали: сохранять текущих клиентов дешевле, чем привлекать новых.
Нужно спрогнозировать, уйдёт клиент из банка в ближайшее время или нет. Вам предоставлены исторические данные о поведении клиентов и расторжении договоров с банком.
Постройте модель с предельно большим значением F1-меры. Чтобы сдать проект успешно, нужно довести метрику до 0.59. Проверьте F1-меру на тестовой выборке самостоятельно.
Дополнительно измеряйте AUC-ROC, сравнивайте её значение с F1-мерой.

Источник данных: [https://www.kaggle.com/barelydedicated/bank-customer-churn-modeling](https://www.kaggle.com/barelydedicated/bank-customer-churn-modeling)

Используемые модели:
1) Решающее дерево (decision tree)
2) Случайный лес (random forest)
3) Логистическая регрессия (logistic regression)

В результате применения этих моделей и с учетом борьбы с дисбалансом классов были получены следующие метрики:

Decision tree (class_weight) - F1 = 0.5773 и AUC_ROC = 0.8031

Logistic regression (upsampling) - F1 = 0.5061 и AUC_ROC = 0.7866

Random forest (class_weight) - F1 = 0.6156 и AUC_ROC = 0.849
