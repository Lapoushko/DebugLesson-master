# Расширенные возможности debug


## Задание

Выполнить задания из класса [MatrixInitializer](src/main/java/ru/urfu/MatrixInitializer.java)

     *     <li>Найти значение sum, при котором происходит исключение
     *         (поставить breakpoint на возникающее исключение и воспользоваться стеком вызовов)</li>
sum = -4390925508
С помощью кнопки Create Breakpoint, которая появляется при ошибке  
     *     <li>Исправить ошибку <b>Важно исправить именно ошибку в существующей логике,
     *         а не добавлять свою логику!</b><br>
Чтобы восстановить логику, необходимо изменить строчки         long left = j > 0
                                                                      ? matrix[i][j - 1]
                                                                      : 1L;
Если визуализировать двумерный массив как таблицу, то можем заметить, что происходит смещение
из нижнего правого угла в левый вверхний. А строчка matrix[i+1][j - 1] 
sum, в таком случае, станет 8556409792055465576
     *         В качестве ответа надо написать какое изменение вы сделали.</li>
     *     <li>Найти значение value перед добавлением значения элемента массива с индексами [95][30]
     *         (нужно использовать условия)</li> 
value = 11
В condition указал для matrix[i][j] i = 95; j = 30
     *     <li>Вычислить значение выражения (up - left + 1) * j / 4 для i = 57, j = 28
     *         (для вычисления нужно использовать окно EvaluateExpression [Alt + F8])</li>
При использовании этого окна результат при текущих значениях будет равен 21
     *     <li>Добавить breakpoint в метод {@link #getValue(long[][], int, int)},
     *         нужно остановиться только когда значение sum станет больше 2300
     *         (нужно в методе test добавить breakpoint (на нём останавливаться не нужно),
     *         после которого должен сработать ранее созданный breakpoint).
     *         Найдите значение выражения up + left
     *         (для вычисления нужно использовать окно EvaluateExpression [Alt + F8])</li>
     *     <li>Вывести в лог значение sum, когда i == j
     *         (<b>Код изменять нельзя! И на точке не останавливаемся!</b>)
     *         Найти сколько раз встречается значение sup по модулю меньше 10 000
     *         (ничего автоматизировать не нужно, достаточно просто посмотреть, что выведено в лог)</li>