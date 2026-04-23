# Predicting Employee Dismissal

## Описание проекта

Этот проект посвящен предсказанию увольнения сотрудников на основе набора данных из Kaggle (https://www.kaggle.com/datasets/tawfikelmetwally/employee-dataset/data). Проект включает разведочный анализ данных (EDA), предобработку, построение моделей машинного обучения и создание интерактивного интерфейса для предсказаний с использованием Gradio.

### Основные этапы проекта:
1. **Разведочный анализ данных (EDA)**: Анализ распределений, корреляций, пропусков и выбросов.
2. **Предобработка данных**: Отбор признаков, кодирование категориальных переменных, заполнение пропусков.
3. **Построение моделей**: Логистическая регрессия и Random Forest.
4. **Оценка и выбор модели**: Финальная модель - Random Forest с ROC-AUC 0.92 на тестовых данных.
5. **Инференс**: Интерактивное приложение на Gradio для предсказаний.

## Структура проекта

- `Predicting dismissal Shift.ipynb` - Jupyter Notebook с полным анализом, предобработкой и обучением моделей.
- `Predicting dismissal Shift.pptx` - Презентация с результатами проекта.
- `requirements.txt` - Список зависимостей для воспроизведения проекта.
- `train_data.zip` - Архив с обучающими данными (необходимо распаковать в папку `train_data`).

## Установка и запуск

### Требования
- Python 3.8+
- Jupyter Notebook
- Gradio (для интерактивного интерфейса)

### Установка зависимостей
```bash
pip install -r requirements.txt
```

### Запуск ноутбука
1. Распакуйте `train_data.zip` в папку `train_data`.
2. Откройте `Predicting dismissal Shift.ipynb` в Jupyter Notebook.
3. Выполните ячейки последовательно.

### Запуск Gradio приложения
В ноутбуке есть раздел с кодом для Gradio. После обучения модели запустите приложение для интерактивных предсказаний.

## Ключевые признаки
- **Числовые**: ОпытВДолжности, Активность, Возраст, Оценка_HR, УровеньОплаты, Офлайн_участие, Закрытые_проекты, ГодНайма, Курсы
- **Категориальные**: Образование, Город, Пол

## Результаты
- **Логистическая регрессия**: ROC-AUC на валидации ~0.85
- **Random Forest**: ROC-AUC на валидации ~0.96, на лидерборде 0.92

## Автор
Андрей Дутов

## Лицензия

MIT License

Copyright (c) 2026 Andrey Dutov

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.