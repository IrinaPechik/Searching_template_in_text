# Практический анализ алгоритмов поиска вхождений строки-шаблона в тексте.
**Печик Ирина Юрьевна**

## Цель работы
* Реализация различных алгоритмов поиска вхождений заданного
паттерна (шаблона) в исходном тексте
* Экспериментальный анализ временной сложности алгоритмов
* Сопоставление теоретических и практических оценок временной
сложности алгоритмов
* Интерпретация экспериментальных результатов
# Рассматриваемые алгоритмы
* Наивный алгоритм с использованием простого посимвольного
сравнения
* Алгоритм Кнута-Морриса-Прата с применением стандартных граней
* Алгоритм Кнута-Морриса-Прата с применением уточненных граней
* Алгоритм Рабина-Карпа
# Тестовые данные
## 1. Виды текста для поиска шаблона:
* Случайно сгенерированный текст в
    бинарном алфавите
    * 10000 символов
    * 100000 символов
* Случайно сгенерированный текст в
    алфавите из 4 символов (а-ля
    последовательность ДНК)
    * 10000 символов
    * 100000 символов
## 2. Шаблон первого типа - без символа подстановки «?»:
Фрагмент исходного текста с
некоторой позиции i переменной
длины:
* 100-3000 символов
* Шаг длины шаблона - 100
## 2. Шаблон второго типа - с символом подстановки «?»:
В шаблон встраивается символ
подстановка, который может означать
любой символ из исходного алфавита. 

Фрагмент исходного текста с
некоторой позиции i переменной
длины:
* 100-3000 символов
* Шаг длины шаблона - 100 

В случайную позицию полученного
шаблона встраивается от 1 до 4 
символов подстановки

# Выходные сравнительные графики
* По всем алгоритмам:
    * Без символов подстановки, 10000 символов, бинарный алфавит
    * Без символов подстановки, 10000 символов, 4-символьный алфавит
    * Без символов подстановки, 100000 символов, бинарный алфавит
    * Без символов подстановки, 100000 символов, 4-символьный алфавит
    * С X символов подстановки, 10000 символов, бинарный алфавит
    * С X символов подстановки, 10000 символов, 4-символьный алфавит
    * С X символов подстановки, 100000 символов, бинарный алфавит
    * С X символов подстановки, 100000 символов, 4-символьный алфавит

* Усреднение результатов замеров проводится большим количеством тестирований
