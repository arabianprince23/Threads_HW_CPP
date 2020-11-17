# Threads_HW_CPP
## Домашняя работа №4 по учебному курсу "Архитектура вычислительных систем", ПИ, 2 курс, НИУ ВШЭ. 
#### В качестве источников информации выступили:
<!--ts-->
  * https://habr.com/ru/post/443406/ <br />
  * https://docs.microsoft.com/ru-ru/cpp/standard-library/thread-class?view=msvc-160&viewFallbackFrom=vs-2019 <br />
  * https://l.wzm.me/_coder/custom/parallel.programming/001.htm <br />
<!--te-->
#### Пояснительная записка к проекту представлена [здесь]().
#### Код программы представлен [здесь]().
### Вариант 5. 
Определить ранг матрицы. Входные данные: целое положительное число n, произвольная матрица А размерности n х n. Количество потоков является входным параметром, при этом размерность матриц может быть не кратна количеству потоков.
## Результаты работы программы
Правильность выполнения работы была проверена на многих тестах, ниже будут представлены некоторые из них.
## Тесты 1 - 2 (некорректные данные)
По логике вещей, количество потоков, переданных программе пользователем, должно быть меньше или равно размерности матрицы. В программе для этого организована проверка.
- **Введём размерность матрицы = 4, кол-во потоков = 12312. Программа не отрабатывает, выписывая соответствующее предупреждение.**</br>
  ![](Materials/incorrect1.png)</br>
  ![](Materials/incorrect1.1.png)</br>
- **Введём размерность матрицы = 4, кол-во потоков = 12312 (теперь уже ручным вводом). Программа не отрабатывает, выписывая соответствующее предупреждение.**</br>
  ![](Materials/incorrect2.png)</br>
## Тест 3 - 4 (корректные данные)
-**Ручной ввод параметров и матрицы.**
  ![](Materials/correct1.png)</br>
-**Считывание параметров и матрицы из файла.**
  ![](Materials/correct2.png)</br>
  ![](Materials/correct2.2.png)</br>
