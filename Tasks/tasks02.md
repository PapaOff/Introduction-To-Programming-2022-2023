# Зад 1. 
Напишете функция, която проверява дали две матрици са идентични.

```cpp
//ROWS = 3
//COLS = 5

int matrix1[ROWS][COLS] = { {1, 2, 3, 4, 5},
			    {6, 7, 8, 9, 10},
			    {11, 12, 13, 14, 15} };

int matrix2[ROWS][COLS] = { {1, 2, 3, 4, 5},
			    {6, 7, 8, 9, 10},
			    {11, 12, 13, 14, 15} };
                           
int matrix3[ROWS][COLS] = { {0, 2, 3, 4, 0},
			    {6, 0, 8, 0, 10},
		            {11, 0, 13, 0, 15} };

cout << (check(matrix1, matrix2) ? "They are equal" : "They are not equal") << endl;
cout << (check(matrix1, matrix3) ? "They are equal" : "They are not equal") << endl;
```

Изход:
```
They are equal
They aren't equal
```

# Зад 2.
Да се напише фунцкия add, която приема 3 матрици с еднакъв размер и записва сбора на първата и втората в третата.
```
1 1 1      0 -1 -1     1 0 0
1 1 1  +  -1  0 -1  =  0 1 0
1 1 1     -1 -1  0     0 0 1
```


# Зад 3. 
Напишете функция, която приема два масива (и размерите им), един указател и една променлива заразмер.

Пренасочете указателя да сочи към масива, чиято сума на елементите е по-малка, както и да промени стойността на последния аргумент, за да съответства с размера на минималния масив.

```cpp
int arr1[] { 1, 2, 3, 4, 5 };
int arr2[] { 9, 9, 9 };
int* ptr;
int size;

findMinAndPointToIt(arr1, 5, arr2, 3, ptr, size);

printArray(ptr, size)
```
Изход:
```
9 9 9
```