Электронная очередь - панель.
ТЗ:
В мед. учреждениии ведется предварительная запись на прием. Утром у администратора есть список пациентов, записанных на прием.
Необходимо, чтобы список пациентов выводился на монитор/инфомат и по мере приема пациентов удалялись записи с экрана
Панель: часть, отвечающая за вывод на экран/инфомат
Программа оператора: засть отвечающая за внесение данных в базу.


Запуск и подготовка:
1. Установить виртуальное окружение. Дополнительные библиотеки не требуются, все в рамках стандартного пакета. Версия Python 3.11.7
2. Файл базы данных baza.db разместить на сетевом ресурсе, либо в папке с общим доступом.
3. В файле программы main.py в функциях refresh_window и View в строке con1 = sqlite3.connect("\\\\path\\path\\path\\baza.db") прописать актуальный путь к базе данных.
4. В функции refresh_window в строке root.after(3000, refresh_window) - изменить 3000 на нужный период обновления окна(1000 = 1 секунде).


