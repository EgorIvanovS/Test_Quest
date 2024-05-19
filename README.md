# Тестовое задание для стажировки

## Описание
Данный репозиторий содержит выполненные задачи в рамках тестового задания для стажировки. 
Задания включают создание модуля на SystemVerilog для сложения двух чисел типа float32 и 
написание модуля для редукции ряда из N вещественных чисел до одного числа.


## Задание 1
При решении данного задания я нашел открытую библиотеку, реализующую суммирование двух чисел 
с плавающей точкой (https://github.com/nishthaparashar/Floating-Point-ALU-in-Verilog). Для 
реализации суммирования я написал элементарный модуль, который обращается к данной библиотеке.
По ссылке https://github.com/EgorIvanovS/Test_Quest/issues/1 я представил подробное описание 
библиотеки. Поэтапно я описал функции практически каждой строчки кода Verilog.
Помимо самого модуля я приложил в файл задания testbench модуля суммы.


## (Задание 2)*
Для редукции ряда из большого числа N вещественных чисел в одно число с использованием 
минимальных аппаратных ресурсов, мы можем использовать алгоритм параллельного суммирования 
и использовать обратное вычисление для минимизации задержек и ресурсов.
Этот модуль series_reducer сокращает задержки и использует параллельное суммирование для 
минимизации использования аппаратных ресурсов. Он принимает массив из N вещественных чисел
шириной WIDTH бит и возвращает их сумму. Ответ на выходе будет корректным на том такте, когда 
все входные числа будут добавлены в итоговую сумму, что происходит после N/2 тактов.







