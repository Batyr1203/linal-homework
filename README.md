### Домашняя работа по численным методам:
1. Точные методы решения СЛАУ (homework1)
2. Итерационные методы решения СЛАУ (homework2)
3. Интерполяция
   - Базовая часть (homework3)
   - Супербонус (superBonus)
4. Уравнения переноса и теплопроводности (homework4)
   -  'transfer.gif', 'thermal.gif'
   
### Описание программ в самих ноутбуках!

# Точные методы решения СЛАУ

### Постановка задачи:
Пусть известны матрица вещественных чисел $A\in \rm I\!R ^{n*n}$ и вектор правой части $f\in \rm I\!R^n$ уравнения:
<img src="https://latex.codecogs.com/svg.latex?\Large&space;Ax = f" \>
Требуется найти вектор $x \in \rm I\!R^n$, из этого уравнения.


###### Для каждого из методов время решения будем сравнивать с временем вычислений соответствующих библиотечных функций, а сами решения будем сравнивать с помощью функции *numpy.linalg.norm()*. Матрица и правая часть уравнения генерируются  случайным образом.

#  




# Метод Гаусса

Пусть $A=LU$, где $L-$ нижнетреугольная матрица, $U-$ верхнетрегольная матрица с единицами на главной диагонали:
$$LUx=f.$$


**Прямой ход**: привести матрицу к улучшенному верхнетреугольному виду элементарнымипреобразованиями строк.
$$Ux = L^{-1}f.$$
**Обратный ход**: привести матрицу кк диагональному виду элементарными преобразованиями строк.
$$x = U^{-1}L^{-1}f.$$

### Асимптотика алгоритмической сложности:
1. прямого хода: $\Theta(n^3);$
2. обратного хода: $\Theta(n^2);$
3. метода Гаусса : $\Theta(n^3)$.

## Результаты программы
My time:  [0.15822672843933105, 0.5739479064941406, 1.3904681205749512, 2.341061592102051, 3.7289059162139893]
lib_time:  [0.025662899017333984, 0.0018117427825927734, 0.0182340145111084, 0.009048938751220703, 0.016607999801635742]


<img src="https://latex.codecogs.com/svg.latex?\Large&space;x=\frac{-b\pm\sqrt{b^2-4ac}}{2a}" title="\Large x=\frac{-b\pm\sqrt{b^2-4ac}}{2a}" />


