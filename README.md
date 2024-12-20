# gpt_2_fine_tuning
Fine tuning модели архитектуры gpt-2 (библиотека transformers) на наборе данных новостей.

Ноутбук включает следующие этапы:
1.	Загрузка и подготовка данных:
    * подготовка текстового корпуса для обучения модели
    * очистка данных
    * разделение данных на тренировочный и валидационный наборы
    * токенизация текстов

2.  Создание модели на основе трансформера:
    * инициализация трансформера (в данном случае GPT)

3.	Обучение модели:
    * настройка гиперпараметров, таких как размерность векторного представления, число эпох и скорость обучения
    * выбор наилучшего оптимизатора (из трёх: Adam, SGD, RMSProp) и исследование их влияние на процесс обучения
    * использование learning rate scheduler для управления скоростью обучения

4.	Оценка модели:
    * пример генерации текста (модель продолжает текст)
    * оценка моделей по метрикам Perplexity, BLEU и ROUGE

6.	Анализ результатов:
    * сравнение результатов моделей с разными оптимизаторами и scheduler'ами


**P.S.** Ноутбук выполнялся на gpu, предоставляемых Kaggle.
