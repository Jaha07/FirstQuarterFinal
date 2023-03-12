# Итоговая проверочная работа.

> Данная работа необходима для проверки ваших знаний и навыков по итогу прохождения первого блока обучения на программе разработчик. Мы должны убедиться что базовое знакомство с it прошло успешно.

Задача алгоритмически не самая сложная, однако для полценного выполнения проверочной работы необходимо:

- [x] Создать репозиторий на GitHub
- [x] Нарисовать блок-схему алгоритма (можно обойтись блок-схемой основной содержательной части, если вы выделяете ее в отдельный метод)
- [x] Снабдить репозиторий оформленным текстовым описанием решения (файл README.md)
- [x] Написать программу, решающую поставленную задачу
- [x] Использовать контроль версий в работе над этим небольшим проектом (не должно быть так что все залито одним коммитом, как минимум этапы 2, 3 и 4 должны быть расположены в разных коммитах)


## Задача

Написать программу, которая из имеющегося массива строк формирует массив из строк, длина которых меньше либо равна 3 символа. Первоначальный массив можно ввести с клавиатуры, либо задать на старте выполнения алгоритма. При решении не рекомендуется пользоваться коллекциями, лучше обойтись исключительно массивами

Примеры:
``` C#
{"hello", "2", "world", ":-)"} // -> {"2", ":-)"}

{"1234", "1567", "-2", "computer science"} // -> {"-2"}

{"Russia", "Denmark", "Kazan"} // -> {}
```


## Описание решения

Программа решающая поставленную задачу написана по принципам функционального программирования.
1. Реализован пользовательский ввод массива строк, если пользователь откажется от ввода, будет использован случайный массив из примеров задания. 
2. Чтобы добавить гибкость решению и избавиться от "магических значений", добавлен пользовательский выбор длины строки для отбора. Пользователь может отказаться от выбора длины строк для отбора. В случает отказа пользователя или, если программе неудастся преобразовать введенную строку к целочисленному значению, будет использовано значение по умолчанию (3), согласно условиям задачи.
3. Результат отбора строк по указанной длине записывается в новый массив, чтобы сохранить исходные данные.
4. Отбор и вывод результата разнесены в отдельные функции.

Проведена отладка решения, в ходе тестирования багов не обнаружено. 