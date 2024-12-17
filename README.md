# Фрактальное пламя

## Описание проекта

Программа реализует алгоритм генерации изображения фрактального пламени с использованием системы итерируемых функций. В программе реализовано две версии: однопоточная и многопоточная.

**Примеры сгенерированных изображений**

<div style="display: flex; justify-content: center;">
    <img src="IMAGES/Fractal_Flame_2024-11-27_23-31-41.PNG" width="500" />
    <img src="IMAGES/Fractal_Flame_2024-12-18_00-51-29.JPEG" width="500" />
</div>
<div style="display: flex; justify-content: center;">
    <img src="IMAGES/Fractal_Flame_2024-12-18_00-39-54.JPEG" height="333" />
    <img src="IMAGES/Fractal_Flame_2024-12-18_00-40-07.JPEG" height="333" />
    <img src="IMAGES/Fractal_Flame_2024-12-18_00-43-34.JPEG" height="333" />
</div>
<div style="display: flex; justify-content: center;">
    <img src="IMAGES/Fractal_Flame_2024-12-11_15-58-17.JPEG" width="500" />
    <img src="IMAGES/Fractal_Flame_2024-12-13_17-08-10.JPEG" width="500" />
</div>
<div style="display: flex; justify-content: center;">
    <img src="IMAGES/Fractal_Flame_2024-12-11_16-01-13.JPEG" width="500" />
    <img src="IMAGES/Fractal_Flame_2024-12-13_16-40-09.JPEG" width="500" />
</div>
<div style="display: flex; justify-content: center;">
    <img src="IMAGES/Fractal_Flame_2024-12-13_16-56-07.JPEG" width="500" />
    <img src="IMAGES/Fractal_Flame_2024-12-13_16-57-53.JPEG" width="500" />
</div>
<div style="display: flex; justify-content: center;">
    <img src="IMAGES/photo_2_2024-12-04_23-59-28.jpg" width="500" />
    <img src="IMAGES/photo_5_2024-12-04_23-59-28.jpg" width="500" />
</div>

***

## Функционал
- Реализация цветного алгоритма генерации фрактального пламени.
- Запуск в двух версиях: однопоточной и многопоточной.
- Сравнение времени работы обеих версий.
- Возможность настройки параметров: размера изображения, количества итераций.
- Возможность выбора из 11 трансформационных функций (выбрать можно одну или несколько).
- Возможность выбора параметра симметрии.
- Возможность выбора папки для сохранения изображений.
- Гамма-коррекция полученного алгоритмом изображения.

***
## Входные и выходные данные

### Ввод
Описание входных и выходных данных
Входные данные
- Размеры изображения (ширина и высота).
- Количество итераций функции для каждой точки (влияет на "заполненность" изображения).
- Показатель симметрии (степень двойки, где 0 - отсустствие симметрии).
- Директория для сохранения изображения (или выбор default папки).
- Выбор трансформаций из представленного списка (или случайный выбор).

### Вывод
- Два изображения, реализованные одно- и многопоточно, сохранённые по указанному при вводе пути.
- Скорость работы при однопоточной и многопоточной генерации. Для многопоточной дополнительно указано количество использованнных потоков.

***
## Тестирование

Тесты проверяют следующие аспекты:
- Корректность работы алгоритма на различных наборах параметров.
- Корректность трансформаций, преобразований, изменения цвета пикселя.
- Правильность работы гамма-коррекции получившегося изображения.
- Сравнение производительности одно- и многопоточной версий.

***
## Источники

* [Статья на хабре](https://habr.com/ru/articles/251537) с описанием фрактального пламени
* [Оригинальная статья об алгоритме](https://flam3.com/flame_draves.pdf) с каталогом вариаций
