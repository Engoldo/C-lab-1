# C-lab-1

## Лабораторная работа №1 (Стандартный ввод/вывод)

### **Задача №1**

```
  Написать программу, которая запрашивает у пользователя пол,
  рост и вес, а затем анализирует соотношение роста и веса, выда-
  вая рекомендации к дальнейшим действиям (похудеть, потолстеть,
  норма)
```

**Пояснение**

За основу расчета можно взять приблизительную оценку **Идеальный_вес=Рост-100** - для мужчин и **Идеальный_вес=Рост-110** - для женщин.

Программа должна состоять из двух функций:

  - **int getRecommendation(char gender, float height, float weight)** - анализ ситуации
  - **main()** - организация диалога
  
  Функция **getRecommendation** должна возвращать:
     - **-1** - вес недостаточен
     - **1** - вес избыточен
     - **0** - вес идеален
     
Необходимо подготовить следующие файлы:

 * **task1.h** - содержит одну строку: **int getRecommendation(char gender, float height, float weight);**
 * **task1.c** - содержит реализацию функции
 
   ```
      #include "task1.h"
      int getRecommendation(char gender, float height, float weight)
      {
         // здесь реализация
      }
   ```
 * **main1.c** - содержит реализацию **main**:
   ```
      #include "task1.h"
      int main()
      {
         // здесь реализация
      }
   ```  
 
 ### **Задача №2**
 
  ```
    Написать программу, которая запрашивает текущее время в 
    формате ЧЧ:ММ:СС, а затем выводит приветствие в зависимости от
    указанного времени ("Доброе утро "Добрый день"и т.д.)
  ```

**Пояснение**

  За границы можно принять следующие значения: 
  - "ночь" - с 00:00 до 06:00
  - "утро" - с 06:00 до 11:00
  - "день" - с 11:00 до 18:00
  - "вечер" - с 18:00 до 00:00
  
Программа должна состоять из двух функций:

  - **char * greet(int hour,int min)** - генерация приветствия и провека корректности времени
  - **main()** - организация диалога
  
Функция **greet** должна возврщать одну из следующих строк:
  - "Good night!"
  - "Good morning!"
  - "Good day!"
  - "Good evening!"
  - "Uncorrect time!"


Необходимо подготовить следующие файлы:

 * **task2.h** - содержит одну строку: **char * greet(int hour,int min);**
 * **task2.c** - содержит реализацию функции
 
   ```
      #include "task2.h"
      char* greet(int hour,int min)
      {
         // здесь реализация
      }
   ```
 * **main2.c** - содержит реализацию **main**:
   ```
      #include "task2.h"
      int main()
      {
         // здесь реализация
      }
   ```  
 ### **Задача №3**
 
  ```
     Написать программу, которая переводит значение угла из граду-
     сов в радианы, и, наоборот, в зависимости от символа при вводе.
     Например: 45.00D - означает значение в градусах, а 45.00R - в
     радианах. Ввод данных осуществляется по шаблону %f%c
  ```
  **Пояснение**
  
Программа должна состоять из двух функций:

  - **char * convert(char buf[], double angle, char type)** 
  - **main()** - организация диалога
  
Функция **convert** должна заполнять буфер **buf** строкой, содержащей значение угла в градусах или радианах,
в зависимости от значений входных параметров. 

Пример: **convert(buf, 180.0, 'D')** выдает строку: **3.14159R**.
Пример: **convert(buf, 3.14159, 'R')** выдает строку: **180.0D**.

Необходимо подготовить следующие файлы:

 * **task3.h** - содержит заголовок функции **convert**.
 * **task3.c** - содержит реализацию функции **convert**.
 
   ```
      #include "task3.h"
      char * convert(char buf[], double angle, char type)
      {
         // здесь реализация
      }
   ```
 * **main3.c** - содержит реализацию **main**:
   ```
      #include "task3.h"
      int main()
      {
         // здесь реализация
      }
   ```  
  
  ### **Задача №4**
 
  ```
    Написать программу, которая переводит рост из американской си-
    стемы (футы, дюймы) в европейскую (сантиметры). Данные вво-
    дятся в виде двух целых чисел, выводятся в виде вещественного
    числа с точностью до 1 знака. 1 фут = 12 дюймов. 1 дюйм = 2.54
    см.
  ```
  **Пояснение**
  
Программа должна состоять из двух функций:

  - **float convert(int feet,int inches)** 
  - **main()** - организация диалога
  
Ввод данных в программу осуществляется в виде:  **футы'дюймы**, например **5'11**.  
  
Необходимо подготовить следующие файлы:

 * **task4.h** - содержит заголовок функции **convert**.
 * **task4.c** - содержит реализацию функции **convert**.
 
   ```
      #include "task4.h"
      float convert(int feet,int inches)
      {
         // здесь реализация
      }
   ```
 * **main4.c** - содержит реализацию **main**:
   ```
      #include "task4.h"
      int main()
      {
         // здесь реализация
      }
   ```  
  
  ## Список веток репозитория
  
| ФИО             | Название ветки |
| --------------- | ------------- |
| Кулагин А.      | b1  |
| Алексеева В.    | b2  |
| Пойлов К.       | b3  |
| Мартьянов А.    | b4  |
| Королева В.     | b5  |
| Политов А.      | b6  |
| Балахонов В.    | b7  |
| Котрикова К.    | b8  |
| Спирин А.       | b9  |
| Назаренко А.    | b10  |
| Перепелкин С.   | b11  |
| Голобородько А. | b12  |
| Мольков А.      | b13  |
| Дамбинова И.    | b14  |
| Миронова Е.     | b15  |
| Тимофеев В.     | b16  |
| Комаров Н.      | b17  |
