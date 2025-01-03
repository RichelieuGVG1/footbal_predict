# Прогнозирование в футболе

Этот проект содержит код для работы с набором данных, анализа, визуализации и решения задач регрессии с использованием методов машинного обучения.

1. Оценка "давления" на игрока
Алгоритм, который определяет, какое давление p оказывается на
каждого игрока в игре по информации о координатах этих же игроков x, y. На выходе алгоритм 
выдает давление от времени p(t) с визуализацией, также требуется построить гистограмму давления с
интерпретацией полученной природы распределения. 


2. Прогнозироване давления на игрока
Модель, для прогнозирования положения игрока x(t + τ ), y(t + τ ) на
временной горизонт τ и, как следствие, давления, оказываемого на него p(t + τ ). Выбираем
оптимальный временной горизонт τ , на котором качество предсказания модели считается приемлемым.
По сути это time series prediction.

## Структура

1. **Обработка данных:**
   - Загрузка и анализ CSV-файлов.
   - Работа с пропусками в данных (интерполяция).
   - Визуализация распределений и результатов.

2. **Модели машинного обучения:**
   - Построение регрессионных моделей с использованием `RandomForestRegressor`.
   - Кросс-валидация с помощью `TimeSeriesSplit`.
   - Метрики оценки: среднеквадратическая ошибка (MSE).

3. **Дополнительный функционал:**
   - Функции для построения графиков предсказаний.
   - Логика для подготовки данных под задачу регрессии.

## Установка зависимостей

Для выполнения проекта необходимы следующие библиотеки Python:
- `pandas`
- `numpy`
- `matplotlib`
- `scikit-learn`

Установите их с помощью команды:
```bash
pip install pandas numpy matplotlib scikit-learn
```

## Как использовать

1. Убедитесь, что все исходные файлы находятся в правильной директории.
2. Запустите код в среде Jupyter Notebook или другой, совместимой с `.ipynb` (например, Google Colab).
3. Следуйте инструкциям и комментариям в ячейках кода.

## Возможные улучшения

- Оптимизация гиперпараметров модели.
- Реализация других методов регрессии.
- Углубленный анализ ошибок и факторов.

## Авторство

Код написан для решения задач в рамках практики/задания.
