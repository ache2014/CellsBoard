# Программа для демонстрации знаний

### Задача:
Дана доска размером M × N клеток. Клетка может находиться в одном из двух состояний: 1 — живая, 0 — мёртвая. Каждая клетка взаимодействует с восемью соседями. Правила таковы:  
- Живая клетка, у которой меньше двух живых соседей, погибает.
- Живая клетка, у которой два или три живых соседа, выживает.
- Живая клетка, у которой больше трёх живых соседей, погибает.
- Мёртвая клетка, у которой три живых соседа, возрождается.

Напишите программу, которая будет:
- случайным образом генерить стартовое состояние;
- уметь получать его из файла (способ выбирается через параметры запуска в консоли);
- каждую секунду выводить в консоль новое состояние доски.

### Результат:
Для того чтобы создать доску с дефолтным размером (10x10) и случайным состоянием клеток, введите в консоли:

    python cells_interaction.py
Для того чтобы создать доску размером M x N и случайным начальным состоянием клеток, введите в консоли:

    python cells_interaction.py M N
    
Для того чтобы создать доску из файла "path/to/file", введите в консоли:

    python cells_interaction.py -f path/to/file
    
Файл должен выглядеть следующим образом (0 - мертвая клетка, 1 - живая):
```
01010101010101
11001100110010
11001101010000
00010010001111
11010100010111
```