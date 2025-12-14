# Домашнее задание к работе 3
## Условие задачи
Написать и отладить программу вычисления объема куба и площади его боковой поверхности по заданной длине ребра.
## 1. Алгоритм и блок-схема
### Алгоритм
1. **Начало**
2. Ввод входных данных:
   - `dl`  — длина ребра куба.

3. Вычислить объем куба:
   - `ob = dl**3`
5. Вычислить площадь боковой поверхности:
   - `plosh = 4 * dl**2`
6. Вывести результаты расчётов с подстановкой значений в текст.
7. **Конец**
### Блок схема
<img width="121" height="631" alt="lab3" src="https://github.com/user-attachments/assets/b43cddbc-fd7d-47fb-a147-358fb570ef1f" />

# Реализация программы

```
#define _CRT_SECURE_NO_WARNINGS
#include <stdio.h>
#include<locale.h>
#include <math.h>


int main() {

    setlocale(LC_ALL, "RUS");

    float dl;  // длина ребра 
    float ob;       // объем 
    float plosh;    // площадь боковой поверхности

    printf("Введите длину ребра куба: ");
    scanf("%f", &dl);


    ob = pow(dl, 3); // объем 

    plosh = 4 * pow(dl, 2); // площадь бок поверхности


    printf("Длина ребра куба: %.2f\n", dl);
    printf("Объем куба: %.2f\n", ob);
    printf("Площадь боковой поверхности: %.2f\n", plosh);

    return 0;

}
```
# Результат программы
<img width="338" height="99" alt="image" src="https://github.com/user-attachments/assets/7a79fa73-21f7-4457-a39c-ca5edd705648" />
