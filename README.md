### Описание проекта
А/А-тестирование мобильного приложения. Необходимо посчитать результаты A/A-теста, проверяя метрику качества FPR (будем проверять на конверсии в покупку). Известно, что сплит-система сломана. Требуется проверить утверждение о поломке и найти ее причины, если сплит-система действительно сломана

#### Описание колонок
experimentVariant – вариант эксперимента
version – версия приложения
purchase – факт покупки
 
#### Задача
1. Запустить A/A-тест
2. Посчитать FPR на уровне альфа = 0.05 (ставьте подвыборки без возвращения объемом 1000). Вы увидите, что FPR > альфа! Нам нужно наоборот – чтобы было меньше.
3. Найти причины поломки сплит-системы, ориентируясь на результаты эксперимента.
4. Написать выводы, которые можно сделать на основе анализа результатов A/A-теста

#### ВЫВОД.
Покрутив датафрейм нашли поломку в версии v2.8.0.
Затем статистически доказали наличие ошибки в версии v2.8.0 и перепроверили себя исключив версию с багом.
