#Сортировка файлов при ограниченном буфере 

#Этапы алгоритма:
1)Открываем поток для считывания исходного файла
2)В соответствии с размером буфера делим наш файл на n частей 
3)Сортируем n файлов с помощью std::sort() 
4)Открываем n потоков и считываем n первых строк каждого файла
5)Сравниваем строки, наименьшую заносим в выходной файл
6)Выполняем пункт 5 пока не будут закрыты все файлы
7)Закрываем 
