# Итоговая проверочная работа

## 1. На GitHub создан репозиторий.
## 2. При помощи Draw.io создана блок-схема основной программы и блок-схема метода формирования массива из строк, длина которых меньше или равна трём символам. Файлы добавлены в репозиторий, создан коммит, отправлен на GitHub.
## 3. Сформировано текстовое описание решения в виде файла Readme.md. Создан коммит, отправлен на GitHub.
## 4. При помощи IDE Visual Studio Code на языке C# написана программа, решающая поставленную задачу. Создан коммит, отправлен на GitHub. Описание программы:
### 4.1. Программа состоит из трёх методов:
#### 4.1.1. Метод GetStringArray. Формирует массив из строк и возвращает его. Запрашивает у пользователя произвольную строку (строковый массив), разделителями элементов массива являются символы 'пробел'. Методом Split из полученной от пользователя строки формируется строковый массив, содержащий подстроки данной строки, разделённые символом 'пробел'. Если пользователь ввёл нулевую строку, то размер выходного строкового массива обнуляется для последующего корректного вывода в соответствии с шаблоном из ТЗ.
#### 4.1.2. Метод PrintArray. Печатает массив в соответствии с заданным в ТЗ шаблоном. Аргумент - строковый массив. Если массив пустой, то печатаются [], иначе методом Join собирается строка из элементов полученного массива строк с необходимыми разделителями элементов. Внутренние кавычки изолированы при помощи обратного слэша.
#### 4.1.3. Метод GetStringArrayThreeSymbol. Формирует массив из строк, длина которых меньше или равна трём символам, и возвращает его. Аргумент - строковый массив. Поскольку изначально неизвестно количество элементов в новом массиве, а использование коллекций не рекомендуется ТЗ, то в начале своей работы метод создаёт выходной массив строк размером 0. Далее при помощи цикла foreach метод последовательно получает все элементы входного строкового массива и сравнивает количество символов (их длину) с 3. В случае длины <= 3 метод меняет размер выходного массива (увеличивает на 1 при помощи Array.Resize) и записывает в новую ячейку выходного массива текщий элемент входного массива. Если длина > 3 текущий элемент никуда не записывается. После окончания поэлементного перебора входящего массива метод возвращает выходной массив.
### 4.2. Основная программа очищает консоль, и поочерёдно вызывает метод формирования массива строк, метод печати (печатает сформированный массив строк), метод формирования массива строк с длиной <= 3 символов и метод печати (печатает новый массив строк). Вызов последних двух методов реализован через передачу возвращаемого значения одного метода в качестве аргумента другого.
## 5. В работе над проектом использован контроль версий. Разработка алгоритма, текстового описания решения и программы расположены в разных коммитах.

